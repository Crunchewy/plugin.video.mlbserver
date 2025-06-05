[![GitHub release](https://img.shields.io/github/release/crunchewy/plugin.video.mlbserver.svg)](https://github.com/crunchewy/plugin.video.mlbserver/releases)
![License](https://img.shields.io/badge/license-GPL%20(%3E%3D%202)-orange)
[![Contributors](https://img.shields.io/github/contributors/crunchewy/plugin.video.mlbserver.svg)](https://github.com/crunchewy/plugin.video.mlbserver/graphs/contributors)

# Notes

This software is in a PRE-ALPHA state. Tony Wagner created this version of mlbserver and I greatly prefered it to the original one, mostly becuase the user interface is much more usable on TV browser, which is how I use it. Tony intended it as an eventual replacement for his [mlbserver](https://github.com/tonywagner/mlbserver) but seems to have dropped the idea. I didn't want it to die, so here you go. The rest of this readme is the same, except that the download links are updated to point to this version so they work again. The docker-compose.yml was also updated to point to this version and so works. I hope you enjoy this being back from the dead and please give all the thanks to Tony, not me!

# Current Features

* Watch in a web browser and optionally Kodi
* Watch free games with a free account
* Watch all non-blackout games with a valid subscription
* Generate M3U/XML to watch streams in separate DVR software

# Disclaimer

Blackout restrictions apply.

# Installation

Choose any one of these three methods to install and run:

1. Kodi version 21 (Omega) or newer  
   * [Download and install Kodi](https://kodi.tv/download/) (see this [guide](https://troypoint.com/how-to-install-kodi-on-fire-tv/) for installing on a Fire Stick)  
   * Download the [latest release ZIP file](https://github.com/crunchewy/plugin.video.mlbserver/releases/latest/download/plugin.video.mlbserver.zip) and copy to your Kodi device (or just use code 302431 in the Downloader app on your Fire Stick)  
   * Launch Kodi and install the ZIP in the Addons section (Kodi will prompt you to allow installing addons from unknown sources)  
   * __**Note:** Windows users must also install the [Microsoft Visual C++ Redistributable](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#latest-microsoft-visual-c-redistributable-version) version 14.40.33810.0 or later to [satisfy InputStream Adaptive](https://github.com/xbmc/inputstream.adaptive/issues/1589)__  

2. [Docker](https://hub.docker.com/r/crunchewy/plugin.video.mlbserver)
   * Download the [docker-compose.yml](https://raw.githubusercontent.com/crunchewy/plugin.video.mlbserver/master/docker-compose.yml) template, update the time zone in the file to your own, and create and start the container from a command prompt or terminal like '''docker compose up --detach'''  
   * Alternately, you can run the command '''docker run -d --name plugin.video.mlbserver --env TZ="America/New_York" -p 5714:5714 --volume ./data:/plugin.video.mlbserver/data crunchewy/plugin.video.mlbserver''' (substituting your own time zone, of course)  

3. Python (3.11.7 or newer) with the "requests" module installed  
   * [Download and install Python 3](https://www.python.org/downloads/) if you don't have it already  
   * Install the Python "requests" module like `pip3 install requests`
   * [Download and unzip the [latest release ZIP file](https://github.com/crunchewy/plugin.video.mlbserver/releases/latest/download/plugin.video.mlbserver.zip)  
   * Run the service script like `python3 plugin.video.mlbserver/service.py`

# Usage

Once installed, open any web browser on your network and navigate to http://IP-ADDRESS:5714 (using the IP address of the device running Kodi or the Python script).

If you installed within Kodi, you can access it within the Addons section of Kodi too.
