# funkradio.start.here
FunkRadio is an enternaining Linux bash script. With it you can listen international broadcast news and enjoy your own favorite music.

Listening to radio is a laid-back way to keep yourself up to date with world events. However, broadcast radio cannot take into account individual music preferences. So sooner or later you want to turn the radio off.

This project presents a Linux bash shell script that combines the best of both worlds -- up-to-date international news and your favorite music.

The script is called funkRadio. You can use it to download and present news broadcasts from internet radio stations. Music comes by the courtesy of your own mp3 files.

## Setting up the funkRadio script
The funkRadio.sh script has been tested in Arch Linux, Debian and Ubuntu environments. Other Linux distributions are probably OK as long as you can install these packages:

- vlc (includes cvlc)
- wget
- mpg123
- ffmpeg (includes speechnorm filter)
- youtube-dl
- curl
- shuf
- bc (for calculations)
  
After installing these packages, please create new directories in your home directory by typing on the terminal:

mkdir ~/funkRadio ~/funkRadio/Archive ~/funkRadio/Talk 
Then download or copy the script funkRadio.sh and place it in the folder ~funk/Radio. Activate the script for later use with the command

chmod u+x  ~/funkRadio/funkRadio.sh
Then, create a log file:

touch ~/funkRadio/Archive/funkRadiolog.txt
If you have a music playlist of the m3u format, please place a copy of it in the folder ~/funkRadio/. The playlist should be a simple filelist. For instance, playlists created by VLC are not OK for our purposes. 

## Lauching funkRadio and making a music playlist

Launche funkRadio by typing on the terminal

~/funkRadio/funkRadio.sh
If there is no music playlist in the directory ~/funkRadio/, the script helps you to create one. First, it will guide you to select a directory which, or its subdirectories, contain mp3 files.

The script shows you directories of your home directory with an assigned number. You are asked to select a directory by typing the associated number.

Perhaps you want to include only relatively short songs? You can set a time limit in minutes if you choose that option.

The last stage in preparing the playlist is to type one or more keywords (music directories, artists, etc) for locating those mp3 files that will be included in the playlist.

The making of the playlist is started when you type 'start' instead of another keyword.

When the playlist is ready, your terminal will show you the funkRadio control panel.

## funkRadio Control Panel
The control panel presents a number of options and associated numbers used to select those options.

You can select a station from which the latest news broadcast will be downloaded. Try option '1' - it downloads some news broadcasts in English.

Wait a minute for the downloads to complete. Then start to listening by selecting option '13 Listen to the funkRadio' in the Control Panel.

While listening, you can toggle between music and news by typing 'Ctrl + C'.

You can turn the radio off by typing 'CTRL + Z'. The command sends the program to the background. The script is turner off also, it you select the last option on the control panel.

### Additional information
Here are some links demonstrating other ways to to work with podcasts on command line.

A script for downloading podcasts: https://github.com/ellencubed/bashpodder

Another script for downloading podcasts: https://github.com/MiguSchweiz/bcaster/blob/master/bcaster

A highly polished script for downloading podcasts: https://github.com/oyvindstegard/podsh/blob/master/podsh #######
