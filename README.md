Play videos in a terminal.
==========================

Works in Gnome-Terminal and the Linux console.

Convert a .GIF you like to a .txt file with color-changing escape sequences:

convert -compress none -resize 50% kot.gif kot.ppm	# Or use -resize 62x46
ppm_to_plain <kot.ppm >kot2.plain
plain_to_escape 0.1 <kot.plain >kot.txt		# 0.1 is the delay between frames.

Then play it with:

play_video kot.txt

The result should look something like this:

![Screenshot.](https://raw.github.com/tema88/play_video/master/screenshots/Снимок-257.png)

If it doesn't, try running the script from the Linux system console. Have fun!
