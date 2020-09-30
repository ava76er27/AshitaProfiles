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
But if you like to use it needs to be uncommented and setup to your Macro set.

Remove this line:	<!---
99 is Equipset to use:	<setvar name="lock" value="99" />
			
11 is Macro Book:	<if p_mainjob="DNC"><setvar name="macrobook" value="11" /></if>
			
Change NIN to yours:	<if     p_subjob="NIN">
Macro Set to use:	<setvar name="macropage" value="2" />
			</if>
Change THF to yours:	<elseif p_subjob="THF">
Macro Set to use:	<setvar name="macropage" value="3" />
			</elseif>
			<else>
Goto Macro set 1	<setvar name="macropage" value="1" />
If no matched SubJob	
			</else>

			<command delay="1500">/macro book $macrobook</command>
			<command delay="3000">/macro set $macropage</command>
			<command delay='6000'>/lockstyleset $lock</command>
Remove this line:	--->

p_mainjob	checks the Main job is correct.
p_subjob	checks to see what sub job you used and goes to the page under
		main jobs macrobook.
Macrobook 	is the 11 book I use for my Dancer macro's
Macropage	is the page to use. If I sub NIN it goes page 2 and if I sub THF then page 3
		You can add more pages for subjobs by coping <elseif> - </elseif> and changing
		the THF to other Subjobs and using Pages 4-10 if needed.
		NIN THF WAR BLU which are the 3 characters Needed to change in p_subjob="THF"
		to making more Pages usable in the Macrobook.
		Copy and Paste this under the </elseif> of THF and change THF to WAR and "3" to "4"
		will go to Macrobook 11 and Macropage 4 etc...
		<elseif p_subjob="THF">
		<setvar name="macropage" value="3" />
		</elseif>
If this doesn't work for you replace the comments and use your old way of Lockstyle and change
to your Macrobooks.
		
			

