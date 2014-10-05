mp3jet
======

Audio printer backend for CUPS

Depending on your system you have to put your CUPS user to the "audio" group.
So that the backend is able to play your audio files.

This project is only for fun. If you have any ideas or patches just give me a
shout.

this is a very simple CUPS backend to play mp3 files
just print your mp3 file with lpr like so:
    $ lpr -H my_cups_ip -P mp3_queue_name greate_mp3.mp3

don't forget to share your printer in the network, so
that everyone can print mp3's.

to control the mp3 spooler just use the CUPS webinterface.
Everyone can take a look on the "playlist" and the admin
can cancle songs and is able to move songs in the playlist

TODO:
1. determine the mimetype of the incomming stream so we prevent some clowns
   from playing pdf's with mplayer ... or OCR this stream and use a text to
   speech engine to play the "song" ;)
2. make this thing more variable, a config file would be nice to set some
   variables like $PLAYER_STR and so on
3. i also thought about a simple plugininterface so that the printed file
   can be pre- or postprocessed, like copy those files to a public location
4. write a usefull installation how to
5. put this TODO in a seperate file ...
6. ... feel free to add points here
