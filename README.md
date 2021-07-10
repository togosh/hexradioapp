# hexradioapp
Livestream of the HEX cryptocurrency Telegram voice chats

https://hexradio.app/

HEX Chat - https://t.me/HEXcrypto    
Pulse Chat - http://t.me/PulseChainCom

# Setup

- 2nd computer with Windows 10

- Disable screen lock and sleep   
Power & sleep Settings >>> Screen: Never,  Sleep: Never

## Software

- Telegram   
https://telegram.org/   

- OBS (Open Broadcaster Software)   
https://obsproject.com/   

- Restream.io (Multistream to Youtube, Twitch, Dlive, etc)   
https://restream.io/   

## OBS

- OBS Stream tab    
OBS >> File >> Settings >> Stream (I use Restream)    

- OBS Video tab   
OBS >> File >> Settings >> Video   
1280x720 base and output, Bicubic downscale filter, FPS 30   

- OBS Output tab   
OBS >> File >> Settings >> Output   
Output Mode Simple   
Video bitrate 3000 Kbps   
Audio Bitrate 160   

## VB Audio Virtual Cable

[Isolate the capture of the Telegram audio, and funnel it into OBS] 

- Download & Install   
https://vb-audio.com/Cable/ (Restart PC?)   

- Computer "Sound Settings" >>> Input Device >>> CABLE Output (VB-Audio Virtual Cable)   

- Computer "Manage Sound Devices" >>> Recording >>> Right click Enable Stereo Mix   

- Telegram    
--- Join Voice Chat >>> Settings >>> Speakers: CABLE Input, Microphone Stereo Mix   

- OBS Audio tab   
OBS >> File >> Settings >> Audio   
--- Global Audio Devices >>> Desktop Audio >>> CABLE Input   

- OBS Audio Mixer window (main window)   
--- Click Gear icon >>> Properties >>> Device: CABLE Input   
--- (OPTIONAL) Click Gear icon >>> Filters >>> Click plus (+) sign >>> Noise Supression   

## Window Capture

- OBS Sources   
--- Sources window >>> Click plus (+) sign >>>    
Window Capture >>> Scale size by moving the sources corners in OBS   
Crop the window by holding ALT key and moving its corners/edges  

Window Capture (HEX Telegram, Pulse Telegram, Uniswap.vision Price Chart)   

# Extra

- Spectralizer (Sound Visualizer) plugin   
https://obsproject.com/forum/resources/spectralizer.861/   
(C:\Program Files\obs-studio\obs-plugins\64bit)   
Mode: Bars, Audio Source: Cable Input, Filter:  Monstercat, Color: #eea820   
Bar width: 6, Bar height: 110, Bar spacing: 2, Gravity: 0.90, Detail: 32 bins   

- HEXradiobot   
--- C# program   
https://github.com/togoshige/hexradiobot    
--- OBS websocket plugin   
https://obsproject.com/forum/resources/obs-websocket-remote-control-obs-studio-from-websockets.466/   
(C:\Program Files\obs-studio\obs-plugins\64bit)   

# TODO

- add UTC clock?   
https://www.youtube.com/watch?v=SgqT58peTQs   
https://obsproject.com/forum/threads/new-i-am-looking-for-a-date-time-plugin-display.135757/   
(Requested by multiple people, to help with making clips)   

- stream audio     
https://medium.com/@richard534/uploading-streaming-audio-using-nodejs-express-mongodb-gridfs-b031a0bcb20f  

