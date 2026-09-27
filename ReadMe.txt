================================================================================
  Amazon Echo Show Clock and Weather Display
  By Mechanical Whispers, v0.6.1, September 21st, 2026

  To get the latest updates or support me by buying me a shot of whiskey,
  please visit Patreon.com/MechanicalWhispers
================================================================================

This .html web page is the result of my frustration with just wanting my Amazon Echo Show 5 device to stop showing ads, and simply keep a constant display of the time and pertinent weather information I wanted at a glance. My frustration turned to joy when I discovered that I could use the free MyPage Alexa Skill to display any web page in the default Echo Silk Browser, and use a 1-second looping .mp3 playing in the background to keep the page from going away (Without this looping .mp3 playing in the background, Amazon Echo Show devices will return to your Home screen after 10 minutes if no activity is detected).

I added in all the weather info that I wanted on the page, and made it easy for anyone to customize for their own locations. In the hopes that this would also make others just as happy, I have decided to release it here on my Patreon for free.


REQUIREMENTS:
- Being frustrated with your Amazon Echo Show device or similar that disrupts your day with ads, and that can load web pages into a (Silk) web browser
- MyPage Amazon Alex Skill Enabled (FREE at https://www.amazon.com/dp/B09CG879RG)
- FTP web server where you can upload the two files (.html and .mp3, and optionally a .jpg for a custom background)
- Currently only works in 5-digit US ZIP code locations.


(1.) Unpack the ZIP file to your computer.
(2.) Open the .html file in a text editor and look for the following variables near the top of the code. Edit these to your preferences.
=========================================================================
  TEMPLATE CONFIGURATION VARIABLES
=========================================================================

CONFIG_ZIP_CODE       = "Input your local 5-digit US ZIP code here, inside the quotes"
CONFIG_LOCATION_NAME  = "Can be any text you want to describe your location, inside the quotes"
CONFIG_TEMP_UNIT      = "F for Fahrenheit, C for Celsius, inside the quotes"
CONFIG_BG_IMAGE_URL_DAY   = "URL to your daytime background image, leave blank for default color, inside the quotes"
CONFIG_BG_IMAGE_URL_NIGHT = "URL to your nighttime background image, leave blank for default color, inside the quotes"
CONFIG_AUDIO_URL      = "URL to your silent looping .mp3, leave blank to disable, inside the quotes"
CONFIG_CANVAS_WIDTH   = 960 (Screen resolution width of your device in pixels, no quotes)
CONFIG_CANVAS_HEIGHT  = 480 (Screen resolution height of your device in pixels, no quotes)
CONFIG_TIME_FORMAT    = 12 (12 for AM/PM format, 24 for 24-hour military format, no quotes)
CONFIG_WEATHER_REFRESH_MINS = 15 (Weather API update frequency in minutes, no quotes)

=========================================================================
(3.) Save your custom .html file and upload both the .html and .mp3 (and optional background .jpg) to your FTP.
(4.) Enable the MyPage skill on your device, and ask your device "Alexa, open MyPage"
MyPage will open to the configuration page when first opened. Alternately, you can say "Alexa, open MyPage and show page list"
(5.) In the "Page 1" URL slot, type in the URL to your .html you uploaded to your FTP. You can also open this configuration page on a computer, by going to https://xdream2000.com/alexa/my_page/, and input the 5-digit code from the MyPage configuration screen on your device. You can leave the "Name" slot blank, or give it a name.
(6.) SAVE IT!
(7.) Say "Alexa, open MyPage" and your custom time/weather page should load on your device.
NOTE: The Silk browser on Alexa devices will always show the top bar upon opening a web page. Tap "Full Screen" on the top right to make it go away. But the top browser bar will return if you use the device for something else and then open MyPage again. You can also set up a Routine in the Alexa app to open MyPage on a schedule, or however else you want to use it in a Routine.
(8.) Enjoy! (And consider subscribing to my Patreon!)

