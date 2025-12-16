# Configuración ZMK - Corne 36 teclas (usando shield de 42)

**IMPORTANTE:** Físicamente tienes 36 teclas, pero usamos el shield de 42 teclas del Corne estándar.
Las columnas externas están marcadas como `&none` porque no existen físicamente.

## **Capa 0: Base**
```
NONE  Q  W  E  R  T        Y  U  I  O  P  NONE
NONE  A  S  D  F  G        H  J  K  L  ;  NONE
NONE  Z  X  C  V  B        N  M  ,  .  /  NONE
         _  1  SPC         ENT  2  _
```
**Home row mods:**
- A=GUI, S=ALT, D=SHIFT, F=CTRL (izq)
- J=CTRL, K=SHIFT, L=ALT, ;=GUI (der)

**Pulgares:**
- 1 = Capa Numpad (hold)
- 2 = Capa Edit (hold)
- ENT = Enter (tap) / Capa Nav (hold)

---

## **Capa 1: Numpad**
```
NONE  BT1  BT2  BT3  BT4  BT5        _  7  8  9  _  NONE
NONE  _    _    _    _    _          _  4  5  6  _  NONE
NONE  BTCLR _   _    _    _          0  1  2  3  _  NONE
```

---

## **Capa 2: Edit**
```
NONE  _  _  _  _  _        _     _  _  _    _  NONE
NONE  _  _  _  _  _        BSPC  _  _  DEL  _  NONE
NONE  _  _  _  _  _        _     _  _  _    _  NONE
```

---

## **Capa 3: Nav** (hold Enter)
```
NONE  _  _  _  _  _        _  _  _  _  _  NONE
NONE  _  _  _  _  _        ←  ↓  ↑  →  _  NONE
NONE  _  _  _  _  _        _  _  _  _  _  NONE
```

---

## Combos

**Combos básicos:**
- **J + K** = ESC
- **C + V** = =
- **M + ,** = -
- **, + .** = '
- **M + , + .** = `
- **, + . + /** = \

**D + F + número** = símbolo correspondiente:
- **D + F + M** (1) = !
- **D + F + ,** (2) = @
- **D + F + .** (3) = #
- **D + F + J** (4) = $
- **D + F + K** (5) = %
- **D + F + L** (6) = ^
- **D + F + U** (7) = &
- **D + F + I** (8) = *

## Notas
- `NONE` = tecla que no existe físicamente (columnas externas)
- `_` = transparente/vacío
- BT1-5 = perfiles Bluetooth (cambiar dispositivo)
- BTCLR = borrar todos los perfiles BT
- Home row mods: tap=letra, hold=modificador (280ms)
- Combos: timeout 50ms
