
Update: (6/9/2026)

I've made another version of the schematic called KH910_Power_Board_Formatted, as when I was sharing the schematic with others and tried to troubleshoot using it, we had trouble understanding the long traces/wires I had on the original.

I'm still keeping the original version here, since it is a closer representation to how the actual board traces and components are positioned and connected, but for troubleshooting and seeing the actual relationship between components, the new formatted version should be much more useful.

I also fixed an issue where I accidently labeled two pin sets the same "P8" name, so I fixed that.

There are some issues with trying to simulate it, as some of the transistors I used in the schematic don't have simulation profiles, so I'm going to have to figure out how to fix that soon, but it shouldn't be too bad.

I added some KiCanvas links in the description section to make it easier to view the schematics.

This has been a very insightful experience into how to use KiCAD, as this is my first "full" project using the program to make schematics. To anyone following this, I appreciate any help and patience, since this is very much a learning experience for me.




Title: 

Brother KH-910 Knitting Machine 5-15v Power Board


Description: 

This is a personal project of mine, as I am currently trying to troubleshoot my Brother KH-910 Knitting Machine with difficulty. 
After much research and troubleshooting, I have narrowed the issue down to something being wrong with the 5-15v internal power board
within my machine.

I have been trying to troubleshoot the board itself, and test the individual components individually, however that has proved to be
difficult. Partially due to my testing equipment being hobby grade at best, but mostly because the documentation about this board, specifically 
regarding the knitting machine's internal circuit boards, are essentially non-existent (if they even existed at all or were released to the public).

Hence I have taken it upon myself to fully recreate the board using KiCAD.


KiCanvas link for KH910_Power_Board: https://kicanvas.org/?repo=https%3A%2F%2Fgithub.com%2Fa-cl-zick%2FBrother-KH910-Knitting-Machine-Power-Board%2Fblob%2Fmain%2FKH910_Power_Board%2FKH910_Power_Board.kicad_sch

KiCanvas link for KH_Power_Board_Formatted: https://kicanvas.org/?repo=https%3A%2F%2Fgithub.com%2Fa-cl-zick%2FBrother-KH910-Knitting-Machine-Power-Board%2Fblob%2Fmain%2FKH910_Power_Board_Formatted%2FKH910_Power_Board_Formatted.kicad_sch


This recreated board uses the same circuit structure as the original board, but replaces some outdated components with modern equivilants.
I chose to go down this path as many of the transistors used on this board aren't in production any more and don't have great datasheets.
Using modern components also worked better with KiCAD, which was nice.

I included the datasheets and pinout images that I used under \Component-Schematics-And-Pinouts\ to save anyone forking or referencing the schematic for troubleshooting some time.

If troubleshooting the physical board with this, be careful about understanding the pinout of whatever component you're probing.
For instance, the original B772 transistor's symbol pinout has the collector with the arrow indicator, while with the new BD442 transistor, 
the symbol pinout has the emitter with the arrow indicator.
That was something that tripped me up when I was designing it, so just be vigilant.


Usage:

Currently this project only contains the schematic design, and doesn't include a PCB design.
This does allow for easier visual troubleshooting, along with KiCAD's simulation feature, which is the extent of what I plan on using.

Depending on what I find regarding my troubleshooting journey, as well as how many people request it, I might do the PCB design along with it.
Also I chose the GNU GPLv3 so anyone can fork off of it and do it themselves if they feel so inclined.


Conclusion / Final Thoughts:

I might revise this schematic further depending on feedback and my experience using it. 
It is highly likely that the current revision, revision 0, has some missing connections. I'll fix it as I go.
Also I can include pictures of the actual board itself for reference to those who don't have the power board itself, or don't want to dig too deep 
into their knitting machine quite yet.

This is my first large-ish project using KiCAD, so any helpful tips or advice on how to improve my schematic-ing skills is always appreaciated.

Thank you for reading this, and I hope this is helpful! :)


