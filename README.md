# EdX powered courses video downloader

This script is intended to download course videos from http://university.mongodb.com
or any other site 'Powered by EdX' (including, of course, http://edx.org itself).

This script relies on [youtube-dl](https://github.com/rg3/youtube-dl/) project
to download videos.

Accepts destination path as optional parameter.

###Dependencies:

* Python 2.7
* Mechanize
* BeautifulSoup4
* Youtube\_dl

### Installation

    git clone https://github.com/svnindia/edu_10gen_dl.git
    cd edu_10gen_dl
    sudo pip install -r requirements.txt

Populate `config.py` with domain and credentials of site, from which you're going to download videos.

Optionally set another options in `config.py` like `writesubtitles` to enable subtitles.

### Usage:

+ `python edx_dl.py`

+ `python edx_dl.py c:\Users\MyUser\Lectures\`

+ `python edx_dl.py --interactive c:\Users\MyUser\Lectures\` To Download all the videos from the Course chapter

+ `python edx_dl.py --interactive --pause /home/svnindia/Downloads/tut_edx/` To Download the specipfic videos from the Course chapter, for each video Download Permission asked

+ `python edx_dl.py --interactive --resume /home/svnindia/Downloads/tut_edx/` To Download all the videos from the Course chapter from the broken download.Because of some reasons we may not able to downloaded all the videos in that case we can make use of the below
