# Sofle Rev1 Keymap Layout

## Layer 0: Base (Standard QWERTY)

Dies ist der Standard-Layer für das tägliche Tippen.

| Reihe      |  1   |  2  |  3  |     4     |  5   |   6    |     7     |    8     |     9     |  10  |  11  |  12  |
| :--------- | :--: | :-: | :-: | :-------: | :--: | :----: | :-------: | :------: | :-------: | :--: | :--: | :--: |
| **Oben**   | ESC  |  1  |  2  |     3     |  4   |   5    |     6     |    7     |     8     |  9   |  0   |  -   |
| **Mittig** | TAB  |  Q  |  W  |     E     |  R   |   T    |     Y     |    U     |     I     |  O   |  P   |  [   |
| **Unten**  | LSFT |  A  |  S  |     D     |  F   |   G    |     H     |    J     |     K     |  L   |  ;   |  '   |
| **Basis**  | LCTL |  Z  |  X  |     C     |  V   |   B    | **TO(4)** | **MUTE** |     N     |  M   |  ,   |  .   |
| **Thumb**  | LGUI | SPC | ENT | **MO(1)** | LALT | _none_ |  _none_   | **SPC**  | **MO(2)** | RSFT | RALT | RALT |

- **TO(4)**: Linker Encoder-Knopf (wechselt in Gaming Layer 4)
- **MUTE**: Rechter Encoder-Knopf

---

## Layer 1: Lower (Funktionstasten & Numblock)

Aktiviert durch Halten der Taste links neben der linken Leertaste (`MO(1)`).

| Reihe      |     1      |   2    |   3    |   4   |   5    |   6    |   7    |  8   |     9     | 10  |   11   |   12   |
| :--------- | :--------: | :----: | :----: | :---: | :----: | :----: | :----: | :--: | :-------: | :-: | :----: | :----: |
| **Oben**   | **Alt+F4** |   F1   |   F2   |  F3   |   F4   |   F5   |   F6   |  F7  |    F8     | F9  |  F10   |  F11   |
| **Mittig** |   _none_   | _none_ | C-BSPC |  UP   | C-DEL  | _none_ | _none_ |  7   |     8     |  9  | _none_ |  F12   |
| **Unten**  |   LCTL+Y   |  BSPC  |  LEFT  | DOWN  |  RGHT  |  DEL   | _none_ |  4   |     5     |  6  | _none_ | _none_ |
| **Basis**  |   _none_   | _none_ | C-Left | C-F10 | C-RGHT | _none_ |  TRNS  | TRNS |  _none_   |  1  |   2    |   3    |
| **Thumb**  |   _none_   | _none_ | _none_ | TRNS  |  TRNS  | _none_ | _none_ | TRNS | **MO(3)** |  0  | _none_ | _none_ |

---

## Layer 2: Raise (Sonderzeichen)

Aktiviert durch Halten der Taste rechts neben der rechten Leertaste (`MO(2)`).

| Reihe      |   1    |   2    |   3    |   4    |   5    |   6    |   7    |  8   |   9    |   10   |   11   |   12   |
| :--------- | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :--: | :----: | :----: | :----: | :----: |
| **Oben**   | _none_ |  AG-1  |  AG-2  |  AG-3  |  AG-4  |  AG-5  |  AG-6  | AG-7 |  AG-8  |  AG-9  | AG-F10 | AG-F11 |
| **Mittig** |  S-`   |  AG-Q  |  S-#   |  AG-E  | _none_ | _none_ | _none_ | AG-7 |  AG-8  |  AG-9  |  AG-0  | AG-F12 |
| **Unten**  |   `    |  S-1   |  S-2   |  S-3   |  S-4   |  S-5   |  S-6   | S-7  |  S-8   |  S-9   |  S-0   |   #    |
| **Basis**  | AG-<>  |   <>   |  S-<>  |   =    |  S-=   | _none_ |  TRNS  | TRNS | _none_ |  AG--  | _none_ |  S--   |
| **Thumb**  |  AG-]  | _none_ | _none_ | _none_ |  TRNS  |  TRNS  | _none_ | TRNS | _none_ | _none_ | _none_ | _none_ |

---

## Layer 3: Adjust (System & Reset)

Aktiviert durch **Gleichzeitiges Halten von Layer 1 und Layer 2**.

| Reihe     |     1      |   2    |   3    |   4    |   5    |   6    |   7    |   8    |   9    |   10   |   11   |   12   |
| :-------- | :--------: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| **Oben**  | **EE_CLR** | _none_ | _none_ | _none_ | _none_ | _none_ | _none_ | _none_ | _none_ | _none_ | _none_ | _none_ |
| **Thumb** |   _none_   | _none_ | _none_ |  TRNS  |  TRNS  | _none_ | _none_ |  TRNS  | _none_ | _none_ | _none_ | _none_ |

- **EE_CLR**: Löscht den EEPROM-Speicher (Reset für VIA).

---

## Layer 4: Gaming (Gaming Mode)

Aktiviert über den Encoder-Druck (`TO(4)`). OLED zeigt ein X-Muster.

| Reihe      |  1   |  2   |  3  |  4  |  5  |  6   |     7     |     8     |  9   |  10  |  11  |  12  |
| :--------- | :--: | :--: | :-: | :-: | :-: | :--: | :-------: | :-------: | :--: | :--: | :--: | :--: |
| **Oben**   | ESC  |  1   |  2  |  3  |  4  |  5   |     6     |     7     |  8   |  9   |  0   |  -   |
| **Mittig** |  T   | TAB  |  Q  |  W  |  E  |  R   |     Z     |     U     |  I   |  O   |  P   |  ;   |
| **Unten**  |  G   | LSFT |  A  |  S  |  D  |  F   |     H     |     J     |  K   |  L   |  ;   |  '   |
| **Basis**  | LCTL | LCTL |  Y  |  X  |  C  |  V   | **TO(0)** |   TRNS    |  N   |  M   |  ,   |  .   |
| **Thumb**  |  -   |  =   | F16 | F17 |  B  | LALT |    SPC    | **TO(0)** | TRNS | TRNS | TRNS | TRNS |

- **TO(0)**: Zurück zum Basis-Layer.
