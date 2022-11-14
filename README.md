# ero.overlays

Overlays included in this repo are for use with OBS as Custom Browser sources and Custom Docks.  Everything in here is used by erodozer on twitch.tv

## controls.html

This is the central listener hub for the overlays.  It consumes messages from Twitch IRC using tmi.js, and adapts them to generic events to be published over localstorage.

This should be mounted to your OBS interface as a Custom Dock to always be running regardless of active scene.

## chat.html

A basic chatbox.  Chat messages are scrubbed by controls.html, so this just listens to simple events and renders them.

## clock.html

Renders your system time on stream so people can know how late it is for you.

## quickchat.html

Put emphasis on your own messages when talking to twitch chat while muted.  You can either talk directly to this using controls.html or it can intercept messages from twitch IRC made by the broadcaster.

Cutely animated to sound like the king of all cosmos, but it's easy to swap out fonts and the talking sound effect.
