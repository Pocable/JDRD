# Web Version
[A newer web version of JDRD was created](https://github.com/Pocable/JDRD-Web-Application). The new version has download cancelation as well as a better UI for downloading tv shows and movies. As I use and like that one more, I will not be updating this repo with new features. I will try to keep this up to date if I change DLAPI's code such that it breaks it, but I will try not to do that.

# JDRD
Python script to search Jackett for a movie/tvshow and send it to DLAPI. I'm just gonna call
this a temp prototype frontend for DLAPI.

Note: Please only use this for grabbing legal backups. I am not responsible for what you do with this.

## Installation
Run these two commands and you are good to go:
```
pip install -r requirements.txt  
python setup.py
python start.py
```

## Configuration
Run setup.py to create a key.txt file, then run start.py.

Input should look something like below:
|Config Tag|Description|
|------|:-----:|
|DLAPI Server | http://127.0.0.1:4248/ |
|DLAPI Key| API key set.|
|Jacket Torznab Path |Should look like http://0.0.0.0:9117/api/v2.0/indexers/all/results/torznab |
|Jackett API Key|Top right of Jackett|
|Movie Output Dir |The directory JDownloader2 will download into when movies are selected (/movies/)|
|TV Output Dir|The directory JDownloader2 will download into when tv shows are selected (/tv/)|

## Troubleshooting

|Issue|Fix|
|:-----:|:----:|
|Throwing Exception| Make sure you are connected to the internet. Other than that post in issues your crash. |
|NON UNICODE TITLE as an option title| Some torrents have non unicode characters in the title. This was a quick fix to display them. |