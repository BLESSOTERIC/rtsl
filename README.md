# Raid Train Single Link (aka RTSL)
by Osiris Indriya

## Why RTSL?
Raid trains are the best way to spready the love around, giving every streamer's channel an opportunity to get viewers and direct support. The problem is that it can be hard to track a raid train in progress as the train moves from channel to channel, especially for people less familiar with Twitch.

## What is RTSL?
This page and the package it is contained within is created to allow the use of a single URL to redirect on a schedule to follow the planned Raid Train, allowing anyone who clicks it to land on the current stream. This is perfect for promoting on Instagram, Facebook, EventBrite, etc. using a single URL.

## How to set up RTSL?

1. Create a directory on a website you have FTP access to.

2. Copy the package files into that directory, including:
  * `/rtsl/` (directory)
  * `/rtsl/event-1/` (directory)
  * `/rtsl/event-1/index.html` (HTML doc with redirect script)
  * `/rtsl/event-1/img/` (directory)
  * `/rtsl/event-1/img/cover.png` (social share image for your event)

3. Add `luxon.js` to the `/rtsl/` directory

3. Modify the `/event-1/` directory name to be specific to your event. I recommend using a date and event name like this `2021-03-13-raid-train-name`.

4. Create a shortened link using your favorite shortener like Bit.ly and point it to your new raid train directory https://yourdomain.com/rtls/your-event-directory/, making sure to change the URL and directory to match what you set up previously for this event.

5. Replace `/rtls/event-1/img/cover.png` with your own event image that will appear when sharing the link on Facebook.

6. Updtate the <head> section below with your event details:
  * `meta description`
  * `meta keywords`
  * `meta og:title`
  * `meta og:image` <--- only change if you are using a different file name and/or file type for the cover image
  * `meta og:url`
  * `title`

7. The script is where the magic happens: 
  * It is set up to collect the users' browser time and convert all times to PST. If you want to use a different master time zone, please refer to the luxon.js documentation.
  * Only change the code where explicitly told to do so by comments.

## Who made this?
RTSL was created by Osiris Indriya to help us build a bigger and stronger community of support for Twitch DJs. If you value this work, please consider showing your support.

### Follow/Subscribe: 
- Twitch: https://www.twitch.tv/osirisindriya

### Donate:
- PayPal: paypal.me/OsirisIndriya
- Venmo: @Osiris-Indriya

### Participate:
- Github: https://github.com/BLESSOTERIC/rtsl/
