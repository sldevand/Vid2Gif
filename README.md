Vid2Gif
======
**Vid2Gif** A simple FFMPEG bash script to encode a video into a GIF.

## Sources
*  [blog.pkh.me](http://blog.pkh.me/p/21-high-quality-gif-with-ffmpeg.html)

## Dependencies
* [FFMPEG](https://ffmpeg.org/)

#### Install ffmpeg with Debian Linux
```
sudo apt-get install ffmpeg
```
## Installation
Just clone this repository into your downloads folder
```
git clone https://github.com/sldevand/Vid2Gif.git
cd Vid2Gif
```
and copy the vid2gif* files into /usr/local/bin
```
sudo cp vid2gif* /usr/local/bin
sudo chmod +x /usr/local/bin/vid2gif*
```

## Usages

#### vid2gif
You can extract the gif from the entire video

```
sudo vid2gif <src/video/file> <dest/file.gif> (<fps>)  <--optional
```

**Note:**
* If you don't give the **fps** argument, ffmpeg takes the video source fps 

#### vid2gif-sample
You can  extract the gif from a video sample
```
sudo vid2gif <src/video/file> <dest/file.gif> <start_time> <duration> (<fps>)  <--optional
```

**Notes:**
* **start_time** and **duration** format is hh:mm:ss.ms (you can be more precise with milliseconds)
* **hh:** and **mm:** are optional.
* If you don't give the **fps** argument, ffmpeg takes the video source fps 

#### Example:
I want my GIF to :
* begin at 12 min 26 sec
* last 5.26 seconds
* 10 frames per second :
```
sudo vid2gif /path/to/video/myVideo.mp4 /path/to/gif/myGif.gif 12:26 5.26 10
```


## License 
* see [LICENSE](https://github.com/sldevand/Vid2Gif/blob/master/LICENSE.md) file

## Thanks
Thanks ubitux for the explanation of this trick
-   [blog.pkh.me](http://blog.pkh.me/p/21-high-quality-gif-with-ffmpeg.html)

