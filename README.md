# Introduction

Here's some instructions for getting ready for the SGB 2025 charity event for The Trevor Project!

# Get Ready For The Event

1. Set up OBS for the event. See "OBS Setup". You may have your own flourish, but we would like to try to have a generally consistent "look" for the event.
2. Make a Tiltify account (or login with Twitch) and request to be part of the team on Tiltify. It requires logging in with Twitch, and going to the [Super Mario Showciety Team Page](https://tiltify.com/+super-mario-showciety/profile) to request an invite. There is a black "Join team +" button next to the "SMM Showciety on Tiltify" header at the top!
3. While **NOT** required we recommend planning donation incentives. See "Donation Incentive Ideas".
4. Set up bot commands for the links to the charity, donation page, etc. (see "Bot Commands"). Optionally set up timers to periodically post the same messages automatically. Make sure there are no conflicting commands - especially for !donate and !charity!
5. Optionally set up a panel on your Twitch channel to advertises the event and provides a link to the donation page.
	a. Click "Add Image" and upload "Panel_Image.png"
	b. Paste "https://tilt.fyi/4XSfyi1iL7" into the "Image Links To:" box.
	c. Click "Submit"
6. Get to know a little about the charity we're supporting so you can talk it up. See "Talking Points" if you need something to get the juices flowing, but you should try to know a few things that the talking points can refresh in your mind's eye.
7. If a Showciety mod is not available try to be around to help coordinate the switchovers if you can. Check the schedule, check that the next streamer is live and ensure they're ready for the raid, then report to the active streamer that the target is ready for the switchover. If there are multiple people talk amongst yourselves to voluntell one of you to handle it so we don't have multiple people trying to do the same thing.

# Stream Setup

This zip file contains the scene collection (for import into OBS), image assets, the font used for any custom text you may want, audio assets and anything else you may need. The assumed canvas size is 1920x1080. If you would like to use a 1280x720 canvas size you will need to make your own modifications or use a 1080p canvas and rescale stream to 720p.

Before opening OBS Studio make sure to right click the SMM2 font "super-mario-maker-2.ttf" and click "Install". If it's not showing up try restarting OBS.

## Importing Scene Collection

To simplify the setup we've included an exported scene collection (SGB25.json). To use this in OBS Studio click "Scene Collection" in the top menu, click Import, the import dialogue should open, click the three dots in the "Collection Path" box, select the JSON file and click the "Import" button.

## Finding Missing Files

Once you import the scene collection you can then click on "Scene Collection" in the top bar and select "SGB24" to load the scene collection (do not do this live as OBS may crash). You will get a dialogue titled "Missing Files" to point OBS to the location all the image and audio assets are stored. Since we've put all the files necessary in this zip file you just have to click "Search Directory..." and browse to where you extracted this to. Once all the files have a new file in the "New File" column you can click "Apply".

# Streamlabs OBS (SLOBS) Setup

SLOBS does not support importing scene collections so you will need to install OBS Studio (https://obsproject.com/), follow the "Importing Scene Collection" and "Finding Missing Files" instructions in OBS Studio and then import that scene collection into SLOBS. Once you have imported into SLOBS you may uninstall OBS Studio if you wish.

Once you have completed "Importing Scene Collection" and "Finding Missing Files" open SLOBS, click on the down-arrow next to "Scenes" panel heading in the bottom left, click "Manage Scene Collections", in the dialogue that opens click "Import Load existing scenes from OBS" in the top right of the dialogue, wait for it to finish importing and all your scene collections from OBS Studio should be imported! If there is more than one scene collection imported you will need to click on the "SGB 2023" scene collection under "Your Scene Collections:" on the left of the dialogue. You may then click "Close" on the "Manage Scene Collections" dialogue and start "Required Customizations"!

## Required Customizations

We have created six "Live" scenes called "Live 16:9 Left Scene", "Live 16:9 Right Scene", "Live 8:7 Left Scene", "Live 8:7 Right Scene", "Live 4:3 Left Scene" and "Live 4:3 Right Scene" for 16:9, 8:7 (i.e. SNES Emulator) and 4:3 (i.e. SNES hardware) games with the game on the left or right according to your preference. You can remove ones you don't plan on using and optionally rename the remaining one(s) (e.g. Naming the one scene you plan on using simply "Live Scene").

You will need to edit the sources to change text, match your devices, use your preferred device settings or add your preferred filters (e.g. Cropping, Chroma Key or audio filters like compressor, expander, etc...) to some degree. The amount you need to change will vary on your setup.

We have added multiple types of video/audio sources with adequate transforms applied for ease of use and you **will not** require ALL of them as there are conflicting sources (e.g. "Desktop Audio Source" and "Application Audio Capture (BETA)"). Make sure to remove conflicting sources or you will have issues. You will need to modify some of the sources you do use at least a little bit such as setting your device, device settings, cropping your camera, adding chroma key, adding an audio compressor filter, etc... We won't cover the specifics here other than to say you might need to edit it.

Sources you will likely need to edit or remove:
* Streamer Name Source
* Pronouns Source
* Game Name Source
* Webcam Source
* Game Capture Source
* Display Capture Source
* Capture Card Source
* Desktop Audio
* Mic Source

You will also need to go into Edit > "Advanced Audio Properties" and set the "Audio Monitoring" and "Tracks" columns to work with your audio setup. We've preset these with some settings that may work for you, but you are responsible for ensuring they work properly.

Depending on your setup you may need to add your own audio sources and/or remove all of ours. There are too many combinations to list for a general guide.

We will try to help if you're having trouble in [#sgb25-setup-help](https://discord.com/channels/475693157720522752/1427377014247129283) for specific setups.

## Suggested Optional Customizations

You are not limited to ONLY these changes! These are here to give you an idea of where to start.

* Resize the game to fit the game area. We've added a transform to the game sources that tries to do a good job of doing this, but it may not meet your needs. Feel free to modify them or delete them and add your own. NOTE: SLOBS does not import the transform so this will likely be required if you use SLOBS
* Adding your own alert sources
* Crop/Resize your camera, add any filters you need, etc...
* Add audio filters to sources
* Change starting / BRB / ending music. We have provided three audio files to choose from, but you may use your own choice of royalty-free music or set up your own custom scenes
* Transitions
* Picture/Rig to put in place of camera for non-camera strimmers

## Bot Commands

Please set up the following bot commands. It's recommended to do this shortly before your stream so you don't impact your normal setup.

!donate - You can donate to The Trevor Project at www.showciety.gives
!schedule - Want to know who's streaming for the charity? You can find the full schedule here! horaro.org/sgb2025/schedule
!charity - The Trevor Project (www.thetrevorproject.org) is the world’s largest suicide prevention and mental health organization for lesbian, gay, bisexual, transgender, queer, and questioning (LGBTQ) young people. Your donations have a direct impact on their ability to provide life-saving counseling services to LGBTQ young people.
!incentives - (list your incentives here - see below for common incentive ideas)
!legislation - The Trevor Project's advocacy programs span the country, and include various types of legislation and education. They have passed 30 bills in the last 10 years, and have fathered 25 different movements, such as "Protecting with Pride".
!trevor - Did you know that one accepting adult decreases the risk of suicide by 40% for LGBTQ young people. The Trevor Project provides LGBTQ youth with 24/7 crisis counseling via phone, text, and chat. Head to www.thetrevorproject.org/get-help if you, or anybody you know may need help.
!showciety - The Super Mario Showciety is a community of Super Mario Maker or Super Mario World streamers, builders, viewers, and players! To get involved with the Showciety, check out our Discord discord.gg/skNMmDe and Blue Sky bsky.app/profile/showciety.org Thanks for your support!

## Finalization

Do a recording, try all the scenes, speak a bit and try to play the game for a few minutes to make sure audio is working correctly! You can also do a test stream if you prefer. Please ping the mods with a screenshot or recording of any scenes you plan to use in [#sgb25-setup-help](https://discord.com/channels/475693157720522752/1427377014247129283) and the mods will give it a once-over and let you know if there are any issues.

# Talking Points

If your mind blanks while you're live and you need some talking points, we got you. Here are some talking points you can OPTIONALLY bring up to inform people on what the charity does. If people know what the charity does is important they will be more likely to donate!

* LGBTQ young people are four times more likely to attempt suicide. Every day, LGBTQ young people reach out for mental health support. When you donate to Trevor, you ensure volunteers can continue to be there for them.
* Trevor provides DIRECT suicide prevention and crisis intervention services to support via phone, text, and chat.
* Trevor fights for policies and laws that protect LGBTQ youth.
* Trevor does research and evaluations that significantly improve their services.
* Trevor provides the world's largest safe-space social networking community.
* Trevor educates and creates public awareness around issues relevant to LGBTQ youth and allies.

# Pre-Charity-Stream Checklist:

Start your stream at least **5 minutes** before your slot is scheduled to begin so that you're ready to go when it's time. Post when you're live in [#sgb25-general](https://discord.com/channels/475693157720522752/1427376805433835610) so a mod or helpful person can check to make sure everything looks and sounds good before the raid.
1. Make sure your overlay looks ok. Power up the game and do a *test recording* or a *test stream* to make sure audio is working properly. You already did this in setup finalization, but it's good to do it again before you're live in case something has changed!
2. Ensure follower/sub only chat is DISABLED so all viewers are allowed to chat.
3. REMOVE all donation links that aren't for the charity from your twitch panels and bots (e.g. commands, timers).
4. Add Twitch's "Charity" tag to your stream.
5. Keep the [Donations+](https://app.tiltify.com/teams/ffdb1c2d-cc74-4048-95a1-421720155892/campaigns/a8c73e5a-1760-4d49-864e-2528e5a71c10/overview/donations) page open so you can read donations aloud. (**HOT TIP:** This URL can be added as a Custom Browser Dock in OBS Studio, however it doesn't work the best unless you click the "fullscreen" button)
6. Get to know the people before and after your slot so that you can welcome/introduce them.
7. Be ready to go a little longer if the streamer after you has an issue. It's not ideal, but I'm sure you'd like someone to have your back like this if you had issues starting. You won't be expected to fill another time slot if someone ends up not being able to make it, but if you want to you can volunteer.

Stream as you usually would, encouraging donations and talking up the cause (See "Talking Points" if you get stuck). Read out the donation messages as much as you can.

When you have confirmation that the next person on the [schedule](https://horaro.org/sgb2024/schedule) is ready for the switchover, give them a little intro and then raid into their stream.

# Indirect donations

To ensure absolute transparency with our viewers, to instill trust with our charity partners, and to avoid unnecessary costs and undue expectations of our streamers, the Super Mario Showciety Mod team has decided that all Streamers moving forward will only accept donations during charity events via the Tiltify platform. At no time should streamers be handling funds that are meant for our charity partners, this means that streamers shall not encourage their viewers to donate to the charity via bits, subs, or tipping to their channel. If you have any questions, please do not hesitate to reach out to a moderator via a ping or DM.

# Crowd Control

We only provide limited instructions for setting up Crowd Control, but we are happy to try to help in [#sgb25-setup-help](https://discord.com/channels/475693157720522752/1427377014247129283).

## Download The App

Download the app from [Crowd Control's website](https://crowdcontrol.live/). Installation is relatively simple. The hard part is setting up the game.

## Game Setup

Game setup is *the* hardest part of Crowd Control. Crowd Control has instructions for every game they support. You can access the game list [here](https://crowdcontrol.live/games/). Once you have selected your game there should be a linke on the left titled "Game Setup Guide". Again, we're happy to try to help in [#sgb25-setup-help](https://discord.com/channels/475693157720522752/1427377014247129283) if you are having trouble.

## Crowd Control Overlay

Crowd Control provides a browser source overlay that shows what effects are active and who sent them. It's meant to fit over top of the game. You can configure how it looks in the Crowd Control app including transparencies. We've included pre-sized browser sources for each aspect ratio for you to paste your overlay URL into. It'll need to be done for each aspect ratio since you can only set one size for an individual browser source.

You can find your URL in the Crowd Control app under "Overlay & Assets". Paste it as the URL for one or more of the pre-sized browser sources in their respective scenes:
* 16:9 Crowd Control Overlay Source
* 8:7 Crowd Control Overlay Source
* 4:3 Crowd Control Overlay Source

## Set Up Charity Donations

In the Crowd Control app go to "Config" -> "Charity" and enter our campaign ID, `a8c73e5a-1760-4d49-864e-2528e5a71c10`, into the "Enter Campaign by ID" box and **click the paper airplane button**. It should come up and show our campaign name: "Showciety Gives back 2025 (SGB25)", part of the description of the campaign and a link to the campaign. If this matches please click "Play for this Charity". Your viewers will now be able to donate for Crowd Control Coins.

## Crowd Control Discord

Crowd Control also has a [Discord server](https://discord.warp.world/) that they also offer help through if we are unable to fix your problem.

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

If you are having trouble with anything we will do our best to help in the [#sgb25-setup-help](https://discord.com/channels/475693157720522752/1427377014247129283).
