# Introduction

Here's some instructions for getting ready for the SGB 2023 charity event for The Trevor Project!

# Get Ready For The Event

1. Set up OBS for the event. See "OBS Setup". You may have your own flourish, but we would like to try to have a generally consistent "look" for the event.
2. Make a Tiltify account (or login with Twitch) and request to be part of the team on Tiltify. It requires logging in with Twitch, and going to the SMMShowciety Team Page (https://tiltify.com/+smm-showciety/profile) to request an invite. There is a black "Join team +" button next to the "SMM Showciety on Tiltify" header at the top!
3. While NOT required we strongly recommend planning donation incentives. See "Donation Incentive Ideas".
4. Set up bot commands for the links to the charity, donation page, etc. (see "Bot Commands"). Optionally set up timers to periodically post the same messages automatically.
5. Optionally set up a panel on your Twitch channel to advertises the event and provides a link to the donation page.
	a. Click "Add Image" and upload "Donate Panel 2023.png"
	b. Paste "https://www.showciety.gives/" into the "Image Links To:" box.
	c. Click "Submit"
6. Get to know a little about the charity we're supporting so you can talk it up. See "Talking Points" if you need something to get the juices flowing, but you should try to know a few things that the talking points can refresh in your mind's eye.
7. Try to be around to help coordinate the switchovers. Check the schedule, check that the next streamer is live and ensure they're ready for the raid, then report to the active streamer that the target is ready for the switchover. If there are multiple people talk amongst yourselves to voluntell one of you to handle it so we don't have multiple people trying to do the same thing.
9. REALLY try to help with the switchovers. Things like streamers being late/offline/having technical difficulties at the last minute can happen, and it will be bad if the active streamer has to try to coordinate that themselves. If someone is truly unavailable at the last minute, try to find and coordinate with another showciety streamer who is using the charity overlay to raid into as a backup.

# OBS Setup

This zip file contains the scene collection (for import into OBS), image assets, the font used for any custom text you may want, audio assets and anything else you may need. The assumed canvas size is 1920x1080. If you would like to use a 1280x720 canvas size you will need to make your own modifications.

Before opening OBS Studio make sure to right click the SMM2 font "super-mario-maker-2.ttf" and click "Install".

## Importing Scene Collection

To simplify the setup we've included an exported scene collection (SGB24.json). To use this in OBS Studio click "Scene Collection" in the top menu, click Import, the import dialogue should open, click the three dots in the "Collection Path" box, select the JSON file and click the "Import" button.

## Finding Missing Files

Once you import the scene collection you can then click on "Scene Collection" in the top bar and select "SGB24" to load the scene collection (do not do this live as OBS may crash). You will get a dialogue titled "Missing Files" to point OBS to the location all the image and audio assets are stored. Since we've put all the files necessary in this zip file you just have to click "Search Directory..." and browse to where you extracted this to. Once all the files have a new file in the "New File" column you can click "Apply".

## Streamlabs OBS (SLOBS) Setup

SLOBS does not support importing scene collections so you will need to install OBS Studio (https://obsproject.com/), follow the "Importing Scene Collection" and "Finding Missing Files" instructions in OBS Studio and then import that scene collection into SLOBS. Once you have imported into SLOBS you may uninstall OBS Studio if you wish.

Once you have completed "Importing Scene Collection" and "Finding Missing Files" open SLOBS, click on the down-arrow next to "Scenes" panel heading in the bottom left, click "Manage Scene Collections", in the dialogue that opens click "Import Load existing scenes from OBS" in the top right of the dialogue, wait for it to finish importing and all your scene collections from OBS Studio should be imported! If there is more than one scene collection imported you will need to click on the "SGB 2023" scene collection under "Your Scene Collections:" on the left of the dialogue. You may then click "Close" on the "Manage Scene Collections" dialogue and start "Required Customizations"!

## Required Customizations

We have created six "Live" scenes called "Live 16:9 Left", "Live 16:9 Right", "Live 8:7 Left", "Live 8:7 Right", "Live 4:3 Left" and "Live 4:3 Right" for 16:9, 8:7 (i.e. SNES Emulator) and 4:3 (i.e. SNES hardware) games with the camera on the left or right according to your preference. You can remove ones you don't plan on using and optionally rename the remaining one(s) (e.g. "Live").

You will need to edit the sources to change text, match your devices or add your preferred filters (e.g. Cropping, Chroma Key or audio filters like compressor, expander, etc...).

We have added multiple types of video/audio sources for ease of use and you probably will not require ALL of them. Sources you don't plan to use such as "Application Audio Capture (BETA)", "Display Capture" or "Audio Output Capture" (i.e. Desktop Audio) can and should be REMOVED. You will definitely need to modify the sources you do use at least a little bit such as cropping your camera, adding chroma key, adding an audio compressor filter, etc... We won't cover the specifics here other than to say you might need to edit it.

Sources you will likely need to edit or remove:
* Streamer Name Source
* Pronouns Source
* Game Name Source
* Webcam Camera Source
* Game Capture Source
* Display Capture Source
* Capture Card Source
* Desktop Audio
* Mic Source

You will also need to go into Edit > "Advanced Audio Properties" and set the "Audio Monitoring" and "Tracks" columns to work with your audio setup.

Depending on your setup you may need to add your own audio sources and/or remove all of ours. There are too many combinations to list for a general guide.

We can try to help if you're having trouble in the #sgb23-setup-help channel for specific setups.

## Suggested Optional Customizations

You are not limited to ONLY these changes, but these are here as a jumping off point.

* Resize the game to fit the game area. We've added a transform to the game sources that tries to do a good job of doing this, but it may not meet your needs. Feel free to modify them or delete them and add your own. NOTE: SLOBS does not import the transform so this will likely be required if you use SLOBS.
* Adding your own alert sources
* Crop/Resize your camera, add any filters you need, etc...
* Add audio filters if you prefer.
* Change starting / BRB / ending music. We have provided three audio files to choose from, but you may use your own choice of royalty-free music.
* Transitions
* Picture/Rig to put in place of camera for non-camera strimmers

## HOT TIP

Do a recording, try all the scenes, speak a bit and try to play the game for a few minutes to make sure audio is working correctly! You can also do a test stream if you prefer.

# Talking Points

If your mind blanks while you're live and you need some talking points, we got you. Here are some talking points you can OPTIONALLY bring up that may cause people to want to donate.

* "Veterans are our mission. Gaming is our passion." Stack Up bridges veterans and civilians through a shared love of gaming, helping veterans through programs like Stacks, Supply Crates, Air Assaults, and their Stack Up Overwatch Program [StOP].
* Stacks are teams of local volunteers around the globe using gaming and other activities to connect to their communities in order to create a weclome and supporting environment for veterans.
* Supply Crates are video game care packages full of the latest games, gear and console sent to deployed units and veterans in need.
* Air Assaults are all expenses paid trips for veterans to attend life-changing video game and geek culture events such as PAX, ComicCon, TwitchCon, etc...
* StOP: Stack Up's Overwatch Program (StOP) offers peer-to-peer support via Discord, focusing on crisis intervention for gamers, providing a safe space to talk and get help.
* Gaming as therapy: Stack Up uses video games as a powerful tool to combat PTSD, depression, and isolation, offering veterans much-needed community, support, and mental health resources.
* What Does 'Stack Up' mean? In military terms, a stack is a formation used during room clearing. For Stack Up, it represents a community coming together to support veterans through the love of gaming.
* Why gaming? For many veterans, gaming provides relief, a sense of connection, and a way to manage the challenges of reintegrating into civilian life. It's more than just a hobby - it's therapy.

# Pre-Charity-Stream Checklist:

Start your stream at least **5 minutes** before your slot is scheduled to begin so that you're ready to go when it's time.

1. Make sure your overlay looks ok. Power up the game and do a *test recording* or a *test stream* to make sure audio is working properly.
2. Ensure follower/sub only chat is DISABLED so all viewers are allowed to chat.
3. REMOVE all donation links that aren't for the charity from your twitch panels and bots (e.g. commands, timers).
4. Add Twitch's "Charity" tag to your stream for your streams.
5. Keep the charity donations list open so you can read donations aloud: https://tiltify.com/+smm-showciety/showciety-gives-back-2024/donations
	HOT TIP: This URL can be added as a Custom Browser Dock in OBS Studio!
6. Get to know the people before and after your slot so that you can welcome/introduce them.
7. Be ready to go a little longer if the streamer after you has an issue. It's not ideal, but I'm sure you'd like someone to have your back like this if you had issues starting. You won't be expected to fill another time slot if someone ends up not being able to make it, but if you want to you can volunteer.

Stream as you usually would, encouraging donations and talking up the cause (See "Talking Points" if you get stuck). Read out the donation messages as much as you can.

When you have confirmation that the next person on the [schedule](https://horaro.org/sgb2024/schedule) is ready for the switchover, give them a little intro and then raid into their stream.

# Bot Commands

* !donate - You can donate to Stack Up at www.showciety.gives
* !schedule - Want to know who's streaming for the charity? You can find the full schedule here: horaro.org/sgb-2024/schedule
* !charity - Founded in 2015, Stack Up www.stackup.org/ brings both veterans and civilian supporters together through a shared love of video gaming through our primary programs: The Stacks, Supply Crates, Air Assaults, and the Stack Up Overwatch Program [StOP].
* !stackup - Stack Up helps US and Allied military service members get through deployments to combat zones and recover from traumatic physical and emotional injuries with the power of video gaming.
* !incentives - (list your incentives here - see below for common incentive ideas) 
* !showciety - The SMM Showciety is a community of Super Mario Maker streamers, builders, viewers, and players! To get involved with the Showciety, check out our Discord discord.gg/skNMmDe and X x.com/smmshowciety Thanks for your support!

# Indirect donations

To ensure absolute transparency with our viewers, to instill trust with our charity partners, and to avoid unnecessary costs and unduly expectations of our streamers, the Super Mario Showciety Mod team has decided that all Streamers moving forward will only accept donations during charity events via the approved means (i.e. Tiltify). At no time should streamers be handling funds that are meant for our charity partners, this means that streamers shall not encourage their viewers to donate to the charity via bits, subs, or tipping to their channel. If you have any questions, please do not hesitate to reach out via @Mod or DM.

# Crowd Control
Sadly Crowd Control does not support our charity this year. It is not recommended to stream Crowd Control for the event.

# Donation Incentive Ideas

Here are some common donation incentives in no particular order.

* Play a specific game for X minutes (hating the game helps)
* Control Modification
    * Play with controller upside down for X time units
    * Play with Oven Mitts for X time units
    * Play behind the back/head for X time units
    * Play blindfolded for X time units
    * Hands off controller for X time units
    * Change a Keybind for X time units
* Food
    * Hot Peppers
    * Beanboozled
    * Spicy Chips/Confections
    * Food you hate
    * Drink water (laaaaaaaaame :P)
* Clothing
    * Put on a hat
    * Put on a pair of sunglasses
    * Write my name on a T-Shirt
    * Put on another shirt
* Music
    * Karaoke
    * Play me a song
    * Choose a word, improv a song off that
    * Choose an instrument, hear a song
* Body Art
    * Write my name on your arm/face/etc. 
    * Put a sticker on your face/body/etc. 
    * Draw an animal face of donators choice on your arm/face/etc. 
    * Temp Tattoo on face/body/etc.
* Exercise
    * Pushups/Squats/Situps/Burpie/etc. (Can be modified where you do all of them at the end of the stream where $1 = 1 exercise)
* Chat
    * Emote Only for X time units
    * Ban/Timeout Donor/Target for X time units
    * Gift random sub to the community
* Pet
    * Show Pet on Stream
    * Give pet pets
    * Give pet treat
* Social Media
    * Follow Donor on Twitter/Twitch/Youtube
    * Incentives follows (i.e. for every sub on Youtube, the streamer donates $1 to the charity)
    * Shout Donor out on Twitter
    * Add Donor to Auto-Host list for 1 month
* Misc
    * Dance 
    * Draw a picture (extra if they choose)
    * Do a Tongue Twister
    * AMA
    * Change your background (green screen) or change your background lighting 
    * Compliment or Roast Donor
    * Tarot Card Reading
    * Dab
    * ASMR
* Swear Jar
* Mario Maker
    * Play My Level (queue skip)
    * Choose my Character 
    * Make a level (choose the theme and idea)
    * Leave an art comment on the level
    * Skip Current Level 
    * Take a Death
* Pokemon
    * Choose my next Pokemon's Name
    * Pokeballs Only
    * No Healing Items for X time
    * Swap Pokemon NOW
    * Use this Move NOW/Next
    * Disable a move for my next battle 
    * Choose a Pokemon I must release
* Music Games (i.e. Dance Dance, osu!, Beat saber 
    * Choose Next Song 
    * Choose a modifier 
    * Minimal Movement 
* FPS
    * Change Weapon
    * Leave Current Game
    * Invert Controls for XX time
    * Adjust Sensitivity
    * Mute your game
    * Drop all your items
* LoL
    * Choose my next champion
    * Choose my lane
    * Choose my skin
* A M O G U S 
    * Choose character color
    * Kill player of donators choice
    * Kill closest player
    * Self report
    * Do something sus (don't talk, talk to much, control the meeting, etc...)
* Goal/Milestone Based (i.e. not single donation, but based on the total)
    * Change into a cosplay 
    * Change into a costume/pj/etc.
    * Dye/Cut Hair
    * Shave Beard/Head
    * Play a Community Game
    * Play a terrible or scary game
    * Cake or Pie to the face
    * Smash an egg on your head/face
    * Costumed Dancing (i.e. Chicken Dance in a Chicken Suit)
    * Get a new Tattoo
    * Do a Bob Ross Tutorial

# Final Notes

If you are having trouble with anything we will do our best to help in the [#sgb24-setup-help channel](https://discord.com/channels/475693157720522752/1284990295016079430).
