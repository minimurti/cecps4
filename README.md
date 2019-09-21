# cecps4
linux scripts used to control ps4 with single keyboard inputs. 


The following three files are ran at startup on my Raspberry Pi to control my PS4 via cec commands, using noral keyboard input. "test" must be used as a startup script to run exactly when the devise is turned on. It will only work if it is run at startup. (Or if no other terminals have been opened.)


You will need the following utilities for it to work

Konsole:
sudo apt-get install konsole

ttyecho
https://github.com/osospeed/ttyecho


libcec
https://github.com/Pulse-Eight/libcec
