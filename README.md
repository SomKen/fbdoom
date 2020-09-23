# Doom for Linux Frambuffer - Unifi (ish)
"Fixed" fbdoom to launch successfully on a UniFi Cloud Key Gen2 Plus. Some may ask why, but I ask why not?

The LCD screen is far too small to be able to see anything inside doom. Playing around with resolution values I was unable to get the screen to be legible, but this is more for fun than anything else.

In order to get this "running." you first need to SSH into your cloudkey and run "killall ck-ui" to all for use of /dev/fb0 without the controller updating the screen on its own.

Video: https://www.youtube.com/watch?v=iEap5nSBxus

---
This port of the original Doom source code targets Linux Framebuffer, without any intermediate abstraction layer (like SDL).

There is no keyboard input, sound or music - you can only watch the demo screen running in the framebuffer. Further, no scaling is implemented - resolution is the original Doom screen resolution.

This port depends only on *stdlib*.
