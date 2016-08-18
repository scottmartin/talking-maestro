# talking-maestro

I'm visually impaired, and I've had several issues ever since Apple changed the way their text to speech works somewhere around OS X Lion. I'm not completely blind, so all I really need is the "Speak selected text when key is pressed" feature in the "Dictation" part of system preferences. Before their change it used to just copy the selected text and read it off of the clipboard. Since the change, it now uses an OS level API that developers have to actively support if they're doing anything out of the ordinary with their text views. Because of this change I still run in to applications that just no longer allow me to use text to speech at all.

## Usage

Hit your key combo once and it will read what you have selected. Hit it again while it's reading and it will stop. I had to add the `textutil` call in the shell script because `say` apparently doesn't like when it can't tell if text is UTF8, and I was having issues when certain webpages used curly quotes and other non-ASCII characters.

## Install

Just download and double-click the macro file from this repository. It will automatically add it to your keyboard Maestro library.
