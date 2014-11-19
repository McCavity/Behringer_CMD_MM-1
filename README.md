Behringer_CMD_MM-1
==================

A script to support voice tracking in mAirlist with the Behringer CMD MM-1
MIDI controller

      written by Henning "McCavity" Halfpap
      inspired by the script "Behringer cmd LC-1" written by Thomas "Kloppi"
      Kloppholz
      see: https://github.com/Lexorius/Mairlist-Behringer-Controller/blob/\
      master/Behringer-CMD-LC-1.txt
      License: Creative Commons "CC-BY-SA 3.0"

      Installation instructions:

      1. Place this script in your mAirlist script folder (e.g.
         C:\Program Files\mAirlist\scripts)
      2. Edit this script and set DEBUG to 'true'
      3. Run this script once from mAirlist. Open mAirlist's System Log and
         note the device number of your Controller.
      4. Edit this script again and set mAirlistDevice to the number you just
         noted.
      5. Run this script once again from mAirlist. All buttons should starti
         blinking blue & the VU meters should light up approximately 2/3. If
         this doesn't happen, maybe your devices uses a different MIDI channel.
         You can either cycle through the edit / run sequence each time
         modifying the MIDI channel number until you find the correct setting
         or use Behringer's App (download from Behringer's product page) to
         determine / set the correct MIDI channel. In any case, edit this
         script to reflect the correct MIDI channel number.
      6. Edit this script to set DEBUG to 'false'
      7. (Optional) Run this script once again with DEBUG set to 'false' if
         the test mode was on. This resets test mode.
      8. Set up this scrip as a Notification Script in mAirlist
