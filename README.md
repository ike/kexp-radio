# kexp-radio

A tiny script that helps you stream 90.3 KEXP from Seattle Washington. Also includes cronjob for a radio alarm clock.

## Requirements

Make sure mplayer is installed. If it's not already available on your system, download and install it here: https://mplayerhq.hu/design7/news.html

## Installation

On most Unix-like systems, just put the shell script in your `/usr/local/bin` and make sure it's executable.

```
git clone git@github.com:ike/kexp-radio
cd kexp-radio
cp kexp /usr/local/bin
sudo chmod a+x /usr/local/bin/kexp
```

## Alarm clock crontab

Use the included crontab to turn on KEXP as a radio alarm clock. The crontab is currently set to 7am. Check out [Crontab Guru](https://crontab.guru) for a refresher on how to set a cron job correctly.

## Usage

 - `kexp --start` will start the stream in the background.
 - `kexp --stop` will stop the currently playing stream.
 - `kexp --np` will grab the current song title, if available.
