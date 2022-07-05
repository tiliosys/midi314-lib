
midi@3:14 is a home-made electronic keyboard for playing music.

This repository contains a Rust crate that allows a host computer to communicate
with midi@3:14 through its MIDI interface.

See [midi314-pcb](https://github.com/tiliosys/midi314-pcb) and
[midi314-firmware](https://github.com/tiliosys/midi314-firmware)
for more information about the keyboard itself.

MIDI events
-----------

This library supports the following custom MIDI Control-Change events:

| Identifier | Event                  |
|:-----------|:-----------------------|
| 20         | Start recording a loop |
| 21         | Play a loop            |
| 22         | Mute a loop            |
| 23         | Delete a loop          |
| 24         | Mute all other loops   |
| 25         | Unmute all muted loops |
| 26         | Set min pitch          |
| 27         | Set min program        |
| 28         | Toggle percussion mode |
