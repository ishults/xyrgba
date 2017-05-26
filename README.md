# xyrgba
A simple browser-based pixel coloring framework for Twitch

In the xyrgba.html file, replace:
* `$yourNick` with your Twitch username
* `$yourKey` with your auth key from Twitch
* `$yourChannel` with the channel you want to monitor
    
Optionally, you can update the `MAGIC_WORD` variable as well.  Then open the file and point your streaming client at it.  The page should now be listening to the channel and properly painting the canvas based on the user input (e.g. `do: 10 10 255 0 255 125`).
