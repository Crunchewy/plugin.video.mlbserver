[![GitHub release](https://img.shields.io/github/release/tonywagner/plugin.video.mlb.svg)](https://github.com/tonywagner/plugin.video.mlb/releases)
![License](https://img.shields.io/badge/license-GPL%20(%3E%3D%202)-orange)
[![Contributors](https://img.shields.io/github/contributors/tonywagner/plugin.video.mlb.svg)](https://github.com/tonywagner/plugin.video.mlb/graphs/contributors)

# Features

* Watch in Kodi and/or a web browser
* Watch recaps and highlights
* Watch free games with an account
* Watch all non-blackout games with a valid subscription

# Disclaimer

Blackout restrictions apply.

# Installation

Choose any one of these three methods to install and run:

1. Kodi version 21 (Omega) or newer  
   * [Download and install Kodi](https://kodi.tv/download/)  
   * [Download the [latest release ZIP file](https://github.com/tonywagner/plugin.video.mlb/releases/latest/download/plugin.video.mlb.zip)  
   * Copy ZIP file to your Kodi device if necessary, and then run Kodi and install the ZIP in the Addons section (Kodi will prompt you to allow installing addons from unknown sources)  
   * __**Note:** Windows users must also install the Microsoft Visual C++ Redistributable version 14.40.33810.0 or later__  

2. Python (3.11 or newer) with the "requests" module installed  
   * [Download and install Python 3](https://www.python.org/downloads/) if you don't have it already  
   * Install the Python "requests" module like `pip install requests` or `pip3 install requests`
   * [Download and unzip the [latest release ZIP file](https://github.com/tonywagner/plugin.video.mlb/releases/latest/download/plugin.video.mlb.zip)  
   * Run the service script like `python plugin.video.mlb/service.py` or `python3 plugin.video.mlb/service.py`

3. Docker
   * Coming soon!  

# Usage

Once installed, you can access the addon from any web browser on your network at http://IP-ADDRESS:5714 (using the IP address of the device running Kodi or the Python script).

If you installed within Kodi, you can access it within the Addons section of Kodi too.

# Notes

Intended as a replacement for both [plugin.video.mlbtv](https://github.com/eracknaphobia/plugin.video.mlbtv) and [mlbserver](https://github.com/tonywagner/mlbserver)

