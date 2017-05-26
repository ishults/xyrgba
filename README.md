# xyrgba
A simple browser-based pixel coloring framework for Twitch

In the xyrgba.html file, replace:
* `$yourNick` with your Twitch username
* `$yourKey` with your auth key from Twitch
* `$yourChannel` with the channel you want to monitor
    
Optionally, you can update the `MAGIC_WORD` variable as well.  Then open the file and point your streaming client at it.  The page should now be listening to the channel and properly painting the canvas based on the user input (e.g. `xyrgba: 10 10 255 0 255 125`).

The program also limits the number of times a user can post in the `$TIMEOUT` variable.  Mods of the channel are exempt from this limit.  Mods may also type the `$KILL_SWITCH` word to refresh the page.

A user with access to the actual browser page may click on the canvas to quickly draw large squares (for erasing inappropriate content, etc.).

Every `$SAVE_TIMEOUT` milliseconds, the page will save the content to local storage.  This is restored upon reloading the page.
