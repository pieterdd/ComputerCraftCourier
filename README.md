Description
-----------

This repository contains a collection of very experimental script files that make up the components of the resource courier system described [here](http://www.youtube.com/watch?v=fpNVGsnAMP8). It was developed for use with the ComputerCraft mod, which adds scripting capabilities to Minecraft.

Unfortunately my system has many major shortcomings, some of which are highlighted in the video I just linked to. I do not plan on investing any more time into it because developing for ComputerCraft is rather cumbersome and the practical use for this stuff, unlike with [AptNotifier](https://github.com/pieterdd/AptNotifier), is very limited. But it was a fun summer project nonetheless!


Documentation
-------------

Relevant API documentation for ComputerCraft is hosted on their wiki.

- [OS API](http://computercraft.info/wiki/index.php?title=OS_%28API%29)
- [Shell API](http://computercraft.info/wiki/index.php?title=Shell_%28API%29)
- [Turtle API](http://computercraft.info/wiki/index.php?title=Turtle_%28API%29)


How to install
--------------

1) Put these files on a ComputerCraft diskette (instructions available elsewhere)
2) Do the following for each component:
	a) Insert the disk.
	b) Run */disk/startup* to copy all files to the computer or turtle. You can use *update* as a shortcut for */disk/startup* from this point forward.
	c) Run *junction*, *endpoint*, *courier* or *outbox*, depending on the function the device fulfills.
	
Make sure that you change the hardcoded target computer ID in */endpoint* for the endpoint where your route starts to reflect the target endpoint you wish to send packages to. Search for the text *"PICKUP* to find it; the line should be marked with *TODO*. If you're in a good mood, you could replace this hardcoded constant with an automatic endpoint discovery system that lets the user choose the target endpoint dynamically.