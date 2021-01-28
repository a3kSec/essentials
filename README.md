# essentials
- For Windows

- The intent of this script is to help install many apps after a reformat

## Usage
- A default list of apps has been included in the 'app_ids.txt' file
- To search for apps to add to the app_ids.txt list, in your terminal type:
```
C:\> winget search chrome   

Name                  Id                                 Version    Match
-------------------------------------------------------------------------------
Brave Browser Nightly BraveSoftware.BraveBrowser-Nightly latest     Tag: Chrome
Brave Browser         BraveSoftware.BraveBrowser         1.18.77    Tag: Chrome
webview2 evergreen    microsoft.webview2-evergreen       1.3.139.59 Tag: chrome
Google Chrome Beta    Google.ChromeBeta                  latest
Google Chrome         Google.Chrome                      latest                <------------ 'Google.Chrome' is the app id for Chrome browser
```

- If you get an error about winget, run the script once to install it.

### Download zip
- Download [essentials.zip](https://github.com/a3kSec/essentials/archive/1.0.zip) and extract.
- Find the powershell script, right click and click run with powershell.
- When it prompts for the file path, give it the path of where your app id list is located (a default list called app_ids.txt has been included)
```
cmdlet essentials.ps1 at command pipeline position 1
Supply values for the following parameters:
FilePath: C:\scripts\essentials\app_ids.txt
```

### Github
```
C:\scripts> git clone https://github.com/a3kSec/essentials.git

C:\scripts> cd essentials

C:\scripts\essentials> .\essentials.ps1 -FilePath C:\scripts\essentials\app_ids.txt
```