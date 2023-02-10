# CheckiMaker.exe
A fun little tool that allows one to take pictures of one's stream (OBS feed) and sign a cheki (チェキ) style photograph.

## Instructions to Install

 1. Place the program files (contents of ChekiMaker.Release.xxx.xxx.zip) in C:\Program Files\ChekiMaker
 2. Import and paste the deck data (contents of ImportThisDeckDataIntoSAMMI.txt) into SAMMI
 3. Make sure you have OBS Websocket 5.0 configured (Built into OBS 28+)
 4. Make sure SAMMI is able to connect to OBS using Websockets 5.0
 5. In the newly imported SAMMI deck, called ChekiMaker.exe System, add a trigger to the button: A channel Point redeem.
 6. In the button Init Variables, edit imageFilePath to your liking.
 7. In the button commands, adjust the positionx and positiony values so that the cheki crops the correct part of the screen.
 8. Set up a Discord channel with Webhooks
 9. Copy the Webhook URL
 10. In the button Init Variables, edit discordWebHookURL and insert the Webhook URL
 11.  Test and Make sure the button runs and is able to open ChekiMaker.exe and how the picture looks; then send the cheki using the send button and check to see if the image is posted in your Discord Channel