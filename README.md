# murti-cec-remote
A modification of Pulse-Eight cec-client that allows for single character input to control multiple devices over HDMI-CEC (WARNING this will break the cec-client command if you have it installed)

##How to install

####Go to this directory

cd murti-cec-client

####Make the install script executable

chmod a+rx install.sh

#####examine and edit the layout file (optional)

nano layout.h

####Run the install script

./install.sh


##How to use

-At any time run the "cec-client" command in a shell

-After waiting, you will eventually see a list of options with text such as:

device #4: Playback 1
address:       2.5.0.0
active source: no
vendor:        Sony
osd string:    PlayStation 4
CEC version:   1.3a
power status:  standby
language:      eng

When prompted "Which Device Number (or lowercase letter) would you like to control?:" type the corresponding device number of the device you wish to control. In this case pressing "4" will control the PS4.


## Default Layout

#####switch

  LISTDEVICE "I"
  CHANGEDEVICE "i"

#####power

  POWERON "p"
  STANDBY "P"

#####navigation

  RIGHT "d"
  LEFT "a"
  UP "w"
  DOWN "s"
  SELECT "x" //x on ps4
  EXIT "b" //circle on ps4
  CLEAR "j"

#####playback

  PLAY "g" //play is g for go!
  REWIND "r"
  RECORD "R"
  FASTFORWARD "f"
  STOP "S"

#####other

  ROOTMENU "h" //home ps button ps4
  SETUPMENU "o" //option button ps4
  EJECT "E" //eject ps4 too
