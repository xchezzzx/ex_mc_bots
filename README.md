# Minecraft bot stress tester
🤖 A simple open source app written in Java used for stress testing Minecraft servers with bots (fake players).  
💥 It can be also used to test plugins or minigames.  
✔️ The MC version of the bots is 1.19.1 (supports 1.19.2).  
For older MC versions please look in the [releases](https://github.com/crpmax/mc-bots/releases " releases").

## 🆒 Features
- ✅ Connect as many bots as you want
- ✅ Use SOCKS4 or SOCKS5 proxies from file or URL
- ✅ Receive colored or noncolored chat
- ✅ Set connection delay
- ✅ Set message or command on join
- ✅ Generate random or real looking nicknames or load from file
- ✅ Online (premium) account support with login using Microsoft OAuth - only for migrated accounts

## 📖 Usage
Minimal Java version: 8  
Use of pre-compiled jar from [releases](https://github.com/crpmax/mc-bots/releases " releases"):  
`java -jar mc-bots.jar -s <server address> [arguments]`  
When running, you can write a chat message to the terminal to send it by all bots.

## 🧪 Example
`java -jar mc-bots-1.2.4.jar -s 192.168.0.189:25565 -p BOT_ -d 4000 5000 -c 30 -r`  
This will connect 30 bots to server at 192.168.0.189:25565 with delay 4000-5000 ms and will use real-looking nicknames prefixed with BOT_

<img src="https://imgur.com/XWcckas.png" title="Connected bots" width="350px"/>
<img src="https://imgur.com/CvJq1Io.gif" title="Sending chat message by bots" width="350px"/>


## ⚡ Options
`-c <count>` The count of bots to connect, default is 1  
`-d <min> <max>` Set the minimum and maximum connection delay range in ms, default is 4000-5000  
`-j <message>` The message or command to send on join, does not work with `-m` or `-x` option  
`-p <prefix>` Custom bot nickname prefix eg. `BOT_`  
`-r` Generate real looking nicknames instead of random ones  
`-n` Do not use color in terminal - useful when the terminal does not support it  
`-m` Minimal run - do not use any listeners, will not receive chat, useful for large amounts of bots  
`-x` The most minimal run - No listeners, no control, no chat - useful for large amounts of bots for better performance  
`-t <type>` Set proxy type - SOCKS4 or SOCKS5  
`-l <path>` Set proxy list file  
`-g` Try to simulate gravity by falling down  
`-o` Use online (premium) account (login with Microsoft OAuth)  
`-ar <delay>` Set auto-respawn delay (default is 100 ms, set to -1 to disable)  
`--nicks <file>` Set nicknames file  

## ⚠ DISCLAIMER
**This app is made for educational and testing purposes only.  
This app can be used like spambots.  
I am not responsible for any abuse.**
