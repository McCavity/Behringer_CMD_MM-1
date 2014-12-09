Behringer_CMD_MM-1
==================

A script to support voice tracking in mAirlist with the Behringer CMD MM-1
MIDI controller

      written by Henning "McCavity" Halfpap
      inspired by the script "Behringer cmd LC-1" written by Thomas "Kloppi"
      Kloppholz
      see: https://github.com/Lexorius/Mairlist-Behringer-Controller/blob/\
      master/Behringer-CMD-LC-1.txt

      Copyright 2014 Henning Halfpap

      Licensed under the Apache License, Version 2.0 (the "License");
      you may not use this file except in compliance with the License.
      You may obtain a copy of the License at

          http://www.apache.org/licenses/LICENSE-2.0

      Unless required by applicable law or agreed to in writing, software
      distributed under the License is distributed on an "AS IS" BASIS,
      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
      See the License for the specific language governing permissions and
      limitations under the License.

      Installation instructions:

      1. Place the file „Behringer_CMD_MM-1.mls“ in your mAirlist script
         folder (e.g. C:\Program Files\mAirlist\scripts)
      2. Edit the script and set DEBUG to 'true'
      3. Run the script once from mAirlist. Open mAirlist's System Log and
         note the device number of your Controller.
      4. Edit the script again and set mAirlistDevice to the number you just
         noted.
      5. Run the script once again from mAirlist. All buttons should start
         blinking blue & the VU meters should light up approximately 2/3. If
         this doesn't happen, maybe your devices uses a different MIDI channel.
         You can either cycle through the edit / run sequence each time
         modifying the MIDI channel number until you find the correct setting
         or use Behringer's App (download from Behringer's product page) to
         determine / set the correct MIDI channel. In any case, edit this
         script to reflect the correct MIDI channel number.
      6. Edit the script to set DEBUG to 'false'
      7. (Optional) Run this script once again with DEBUG set to 'false' if
         the test mode was on. This resets test mode.
      8. Set up the scrip as a Notification Script in mAirlist
