---
title: 'New release of Costa - version 1.5.0'
img: costa_featured6.png
layout: post
categories:
  - Costa
---
Just in time before the new year, Costa version 1.5.0 has finished testing and has been released. This version comes with many improvements and changes, but three stand out from the rest: A new UI design based on [Costa 0.9.4](https://costa.jacobpalm.dk/archive.html#version094), massive speed improvements to handling of data files, and full keyboard support in all accessories. Code optimizations have also helped reduced the combined size of Costas executables significantly.

To give Costa its own unique look, and separate it from the countless Windows clones out there, the [UI](https://en.wikipedia.org/wiki/Graphical_user_interface) I designed myself for Costa 0.9.4 has been brought back to life, with some improvements. In Costa 0.9.4, the colors of the UI were predefined and could not be customized, but now, everything can be customized. Every one of the 27 themes that comes with Costa have been adaped to work with the new UI. Fun fact: The basis of this new UI was initially designed by me using [Microsoft Paint](https://en.wikipedia.org/wiki/Microsoft_Paint) 14 years ago!\
Personally, I think the new UI looks great, and gives Costa a bit more of a retro look.

Previously, users have been required to use a mouse to edit icons and themes, since there was no way to select colors using the keyboard, and in the icon editor there was no way to draw individual pixels using the keyboard alone. Now, colors can be cycled using the keyboard in both accessories, and in the icon editor pixels can be selected using the arrow keys, and painted with the Space or Enter keys.

Massive speed improvements have been made to all file and disk related operations. This work started when I acquired an old [IBM PS/2](https://en.wikipedia.org/wiki/IBM_PS/2) computer, with a 16 MHz [386 CPU](https://en.wikipedia.org/wiki/I386) and a slow hard drive. I quickly saw that Costa was barely usable, due to the slow disk speeds. This was not something I had previously seen, as I've previously been testing Costa only on [486](https://en.wikipedia.org/wiki/I486) hardware. So, work began to replace all file formats used by Costa with binary formats, which can be read from and written to disk vastly faster than the old formats.\
At the same time, I've added to option in Costas configuration to disable disk caching of the desktop. Disabling this results in more screen redraws, which on faster machines will result in a bit of flicker, but on old machines with a slow disk, the speed increase is instantly noticeable. So, I figured that having an option for this would allow Costa to run as best it could on both types of machines.\
Lastly, all settings are now cached in memory, instead of being read from disk every time they were used.

![The Costa GUI version 1.5.0]({{site.url}}/assets/img/150.png)

More information and download links can be found at <https://costa.jacobpalm.dk>.

For those who are interested in development, [visit GitHub](https://github.com/jacobpalm/costa) to have a look at the source code.