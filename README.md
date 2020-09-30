# AshitaProfiles Thanks to other coder's for let me see their work. Haven't program in years
After looking at several other coder's I wrote a few as I need to use Ashitacast gearswap.
If your on Retail Server Please Read Ashitacast Doc's because there is a command to search all
your Inventory which can get you Banned!!! I don't use it! I just use Warerobe only to store my
Gear. Its search all the Warerobe to swap it in and doesn't matter where its stored in your
Warerobe unless you didnt pay for Warerobe 3 or 4. 
--------------------------------------------------------------------------------------------------------------
Chapter 1:----Setup Ashitacast and XML files.----
-------------------------------------------------
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
--------------------------------------------------------------------------------------------------------------
Chapter 2:----Setup Summoner with Siphon----
--------------------------------------------
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
			(Create a folder called siphon in Scripts folder called siphon) to put the files called 
						
					
					dark.txt earth.txt fire.txt ice.txt light.txt thunder.txt 
					water.txt wind.txt. 
					
  Example wind.txt in (Ashita folder - Scripts folder - siphon folder) to put the file wind.txt:
					
					/ma "Air Spirit" <me>
					/wait 6
					/ja "Elemental Siphon" <me>
					/wait 2
					/pet "Release" <me>

I've Coded more and am going change this XML more since I learned alot more about Ashitacast.
Alot of my XML use /exec command and putting .txt files in script folder. 
/exec commands are the same as using In-Game Macro without the limit of six spaces.
The commands can be add as Macro's or on the command line like /siphon used in Summoner XML.

--------------------------------------------------------------------------------------------------------------
Chapter 3:----Setup start .txt to add what addons wish to use for that Job----
------------------------------------------------------------------------------
smn.txt thf.txt dnc.txt go in (Ashita folder - Script folder) and are called by the XML.
I unload all the Addons and load the addons by Job. Such as PetInfo addon which needs
to installed in the (Ashita Folder - Addons Folder) to work. All addons can be installed
via Ashita by the addons button. These are what I use from the basic setup of Ashita.
--------------------------------------------------------------------------------------------------------------
Chapter 4:----Setup Lock Style and going your Macro Set and Page by Subjob
--------------------------------------------------------------------------
I've commented this section out because your Macro setup is different then mine.
But if you like to use it then you need to uncomment and setup the Lock Style, Macrobook, and Macropage.

p_mainjob	checks the Mainjob is correct and goes to macrobook 11 for my Dancer. Next change 11 to your Macrobook
		you use for the Mainjob.

p_subjob	checks to see what subjob you used and goes to the Macropage under
		Mainjob Macrobook. Mine is Macrobook 11 for Dancer and the page is 2 for NIN 
		and 3 for THF.
		
		
Macrobook 	is the 11 book I use for my Dancer macro's (Lots to use when it comes to Macrobook).

Macropage	is the page to use. If I sub NIN it goes page 2 and if I sub THF then page 3
		You can add more pages for subjobs by coping <elseif> - </elseif> and changing
		the THF to other Subjobs and using Pages 2-10 if need you change it from NIN and THF.
		NIN THF WAR BLU which are the 3 characters needed to be used in statement p_subjob="THF".
		All the Subjobs have a 3 character code which can be used.
		Macropage is Page usable in the Macrobook 11 or what Macrobook you use and Macropage can
		be 1-10.

lockstyleset    Is under "Edit Equip SET" pages 1-100 to Lock your Style from Blinking when changing Gear.
		I have 99 as my causal gear and 100 my lvl 1 crafting. You can lock to any of 1-100 set
		by changing 99	<setvar name="lock" value="99" /> to any of your sets from 1-100.
		

If this doesn't work for you replace the comments and use your old way of Lockstyle and change
to your Macrobooks.
		
			

