#!/bin/bash

mute=$(amixer get Master | awk  '/'Front' 'Left:' 'Playback'/  {print $6}')

if [ "$mute" = "[off]" ]
	then amixer set Master unmute
else
	amixer set Master mute
fi
exit 0
