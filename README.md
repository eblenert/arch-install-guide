Arch Install Guide [WIP]
-
This guide is my personal to-do list when doing a new Arch installation.


* [TouchPad] Invert touchpad direction (aka natural direction)

	Make sure the *xf86-input-synaptocs* is installed.

	Open/create the file */etc/X11/xord.conf.d/70-synaptics.conf* and set/update the following settings:

	```
	Section "InputClass"
		Identifier		"touchpad"
		Driver			"synaptics"
		MatchIsTouchpad	"on"
		Option			"VertScrollDelta"		"-111"
		Option			"HorizScrollDelta"		"-111"
	EndSection
	```
