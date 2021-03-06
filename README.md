# FiveThirtyEight Baseball Data scrape

This is a script I wrote to scrape fivethirtyeight.com's daily baseball predictions. The function allows users to automatically populate two (2) data frames: i) All the games involving National League Teams and ii) All games involving American League Teams. The data frame is a nx3 with columns: ``` Team, Win (Win percentage), and Date. ```
```
> al.odds
        Team  Win       Date
1    Orioles 0.53 Tue Aug 16
2     Redsox 0.47 Tue Aug 16
3     ...
...
```
Added columns for EV also, which gives you ODDs (decimal) that a bet will have a positive value. 

**Website:** 
http://projects.FiveThirtyEight.com/2016-mlb-predictions

**Main function:**
```
GetOdds(kVector.of.strings)  # Strings are passed through lapply 
(where kVector.of.strings <-"Mariners, ...")
```
The final Data frames are titled ``` nl.odds ``` and ``` al.odds ```.

**Notes:**
Google's R style guide is followed.

