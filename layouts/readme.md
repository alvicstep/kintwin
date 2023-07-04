## Custom Layout
Contoured Kinesis keyboards belong to a relatively small group of keyboards that utilize thumb clusters. The keycap profiles of thumb cluster keys make it easy to press multiple keys simultaneously by a thumb finger. Co-locating CTRL, SHIFT and KEYPAD modifiers in the thumb cluster gives truly unique capabilities to these keyboards.

### Software Developer Layout
The **soft_dev** layout is optimized for software development on a Windows machine. It is a result of many years of daily usage, keeping what works and removing what does not. 
Even if it might not be exactly what you are looking for, some of the ideas described below could be useful when designing a new layout.

#### Layout Features
- 3 layers: default layer, keypad layer, numpad layer
- keypad layer allows for 2 finger operation (using the same hand) using **arrow** keys together with
    - **CTRL** and/or **SHIFT** modifiers OR
    - **HOME/END** keys OR
    - **PAGEUP/PAGEDOWN** keys.  
- two finger operations can be achieved by holding up to 3 modifier keys (KEYPAD/SHIFT/CTRL) with a thumb finger and using index/middle/ring finger by pressing keywell keys. For example, you can fully control caret position and text selection of:  
    - each letter
    - each word
    - from a current caret position to the beginning of the line
    - from a current caret position to the end of the line
    - multiple lines
    - multiple pages
- executing  key combinations in a sequence can also be very beneficial. For example, executing "KEYPAD + O" and then "KEYPAD + SHIFT + U" selects the whole line of text in any text editor.
- keypad layer allows accessing the following keys by moving one finger away from the home row 
    - function keys (F1-F12)
    - **ESC** key
    - **CAPSLOCK** key
- **KEYPAD** key is a "momentary" modifier key which is used to switch to the keypad layer while the key is being pressed. There are 2 KEYPAD keys which are ENTER/DELETE keys on Kinesis thumb cluster keyboards
- **KEYPAD** key can also be used to access US ANSI Shifted Symbols instead of pressing a SHIFT key
- **NUMPAD** "momentary" modifier key can be used to quickly switch to a numpad while typing alphanumeric strings

#### Layout Layers

<img src="https://i.imgur.com/86LCI3zh.jpg"> 
<img src="https://i.imgur.com/Gv4WBw7h.jpg"/> 
<img src="https://i.imgur.com/gKXMUI2h.jpg"/> 

#### Notes
- MO(1) - switch to **KEYPAD** layer while key is being pressed
- MO(2) - switch to **NUMPAD** layer while key is being pressed
- TO(0) - switch to base layer 
- TO(2) - switch to **NUMPAD** layer 
- Rsft(Enter) - acts as an Enter key when pressed and released. Acts as a shift modifier in combination with other keys
- Bt - enter bootloader mode
- Alt(Tab) - toggle between last two active applications
- Ctrl(Tab) - toggle between last two active tabs


### Shortcuts


|Shortcut             | Control Caret                         |
|---------------------|---------------------------------------|
|`KEYPAD + J`         | move caret one character left         | 
|`KEYPAD + L`         | move caret one character right        | 
|`KEYPAD + I`         | move caret one line up                | 
|`KEYPAD + K`         | move caret one line down              | 
|`KEYPAD + CTRL + J`  | move caret one word to the left       | 
|`KEYPAD + CTRL + L`  | move caret one word to the right      | 
|`KEYPAD + U`         | move caret to the start of the line   | 
|`KEYPAD + O`         | move caret to the end of the line     | 
|`KEYPAD + H`         | move caret one page up                | 
|`KEYPAD + N`         | move caret one page down              | 


|Shortcut             | Scroll Lock                           |
|---------------------|---------------------------------------|
|`KEYPAD + CTRL + I`  | scroll page up                        | 
|`KEYPAD + CTRL + K`  | scroll page down                      | 


|Shortcut                     | Select Text                   |
|-----------------------------|-------------------------------|
|`KEYPAD + CTRL + SHIFT + J`  | select one word to the left   | 
|`KEYPAD + CTRL + SHIFT + L`  | select one word to the right  | 
|`KEYPAD + CTRL + SHIFT + I`  | select one line up            | 
|`KEYPAD + CTRL + SHIFT + K`  | select one line down          | 
|`KEYPAD + SHIFT + H`         | select one page up            | 
|`KEYPAD + SHIFT + N`         | select one page down          | 
|`KEYPAD + CTRL + SHIFT + U`  | select from beginning of the file up to the caret position   | 
|`KEYPAD + CTRL + SHIFT + O`  | select from caret position to the end of the file  | 


|Shortcut             | US ANSI Shifted Symbols               |
|---------------------|---------------------------------------|
|`KEYPAD + -`         | _                                     | 
|`KEYPAD + 1`         | !                                     | 
|`KEYPAD + 2`         | @                                     | 
|`KEYPAD + 3`         | #                                     | 
|`KEYPAD + 4`         | $                                     | 
|`KEYPAD + 5`         | %                                     | 
|`KEYPAD + 6`         | ^                                     | 
|`KEYPAD + 7`         | &                                     | 
|`KEYPAD + 8`         | *                                     | 
|`KEYPAD + 9`         | (                                     | 
|`KEYPAD + 0`         | )                                     | 
|`KEYPAD + =`         | +                                     | 
|`KEYPAD + \`         | \|                                    | 
|`KEYPAD + '`         | "                                     | 
|`KEYPAD + ;`         | :                                     | 
|`KEYPAD + /`         | ?                                     | 
|`KEYPAD + [`         | {                                     | 
|`KEYPAD + ]`         | }                                     | 
|`KEYPAD + ,`         | <                                     | 
|`KEYPAD + .`         | >                                     | 
|`KEYPAD + BACKTICK`  | ~                                     | 