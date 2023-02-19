# CheckiMaker.exe
A fun little tool that allows one to take pictures of one's stream (OBS feed) and sign a cheki (チェキ) style photograph.

![Example](https://github.com/HueVirtualCreature/ChekiMaker/blob/main/Images/ChekiMakerRunningExample.png)

## Instructions to Install

 1. Place the program files (contents of ChekiMaker.Release.xxx.xxx.zip) in C:\Program Files\ChekiMaker
 2. Import and paste the deck data (contents of ImportThisDeckDataIntoSAMMI.txt) into SAMMI
 3. Make sure you have OBS Websocket 5.0 configured (Built into OBS 28+)
 4. Make sure SAMMI is able to connect to OBS using Websockets 5.0
 5. In the newly imported SAMMI deck, called ChekiMaker.exe System, add a trigger to the button, like a channel point redeem.
 6. In the button commands, adjust the positionx and positiony values so that the cheki crops the correct part of the screen.
 7. (Optional) Set up a Discord channel with Webhooks (This is used so that ChekiMaker automatically uploads the image to Discord)
 8. (Optional) Copy the Webhook URL
 9. (Optional) In the button Init Variables, edit discordWebHookURL and insert the Webhook URL
 10. Test and Make sure the button runs and is able to open ChekiMaker.exe and how the picture looks; then send the cheki using the send button and check to see if the image is posted in your Discord Channel
 
## Notes
You do **NOT** need to provide a Discord WebHook URL
If you press the Send button, the image will be sent to "C:\POLAROIDS_SIGNED"; be sure to clear this directory every so often

You can replace the cheki template by replacing the file overlay-polaroid-template.png, but it **must** have the same dimensions
