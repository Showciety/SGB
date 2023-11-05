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
8. REALLY try to help with the switchovers. Things like streamers being late/offline/having technical difficulties at the last minute can happen, and it will be bad if the active streamer has to try to coordinate that themselves. If someone is truly unavailable at the last minute, try to find and coordinate with another showciety streamer who is using the charity overlay to raid into as a backup.

# OBS Setup

This zip file contains the scene collection (for import into OBS), image assets, the font used for any custom text you may want, audio assets and anything else you may need. The assumed canvas size is 1920x1080. If you would like to use a 1280x720 canvas size you will need to make your own modifications.

Before opening OBS Studio make sure to right click the SMM2 font "super-mario-maker-2.ttf" and click "Install".

## Importing Scene Collection

To simplify the setup we've included an exported scene collection (SGB_2023 for OBS.json). To use this in OBS Studio click "Scene Collection" in the top menu, click Import, the import dialogue should open, click the three dots in the "Collection Path" box, select the JSON file and click the "Import" button.

## Finding Missing Files

Once you import the scene collection you can then click on "Scene Collection" in the top bar and select "SGB 2023" to load the scene collection (do not do this live as OBS may crash). You will get a dialogue titled "Missing Files" to point OBS to the location all the image and audio assets are stored. Since we've put all the files necessary in this zip file you just have to click "Search Directory..." and browse to where you extracted this to. Once all the files have a new file in the "New File" column you can click "Apply".

## Streamlabs OBS (SLOBS) Setup

SLOBS does not support importing scene collections so you will need to install OBS Studio (https://obsproject.com/), follow the "Importing Scene Collection" and "Finding Missing Files" instructions in OBS Studio and then import that scene collection into SLOBS. Once you have imported into SLOBS you may uninstall OBS Studio if you wish.

Once you have completed "Importing Scene Collection" and "Finding Missing Files" open SLOBS, click on the down-arrow next to "Scenes" panel heading in the bottom left, click "Manage Scene Collections", in the dialogue that opens click "Import Load existing scenes from OBS" in the top right of the dialogue, wait for it to finish importing and all your scene collections from OBS Studio should be imported! If there is more than one scene collection imported you will need to click on the "SGB 2023" scene collection under "Your Scene Collections:" on the left of the dialogue. You may then click "Close" on the "Manage Scene Collections" dialogue and start "Required Customizations"!

## Required Customizations

We have created four "Live" scenes called "Live (16:9 Left)", "Live (16:9 Right)", "Live (4:3 Left)" and "Live (4:3 Right)" for 16:9 and 4:3 games with the camera on the left or right according to your preference. You can remove ones you don't plan on using and optionally rename the remaining one(s) (e.g. "Live").

You will need to edit the sources to change text, match your devices or add your preferred filters (e.g. Cropping, Chroma Key or audio filters like compressor, expander, etc...).

We have added multiple types of video/audio sources for ease of use and you probably will not require ALL of them. Sources you don't plan to use such as "Application Audio Capture (BETA)", "Display Capture" or "Audio Output Capture" (i.e. Desktop Audio) can and should be REMOVED. You will definitely need to modify the sources you do use at least a little bit such as cropping your camera, adding chroma key, adding an audio compressor filter, etc... We won't cover the specifics here other than to say you might need to edit it.

Sources you will likely need to edit or remove:
* Streamer Name
* Game Name
* Camera
* Game Capture
* Display Capture
* Video Capture Device
* Application Audio Capture (BETA)
* Audio Output capture
* Mic

You will also need to go into Edit > "Advanced Audio Properties" and set the "Audio Monitoring" and "Tracks" columns to work with your audio setup.

Depending on your setup you may need to add your own audio sources or remove all of ours. There are too many combinations to list for a general guide.

We can try to help if you're having trouble in the #sgb23-setup-help channel for specific setups.

## Suggested Customizations

You are not limited to ONLY these changes, but these are here as a jumping off point.

* Resize the game to fit the game area. We've added a transform to the game sources that tries to do a good job of doing this, but it may not meet your needs. Feel free to modify them or delete them and add your own. NOTE: SLOBS does not import the transform so this will likely be required if you use SLOBS.
* Crop/Resize your camera, add any filters you need, etc...
* Add audio filters if you prefer.
* Change text outlines:
    * YELLOW - #FFF600
    * WHITE - #FFFFFF
    * DARK YELLOW - #907a01
    * GREY - #2b2b2b
* Transitions
* Picture to put in place of camera for non-camera strimmers

## HOT TIP

Do a recording, try all the scenes, speak a bit and try to play the game for a few minutes to make sure audio is working correctly! You can also do a test stream if you prefer.

# Talking Points

If your mind blanks while you're live and you need some talking points, we got you. Here are some talking points you can OPTIONALLY bring up that may cause people to want to donate.

* LGBTQ young people are four times more likely to attempt suicide. Every day, LGBTQ young people reach out for mental health support. When you donate to Trevor, you ensure volunteers can continue to be there for them.
* Trevor provides DIRECT suicide prevention and crisis intervention services to support via phone, text, and chat.
* Trevor fights for policies and laws that protect LGBTQ youth.
* Trevor does research and evaluations that significantly improve their services.
* Trevor provides the world's largest safe-space social networking community.
* Trevor educates and creates public awareness around issues relevant to LGBTQ youth and allies.

# Pre-Charity-Stream Checklist:

Start your stream at least 5 minutes before your slot is scheduled to begin so that you're ready to go when it's time.

1. Make sure your overlay looks ok. Power up the game and do a *test recording* or a *test stream* to make sure audio is working properly.
2. Ensure follower/sub only chat is DISABLED so all viewers are allowed to chat.
3. REMOVE all donation links that aren't for the charity from your twitch panels and bots (e.g. commands, timers).
4. Add Twitch's "Charity" tag to your stream for the duration of the event.
5. Keep the charity donations list open so you can read donations aloud: https://tiltify.com/+smm-showciety/showciety-gives-back-2023/donations?scopeKey=c2hvd2NpZXR5LWdpdmVzLWJhY2stMjAyMw==
	HOT TIP: This URL can be added as a Custom Browser Dock in OBS Studio!
6. Get to know the people before and after your slot so that you can welcome/introduce them.
7. Be ready to go a little longer if the streamer after you has an issue. It's not ideal, but I'm sure you'd like someone to have your back like this if you had issues starting.

Stream as you usually would, encouraging donations and talking up the cause (See "Talking Points" if you get stuck). Read out the donation messages as much as you can.

When you have confirmation that the next person on the schedule (https://horaro.org/sgb2023/schedule) is ready for the switchover, give them a little intro and then raid into their stream.

# Bot Commands

!donate - You can donate to The Trevor Project at www.showciety.gives

!schedule - Want to know who's streaming for the charity? You can find the full schedule here! horaro.org/sgb2023/schedule

!charity - The Trevor Project (www.thetrevorproject.org) is the world’s largest suicide prevention and mental health organization for lesbian, gay, bisexual, transgender, queer, and questioning (LGBTQ) young people. Your donations have a direct impact on their ability to provide life-saving counseling services to LGBTQ young people.

!incentives - (list your incentives here - see below for common incentive ideas)

!legislation - The Trevor Project's advocacy programs span the country, and include various types of legislation and education. They have passed 30 bills in the last 10 years, and have fathered 25 different movements, such as "Protecting with Pride".

!showciety - The SMM Showciety is a community of Super Mario Maker streamers, builders, viewers, and players! To get involved with the Showciety, check out our Discord discord.gg/skNMmDe and Twitter twitter.com/smmshowciety . Thanks for your support!

!trevor - Did you know that one accepting adult decreases the risk of suicide by 40% for LGBTQ young people. The Trevor Project provides LGBTQ youth with 24/7 crisis counseling via phone, text, and chat. Head to www.thetrevorproject.org/get-help if you, or anybody you know may need help.

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
* Crowd Control (See "Crowd Control" below)
    * Switch to a different, harder game or a game you hate for X time units

## Crowd Control

Crowd Control is an incentive itself! You don't technically need any other incentives for a Crowd Control stream, but don't limit yourself if you don't want to. Incentives above and beyond are NOT required, but they can also be a lot of fun!

### Crowd Control Charity Campaign Setup

We will not be covering how to set up Crowd Control for games. Crowd Control has many articles on how to set up individual games. We are only covering how to link to our charity campaign.

1. Install Crowd Control (https://crowdcontrol.live/) by downlaoding and running the installer with the big red "Download" button in the top right.
2. Log in to the app.
3. Go to Config > Charity in the menu on the left of the app.
4. Enter the following campaign ID in the "Enter Campaign by ID" box: c28d1a42-dd41-4d70-aec3-f306e450f145
5. Click the little paper airplane button to initate the link.
6. The "Showciety Gives Back 2023" campaign should show up under "Manage your Charity Campaign".
7. Set up your game following Crowd Control's instructions: https://crowdcontrol.live/games/

Once you've linked your account to the campaign the coin purchases through Crowd Control should go to Tiltify and count towards our amount raised for The Trevor Project!

Once the event is over don't forget to click on the red "Unlink" button in the botom right if you plan on doing Crowd Control for yourself later!

If you are having trouble with anything we will do our best to help in the #sgb23-setup-help channel.