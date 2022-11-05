# Typer-Mode #
Provides a program to practise your keyboard typing. It provides a
buffer with text that need be typed. As the user starts typing the
correct characters, they get removed from the buffer. If the user
types the wrong character a new line of text is added. This goes on
until the user types all characters correct which results in "Game
Won". If the user makes to many succesive errors then it’s "Game
Over".

## Getting Started ##
You can clone this project and add it to the load-path
in your init-file:
```
(add-to-list 'load-path "~/.emacs.d/elisp/typer-mode")
(require 'typer-mode)
```
## How it works ##
You can start the game by typing: `M-x typer ENT`. This opens a buffer
with random sentences from a file provided by the custom variable
‘typer-mode-content’. You than type in the words you see until the
end. If you type a character wrong, than a new line is added. As soon
as you manage to type in all characters correctly until the end. You
win the game. If you make to many errors you will lose the game. You
can exit the game anytime you want by either switching buffer or
killing it. If you want restart the game, just type again ‘M-x typer
ENT’.
