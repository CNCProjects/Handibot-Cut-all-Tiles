Handibot-Cut-all-Tiles
======================

This is a ShopBot file that will allow your Handibot to cut one tile after another without having to load each file one by one.

Here's how it works:

Go to VCarve and make a tiled toolpath. Save that toolpath with no filename. VCarve will create filenames with T1_.sbp T2_.sbp etc.

Drop this file from Github into the directory where you exported all of your tiles

Open Shopbot, set your parts folder to the folder you set in Step 2

Run the "Cut all tiles file"

It will open up and zero the axis by running that Zero XY SBP file

It will pick T1, cut it, and wait for you to hit GO for the next tile, T2 It'll keep going to 50 tiles and then it unceremoniously ends. (or you can just quit out :)


If you get screwed up, you can uncomment the GOTO command and set it to whatever tile you left off on, because I put labels on each and every tile cutting command for that exact purpose.
