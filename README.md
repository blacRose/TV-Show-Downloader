# What the hell is this thing ?
Maybe you're a guy a bit like me -- who watch a *lot* of series -- so I guess you already know that downloading the latest episodes of all your favorites TV Shows is absolutely PAINFUL. I mean it, really.

Each serie is released always the same day each week ; but obviously it's hard to remember the release day of all your shows (by the way, sometimes they make a little break, so you won't have episode during 2/3 months).

Thus, TVShow Downloader is a set of basic scripts (crontab + python script + bash script) designed
to simplify my whole existence on this earth: I haven't to think about downloading my serie anymore \o/.

# How it works ?
The idea behind this "project" is very, very, (really.) very simple:
    * The python script checks if a new episode is released by the eztv team (btw, thank you guys)
        * if a new one is available, the script writes its magnet URI somewhere and add it to the database
        * if the latest released is already in the TVShow Downloader, it does nothing
    
    * With a bash script you can add the magnets into your favorite torrent manager (I personaly use transmission, I've planned to fully integrate this one in my script... one day.)

    * Last part, the crontab runs the whole process one time per day for example!

Anyway I hope you'll enjoy the thing as much as I do (at least).

# Requirements
Currently, it only uses the feedparser library ; you can find it here:
    http://code.google.com/p/feedparser/

NB: Maybe, I will replace the feedparser library by basics python regex