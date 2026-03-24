# HP-ProBook-and-EliteBook-Boot-Logos

FOR THIS EXAMPLE I'LL USE MY 6560b

This is to be used in combination with the sp58176.exe from HP to add a custom boot logo for your laptop. Like me, you may have a older HP laptop and are looking to make it more modern or just want to add a but of pizazz to your boot sequence. I've got you Ill also walk you through the setup. 

First, you'll want the sp58176.exe. You can get that here: http://ftp.hp.com/pub/softpaq/sp58001-58500/sp58176.exe 

Once downloaded and through the installation on the 6560b (or whatever laptop you've got), navigate to: C:\SWSetup\SP58176

Now that you are in the SP58176 folder, you should see a file named "ereplogo.exe"  Don't touch it yet, but keep this folder open

Download Rufus if you don't already have it. You can get that here: https://github.com/pbatard/rufus/releases/download/v4.13/rufus-4.13.exe  

Now, open Rufus and insert a flash drive (Mine was 512MB, so it really doesn't matter). Now, under the box thing that says "Disk or ISO image (Please select)", pick FreeDOS

Check the options below by settings and whatnot, set it to MBR for partition scheme, and that should make it be BIOS. I actually don't know if it matters, but just trust.

Flash that by pressing the start button below.

Once it's finished flashing, open that folder for the "ereplogo.exe" thing again, and just copy that to the FreeDOS flashdrive.

YAY, the hard part is done, now it's up to your creativity.

Make an image, it can be literally anything, over a 1024x768 canvas, yes, 4:3 aspect ratio. Here is my current boot thing you can use: https://www.canva.com/design/DAHE0bj6p6I/MBCEsj5_YH-SFHVUz8mpHQ/edit?utm_content=DAHE0bj6p6I&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

I will also include more logos in the releases tab. NAME YOUR IMAGE "bootlogo" and be sure it's a JPG, otherwise it won't work, I think. Well, you can name it whatever, but later in the tutorial, you'll need to swap out the bootlogo for whatever you named yours.

Now that you have your image picked out, restart your computer and spam your boot devices button. I belive its F9 for HP

Select your USB and click any button to boot from USB

Type "EREPLOGO /fbootlogo.jpg" if you picked a different name, it will be "EREPLOGO /fXXXXXXX.jpg" those X's being the name of the image.

Press enter, and it should work, if not, umm, god help you. NOTE: I'm not god.

Done, Reboot and hope for the best on startup
