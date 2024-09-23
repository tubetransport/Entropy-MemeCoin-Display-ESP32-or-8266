# Entropy-MemeCoin-Display-ESP32-or-8266
This program will fetch the $ENT price from a public API every 60secs and Display it on the SSD1306 LCD.

I created this fun little project while patiently waiting for my spot as a miner of $ENT, a hilarious memecoin. You can find the details at https://justentropy.lol
Since they use ESP32 Dev Boards for the "mining" I thought I would use the wait time to improve my coding skills on the ESP boards. I prevously wrote some code to display DOGE Coin price,I figiured it would be easy do do same for $ENT. Turns out I was wrong. After taking a few weeks to learn JSON, I was able to get it working. Remember I'm just an amature coder, dont hate my crap code! Sugestions welcome. 

To all you entropy "miners" in waiting: this is just a fun project to help you learn the in's and out's of programming the ESP32 you bought for mining. Enjoy!
Perhaps if the @entropy Devs like it, they will add to the "miner" code. Hope you all like the custom bmp!

For any serious miners: The skills I gained playing with these boards, and some good practice in the Linux world, led me to a much more difficult task, unbricking some KS0 Ultras. I'm happy to report the KS0's are working flawlessly. Maybe try my hand at overclocking them next??? 

Hardware:
-1x ESP32 or ESP8266 Board. ($9 on Amazon)
-1x SSD1306 LCD Display (5 for $14.99 on Amazon) 
-1x Package of Female to Female jumper wire - only need 4 total strands (120 Pack on Amazon $4.99)
-USB Data Cable C or A depending on your board. Make sure you get an actual data cable not a simple charge cable.
-Programming software of your choice. Arduino IDE is free and easy to use.

Instructions:
1. Copy either the ESP8266 or ESP32 Code from the respective repostiory on the left <------
2. Connect the VCC Pin of the Display to 3v Pin on ESP Board
3. Connect GND Pin on Display to any GND pin on ESP Board
4. Connect SCL Pin on Display to SCA Pin on Board. (look at board instructions for pin assigment. Usually D1 on 8266 and usually P22 on ESP32).
5. Connect SDA Pin on Display to SDA Pin on board. (look at board instructions for pin assigment. Usually D2 on 8266 and usually P21 on ESP32).
6. Connect Board to your computer with USB DATA cable.
7. Paste Code you copied above into Programming software of your choice
8. Edit Line #22 to replace "YOUR SSID" with your wifi network SSID name. ie. "My Home WiFi Network"
9. Edit Line #23 to replace "YOUR PASSWORD" with your Wifi network password. ie. "914Shoes"
10. Complie and upload to the Board!

If you get it working post your success on my Discord: https://discord.gg/XhtnnDwf

Whats next:
Add LED Blink (Maybe color?) each time the price is fetched. 
Add support for multi color LCD
Make Phone app to program Wifi credentials for easy beginner setup. 
Annimation??
