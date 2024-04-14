# RobloxServerFinder
Find a roblox server in a given region. This program was written in python (which I'm not too proficient in) so expect some spaghetti code.

I might make a javascript extension for this if someone pays me.

# Installation:
Open your terminal and move to the directory you wish to install this tool and clone this repo: `git clone https://github.com/Exilon24/RobloxServerFinder.git`

Then `cd` into the installed directory and run `pip install -r requirements.txt`

The program requires some settings to be set. Open up `roServerFinder.py` in a text editor (notepad, vim, anything really). There are 2 fields you need to set (starting line 7):

```py
# Enter your roblox cookie here
robloxCookie = ""

# enter desired regions here: DE, SG, US, UK, FR, IN
regions = ["DE", "SG"]
```

Then go to the directory `roServerFinder.py` is in and run `python roServerFinder.py` and enter the game ID e.g: `https://www.roblox.com/games/15069312471/LifeLike-Disasters` game ID is `15069312471`

This will open a browser window, requesting to join a roblox game. It will prompt you to allow roblox to open. If you decline, roblox will not open. The browser window will automatically close after you join.

# Security concerns
## This program requires your roblox cookie to work
It will NOT automatically get these cookies. You must provide them yourself

All the code you will run can be seen on this github (open source).

All this program does is uses the roblox API to find servers (your cookie is used to authenticate these requests) and `https://ip-api.com/` (which only recieves the servers IP address) to get the server region. a selenium webdriver is used to open the browser on roblox, login with your cookie and run the game.

Do not send the code to other people directly as you may still have your cookie saved. Instead, send them to this github.

If you really do not trust this program, you can create an alt account and use that cookie instead.
