# WebAudio
WebAudio is a 2,8 KB audio libary for javascript.
It has support for:
 - lazy loading
 - looping
 - time tracking
 - sound fading
 
 Thats's it :)
 
 ## Methods
 ####Create instance
 ```javascript
const media = new WebAudio(mp3 file);
```
####Set looping
 if the file should repeat on finish
 ```javascript
media.setLooping(boolean);
```

####Play
Start the media
 ```javascript
media.play();
```

####Set time
Jump to a time stamp (seconds)
 ```javascript
media.setTime(int seconds);
```

####Get time
Get the current time stamp (in seconds)
 ```javascript
media.getTime();
```

####Set volume
Set the volume (range is [1 - 100])
 ```javascript
media.setVolume(int volume);
```

or fade to volume, the delay is the fade duration in miliseconds
 ```javascript
media.setVolume(int volume, int delay);
```

####Pause
Stops the sound (but can be resumed)
 ```javascript
media.pause();
```

####Destroy
Destroy and remove the sound from memory
 ```javascript
media.destroy();
```

####File Status
 check if the file is still loading (returns bolean)
 ```javascript
media.isLoading
```

####Sound status
 Check if the file is playable (the file does not have to be completely loaded)
 ```javascript
media.isPlayable
```