# Project Overview

The purpose of this project is to collect audio features using web scraping and APIs from the most popular songs in Germany between 2015 and 2022.  
Since audio features are no longer accessible via Spotify, I used the website [www.acousticbrainz.org](https://www.acousticbrainz.org/) to search for audio features.

## Steps

### Step 1
Using the website [https://www.offiziellecharts.de/](https://www.offiziellecharts.de/) and web scraping with the help of BeautifulSoup, I saved the top 100 songs for each year from 2015 to 2022.

### Step 2
Using the song title and artist’s name, I searched for the MBID (MusicBrainz Identifier) on acousticbrainz.org.

### Step 3
After that, using the MBID, I retrieved the audio features for each track by using the API functions of the acousticbrainz.org website.

### Step 4
All results were saved as CSV files. The low-level and high-level audio features were extracted from JSON data and saved into CSV format.

---

Unfortunately, audio features were not available for every song.  
Approximately 30% of the songs had audio features available on the acousticbrainz.org website.