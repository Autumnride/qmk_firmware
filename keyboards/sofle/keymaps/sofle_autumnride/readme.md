![SofleKeyboard default keymap](https://i.imgur.com/MZxVvm9.png)
![SofleKeyboard adjust layer](https://i.imgur.com/f5sKy0I.png)

# Default keymap for Sofle Keyboard

Layout in [Keyboard Layout Editor](http://www.keyboard-layout-editor.com/#/gists/76efb423a46cbbea75465cb468eef7ff) and [adjust layer](http://www.keyboard-layout-editor.com/#/gists/4bcf66f922cfd54da20ba04905d56bd4)

Features:

- Symmetric modifiers (CMD/Super, Alt/Opt, Ctrl, Shift)
- Various modes, can be switched (using Adjust layer and the selected one is stored in EEPROM.
- Modes for Qwerty and Colemak support
- Modes for Mac vs Linux/Win support -> different order of modifiers and different action shortcuts on the "UPPER" layer (the red one in the image). Designed to simplify transtions when switching between operating systems often.
- The OLED on master half shows selected mode and caps lock state and is rotated.
- Left encoder controls volume up/down/mute. Right encoder PGUP/PGDOWN.

## Workflow & Erkenntnisse (Wichtig für KI-Unterstützung)

Falls dieses Keyboard in Zukunft angepasst werden soll, hier sind die wichtigsten technischen Rahmenbedingungen:

### 1. Build-Prozess

QMK erkennt Änderungen in der `keymap.c` manchmal nicht automatisch, wenn der Cache noch Fragmente enthält.

- **Wichtig:** Vor dem Kompilieren immer den Build-Ordner löschen:
  `rm -rf .build/ && qmk compile -e CONVERT_TO=promicro_rp2040 -kb sofle/rev1 -km sofle_autumnride`

### 2. VIA vs. C-Code (rules.mk)

- Damit Änderungen in der `keymap.c` sofort nach dem Flashen aktiv werden, ist `VIA_ENABLE = no` in der `rules.mk` gesetzt.
- Wäre VIA aktiv (`yes`), würde die Tastatur das Layout aus dem EEPROM laden und Änderungen im Code ignorieren, bis der EEPROM gelöscht wird.

### 3. Flashen beider Hälften

- Bei Änderungen an der Konfiguration (`rules.mk`, `config.h`) müssen **beide Hälften** einzeln geflasht werden.
- Bei reinen Tastenänderungen in `keymap.c` reicht oft die Master-Hälfte (meist links), aber beide Seiten zu flashen ist sicherer für die Synchronität.

### 4. Debugging von Tasten

- Wenn Tasten (wie F6/F8) nicht reagieren: Erst mit einfachen Buchstaben (z.B. `KC_A`) in der `keymap.c` testen. Wenn der Buchstabe geht, liegt das Problem am Betriebssystem/Software-Shortcuts, nicht an der Hardware oder QMK.

### 5. Hardware-Spezifikation

- **Board:** Sofle Rev1
- **Controller:** RP2040 (daher `-e CONVERT_TO=promicro_rp2040`)
- **Besonderheiten:** Individuelle OLED-Animation in Layer 4 (Gaming Mode) und Encoder-Layer-Wechsel.
