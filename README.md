# :fish: Fish Galore Ark Tool :fishing_pole_and_fish:
[Download Executable](https://github.com/Mechanically/Fish-Galore-Ark-Tool/releases/latest)

This tool automates the fishing aspect of the game by analysing the screen to identify which key is being required by the game and simulate the keypress.

It automatically modifies the Gamma value of the game engine to increase the contrast (makes identification easier), cycles between rods to increase the time which the tool can run autonomously, and when a fish is captured it saves a screenshot so you can check the catches later.



# :wrench: Configuration
On the game settings you need to change:

**Window Mode:** WindowedFullscreen

**UI General Scaling:** Move the slider all the way to the right side



# :computer: How to use
1- Run the program as Admin (right click on the executable -> Run as Admin)

2- Open the game, connect to your server, sit on a place to start fishing (Pelagornis, Raft with Chair, or just a chair on the shoreline).

3- On your inventory, put your bait one every fishing rod you have, then put the rods on the hotbar (1~9).

4- Using the first fishing rod on the hotbar, cast the line on the water and press the F2 key to start the fishing script.

5- If you are using more than one rod you can press the F3 key to enable auto switching (makes the rods last longer by switching everytime it catches a fish), then adjust the last fishing rod on the hotbar pressing F6 and the first fishing rod on the hotbar pressing F4.

6- To stop fishing just press F2 again.



# :tv: Compatible Resolutions
16:9 aspect ratio:
- [x] 1920x1080
- [x] 1366x768

16:10 aspect ratio:
- [x] 1680x1050

You don't see your resolution on this list? Try it anyway... the program tries to interpolate to unknown resolutions.

If it doesn't work please take screenshots of every letter (A, C, D, E, Q, S, W, X and Z) and send to me on an Issue so I can add it to the script.



# :poop: Is this safe to Download?
If you trust me you can [download the executable](https://github.com/Mechanically/Fish-Galore-Ark-Tool/releases/latest) and run without any hastle.

But to be fair you should never really trust unknown programs you download from the internet.

That's why you may want to peek the code to check if there is something suspicious, and after that you can run the script following this steps:

1. Download the tool Autohotkey on [autohotkey.com](https://www.autohotkey.com/)
2. Download this script from [https://github.com/Mechanically/Fish-Galore-Ark-Tool](https://github.com/Mechanically/Fish-Galore-Ark-Tool)
3. Extract the zip file on a folder (anywhere you can remember later)
4. On the folder find the file "Fish Galore Ark Tool - v1.0.ahk", press right click on it and click on "Compile Script"
5. Wait a few seconds and a new executable file will appear on the folder. Right click on it and Run as Admin.
6. Enjoy your game :)



# :bomb: It is not working, what should I do?
If the script isn't working or has a bug please let me know what happened by opening an Issue.



# :clipboard: Methodology to find the letters

To find the letter unique positions I took screenshots of every letter the game asks, imported them on Krita (opensource image editing software), then colored and cut each letter to a new layer.

After that I overlaped all the letters and cut the intersection between them. The few parts that remained where the unique positions of each letter.

But 3 of the letters (S, E and C) were totally overlaped (no unique positions). I did the same procedure above, but now with only these 3 letters to have the unique positions between them.

So the script first tries to get the easy letters, and if one was not found it iterates between the hard letters comparing against the easy letters.



# :scroll: Credits to 

  - Spencer J Potts
  
    Contribution:
  
      Methodology for detecting letters and Catch message;
    
      Points for the resolution 1920x1080;
    
    GitHub: https://github.com/SpencerJPotts

  - Linear Spoon
  
    Contribution:
  
      CaptureScreen() Script, used to save screenshots;
    
    GitHub: https://github.com/LinearSpoon/
  
