# Raid Train Single Link (aka RTSL)
by Osiris Indriya (https://www.twitch.tv/osirisindriya)

## Why RTSL?
One way to build community on Twitch.tv is for streamers to raid other channels, introducing their viewers to someone else's content and community. A popular way host events on Twitch.tv is to prearrange a sequence of scheduled streams and raids otherwise known as a "Raid Train". Raid Trains are the best way to spready the love around, giving every streamer's channel an opportunity to get viewers and direct support. The problem is that it can be hard to track a Raid Train in progress as the train moves from channel to channel, especially for people less familiar with Twitch.

## What is RTSL?
This package was is created to allow a single URL to redirect according to a predetermined schedule. This allows one link to land a user on the current active channel on a planned Raid Train. Once set up, this link can be shared widely inside and outside of Twitch.tv to direct people to a promotional page before the event begins, and to the Raid Train in progress. This single link is ideal for gathering new viewers who are not familiar with Twitch.

## What do I need to get started?
* An Internet-accessible domain
* FTP access to publish HTML and image files at that domain
* Some experience editing HTML and JavaScript

## How to set up RTSL?

1. Create a directory in a website directory you have FTP access to.

1. [Download](https://github.com/BLESSOTERIC/rtsl/archive/v1.zip) and copy the package files into that directory, including:
    * `/rtsl-1/` (directory)
    * `/rtsl-1/event-name/` (directory)
    * `/rtsl-1/event-name/index.html` (HTML doc with redirect script)
    * `/rtsl-1/event-name/img/` (directory)
    * `/rtsl-1/event-name/img/cover.png` (social share image for your event)

1. Add `luxon.js` to the `/rtsl/` directory.
    * Get the latest `luxon.js` download at https://moment.github.io/luxon/docs/manual/install.html

1. Modify the `/event-name/` directory name to be specific to your event.

1. Create a shortened link using your favorite shortener like Bit.ly and point it to your new Raid Train directory https://yourdomain.com/rtls/your-event-directory/, making sure to change the URL and directory to match what you set up previously for this event.

1. Replace `/rtls/event-1/img/cover.png` with your own event image that will appear when sharing the link on Facebook.

1. Updtate the <head> section below with your event details:
    * `meta description`
    * `meta keywords`
    * `meta og:title`
    * `meta og:image` <--- only change if you are using a different file name and/or file type for the cover image
    * `meta og:url`
    * `title`

1. The script is where the magic happens: 
    * It is set up to collect the users' browser time and convert all times to PST. If you want to use a different master time zone, please refer to the luxon.js documentation.
    * Only change the code where explicitly told to do so by comments.

## Who made this?
RTSL was created by Osiris Indriya to help us build a bigger and stronger community of support for Twitch DJs. If you value this work, please consider showing your support.

### Follow/Subscribe: 
* Twitch: https://www.twitch.tv/osirisindriya

### Donate:
* PayPal: paypal.me/OsirisIndriya
* Venmo: @Osiris-Indriya

### Participate:
* Github: https://github.com/BLESSOTERIC/rtsl/

## Credits

### cover.png Designer
Polygon Rainbow (www.flow.page/polygonrainbow)
