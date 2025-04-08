# RecoverPlaysTVClips
Download PlaysTV clips post shutdown.

This script will allow you to (hopefully) download those old PlaysTV clips you may think are gone and forgotten.

None of this would be possible without the Internet Archive. If this has helped and you can spare a bit of money donate to them at https://archive.org/donate?origin=iawww-TopNavDonateButton

## How does it work?
It uses Internet Archive to access the latest archived version of your Plays TV profile and attempts to download each one of your videos with highest quality possible. I was able to download approximately half of my old clips. (o7 to the rest of the clips lost forever)

## Requirements
1. [Python 3.7+](https://www.python.org/downloads/)
2. [git](https://git-scm.com/downloads)

## Installation and Usage
1. Install the repo and change your directory to the script's location
```
git clone https://github.com/RJTuckey/RecoverPlaysTVClips
cd RecoverPlaysTVClips
```
2. Install the required libraries
```
python -m pip install -r requirements.txt
```
3. Run the script with your Plays.TV username
```
python playstvrecover.py YourPlaysTVUsername
```
That's it! The script will keep you informed in the process.

## Options
```
usage: playstvrecover.py [-h] [-p PATH] [-f] [--headless] username

Download some of your old Plays.TV clips from the web archive.

positional arguments:
  username              your Plays.TV username

optional arguments:
  -h, --help            show this help message and exit
  -p PATH, --path PATH  the directory where all videos will be placed in
  -f, --force           overwrite/re-download if the video is already downloaded
  --headless            use a headless browser (no gui)
```
