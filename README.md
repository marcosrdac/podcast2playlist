# podcast2playlist
Bash script for Linux to convert podcast rss feeds to m3u, pls and Volumio 2 playlist files. It allows you to stream episodes of radio shows to Pi Musicbox, Volumio or other MPD/Mopidy clients. Tested with Pi Musicbox, Volumio 1 and Volumio 2 on a Raspberry Pi with Raspbian Jessie.

##Dependencies:
xsltproc

##Installation on Debian/Ubuntu:
- sudo apt-get update
- sudo apt-get install xsltproc
- download files into directory /home/volumio/podcast2playlist
- nano podcast2playlist.sh
- change destination folders and script folder in code and save
- chmod +x podcast2playlist.sh
- nano rssfeeds.txt
- paste rss feeds, 1 per line, like
- OVT;http://radiobox2.omroep.nl/rss/ug/programme/28.rss

##Usage:
- /home/volumio/podcast2playlist/podcast2playlist.sh

or something like

- crontab -e
- 0 * * * * /home/volumio/podcast2playlist/podcast2playlist.sh


