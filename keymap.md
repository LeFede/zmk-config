# Configuración ZMK - Corne 36 teclas (usando shield de 42)

**IMPORTANTE:** Físicamente tienes 36 teclas, pero usamos el shield de 42 teclas del Corne estándar.
Las columnas externas están marcadas como `&none` porque no existen físicamente.

## **Capa 0: Base**
```
NONE  Q  W  E  R  T        Y  U  I  O  P  NONE
NONE  A  S  D  F  G        H  J  K  L  ;  NONE
NONE  Z  X  C  V  B        N  M  ,  .  /  NONE
         _  1  SPC         ENT  BSPC  DEL
```
**Home row mods:**
- A=GUI, S=ALT, D=SHIFT, F=CTRL (izq)
- J=CTRL, K=SHIFT, L=ALT, ;=GUI (der)

**Pulgares:**
- 1 = Capa Numpad (hold)
- ENT = Enter (tap) / Capa Nav (hold)
- BSPC = Backspace (tap) / Capa Edit (hold)
- DEL = Delete

---

## **Capa 1: Numpad**
```
NONE  BT1  BT2  BT3  BT4  BT5        _  7  8  9  _  NONE
NONE  _    _    _    _    _          _  4  5  6  _  NONE
NONE  BTCLR _   _    _    _          0  1  2  3  _  NONE
```

---

## **Capa 2: Edit** (vacía - reservada para futuros usos)
```
NONE  _  _  _  _  _        _  _  _  _  _  NONE
NONE  _  _  _  _  _        _  _  _  _  _  NONE
NONE  _  _  _  _  _        _  _  _  _  _  NONE
```
*Nota: Backspace y Delete ahora están en los pulgares*

---

## **Capa 3: Nav** (hold Enter)
```
NONE  _  _  _  _  _        _  _  _  _  _  NONE
NONE  _  _  _  _  _        ←  ↓  ↑  →  _  NONE
NONE  _  _  _  _  _        _  _  _  _  _  NONE
```

---

## **Capa 4: WinNum** (hold G)
```
NONE  W+S+Q  _  _  _  _          _    W+7  W+8  W+9  _  NONE
NONE  _      _  _  _  G(hold)    _    W+4  W+5  W+6  _  NONE
NONE  _      _  _  _  _          W+0  W+1  W+2  W+3  _  NONE
```
**Uso:**
- Hold G + tap M = Win+1
- Hold G + hold M = Win+Shift+1
- Hold G + Q = Win+Shift+Q (cerrar ventana en i3)
- Y así con todos los números en sus posiciones del numpad

---

## **Capa 5: Tmux** (hold T)
```
NONE  _  _      C-SPC [  _  T(hold)    _  _          _          _         _      NONE
NONE  _  C-SPC S  _  _  _              _  _          C-SPC %    C-SPC "   C-SPC; NONE
NONE  Z  _      _  _  _                _  _          C-SPC ,    C-SPC .   _      NONE
```
**Uso (todos ejecutan Ctrl+Space + comando con 1ms de espera):**
- Hold T + E = Ctrl+Space → [ (copy mode / navegación)
- Hold T + Z = Ctrl+Space → Z (zoom pane)
- Hold T + S = Ctrl+Space → S (session list)
- Hold T + K = Ctrl+Space → % (split horizontal)
- Hold T + L = Ctrl+Space → " (split vertical)
- Hold T + ; = Ctrl+Space → ; (último pane)
- Hold T + , = Ctrl+Space → , (renombrar window)
- Hold T + . = Ctrl+Space → . (mover window)

---

## **Capa 6: Tmux Windows** (hold W)
```
NONE  _  W(hold)  _  _  _          _      Win7  Win8  Win9  WPrev  NONE
NONE  _  _        _  _  _          _      Win4  Win5  Win6  _      NONE
NONE  _  _        _  _  _          WNext  Win1  Win2  Win3  _      NONE
```
**Uso (Ctrl+Space → número/comando):**
- Hold W + M = Ctrl+Space → 1 (ir a window 1)
- Hold W + , = Ctrl+Space → 2 (ir a window 2)
- Hold W + números (1-9) = ir a esa window
- Hold W + N = Ctrl+Space → n (next window)
- Hold W + P = Ctrl+Space → p (previous window)

---

## **Capa 7: Tmux Panes** (hold Q)
```
NONE  Q(hold)  _  _  _  _          _      Pane7  Pane8  Pane9  PPrev  NONE
NONE  _        _  _  _  _          _      Pane4  Pane5  Pane6  _      NONE
NONE  _        _  _  _  _          PNext  Pane1  Pane2  Pane3  _      NONE
```
**Uso (Ctrl+Space → q → número/comando o Ctrl+Space → o/;):**
- Hold Q + M = Ctrl+Space → q → 1 (ir a pane 1)
- Hold Q + , = Ctrl+Space → q → 2 (ir a pane 2)
- Hold Q + números (1-9) = ir a ese pane
- Hold Q + N = Ctrl+Space → o (pane next)
- Hold Q + P = Ctrl+Space → ; (pane previous)

---

## Combos

**Combos básicos:**
- **J + K** = ESC
- **J + K + L** = TAB
- **C + V** = =
- **M + ,** = -
- **, + .** = '
- **M + , + .** = `
- **, + . + /** = \

**Combos de Tmux:**
- **W + N** (combo) = Crear nueva window (Ctrl+Space → C)
- **Hold W + N** (layer) = Window next (Ctrl+Space → n)
- **S + N** = Crear nueva session (Ctrl+Space → :new-session)
- **Q + BSPC** = Cerrar pane actual (Ctrl+Space → x → y)
- **W + BSPC** = Cerrar window actual (Ctrl+Space → & → y)

**D + F + número** = símbolo correspondiente:
- **D + F + M** (1) = !
- **D + F + ,** (2) = @
- **D + F + .** (3) = #
- **D + F + J** (4) = $
- **D + F + K** (5) = %
- **D + F + L** (6) = ^
- **D + F + U** (7) = &
- **D + F + I** (8) = *

**Combos M + , + home row** = paréntesis y corchetes:
- **M + , + A** = {
- **M + , + S** = }
- **M + , + D** = (
- **M + , + F** = )
- **M + , + E** = [
- **M + , + R** = ]

**Botón pulgar izquierdo + tecla** = teclas F:
- **Botón + M** = F1
- **Botón + ,** = F2
- **Botón + .** = F3
- **Botón + J** = F4
- **Botón + K** = F5
- **Botón + L** = F6
- **Botón + U** = F7
- **Botón + I** = F8
- **Botón + O** = F9
- **Botón + /** = F10
- **Botón + ;** = F11
- **Botón + P** = F12

## Notas
- `NONE` = tecla que no existe físicamente (columnas externas)
- `_` = transparente/vacío
- BT1-5 = perfiles Bluetooth (cambiar dispositivo)
- BTCLR = borrar todos los perfiles BT
- Home row mods: tap=letra, hold=modificador (300ms)
- Win num behaviors: tap=Win+Num, hold=Win+Shift+Num (200ms)
- Combos: timeout 50ms
