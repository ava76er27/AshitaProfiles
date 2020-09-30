# AshitaProfiles Thanks to other coder's for let me see their work. Haven't program in years
After looking at several other coder's I wrote a few as I need to use Ashitacast gearswap.
If your on Retail Server Please Read Ashitacast Doc's because there is a command to search all
your Inventory which can get you Banned!!! I don't use it! Just use Warerobe only to store your
Gear. Its search all the Warerobe to swap it in and doesn't matter where its stored in your
Warerobe unless you didnt pay for Warerobe 3 or 4. 

Start Ashita add Plug-in Ashitacast (May need to restart Ashita so 
it can create the Folder after installing it)
If you look in the (Ashita Folder - Config folder - Ashitacast folder).
Store the YourName_SMN.xml in there and Change YourName in YourName_SMN.xml
to your Character's Name. Example: Your Character Name is Ralphm.

Ralphm_SMN.xml will load automatically when you change to Summoner
or Login as Summoner. If you delete a < or > when adding your gear
then it might say Parse Error. Look up Ashitacast commands:
Please Read Ashitacast Doc's
/ac load
/ac unload
/ac debug
to test your changes to xml file.

SMN PUP SCH Profiles...
Summoner was my starting XML with thanks to all the Other Coder's help. This was a mix of 2 other people xml.
If you don't have my gear it's ok.

Prep set which is my Refresh gear. 
PrePact set with avatar favor lower's my Blood Pact time. Am at 20 seconds.
avMaB and avMaBMerit I use my Pet Magic Attack Bonus gear with Magic Attack Bonus Staff.
avAtk set is Pet Attack gear with a different staff not to be confused with a Magic Attack Bonus Staff.
This work for me and am not you and if you have opinion your absolutely right.

I Added Siphon Routine that picks the Right Day for max Siphon. 
How to setup this up is in XML file with more details.
			Ashita looks in the (Ashita Folder - Scripts folder - siphon folder)
			(Create a folder called siphon in Scripts folder called siphon) for the files called 
						
					
					dark.txt earth.txt fire.txt ice.txt light.txt thunder.txt 
					water.txt wind.txt. 
					
  Example wind.txt in (Ashita folder - Scripts folder - siphon folder) for the file wind.txt:
					
					/ma "Air Spirit" <me>
					/wait 6
					/ja "Elemental Siphon" <me>
					/wait 2
					/pet "Release" <me>

I've Coded more and am going change this XML more since I learned alot more about Ashitacast.
Alot of my XML use /exec command and the script folder with txt's files to use. /exec files
are the same as using In-Game Macro without the limit of six spaces.

smn.txt thf.txt dnc.txt go in (Ashita folder - Script folder) and are called by the XML.
I unload all the Addons and load the addons by Job. Such as PetInfo addon which needs
to installed in the (Ashita Folder - Addons Folder) to work. All addons can be installed
via Ashita by the addons button. These are what I use from the basic setup of Ashita.
