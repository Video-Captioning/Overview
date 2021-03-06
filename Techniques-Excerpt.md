# Extract still images from the video

Since our video is nearly two hours long, let's grab an excerpt of just a few minutes, and sample a few frames per second from that excerpt. See the Video Excerpting repository, [Practical-VLC](https://github.com/KarlEdwards/Practical-VLC.git)

#### Parameters

* Input: `~/VLC_stuff/2015bsVriot.mp4`
* Start time: `500` ( seconds from beginning of video )
* Duration: `300` ( seconds )
* Output: `./`  ( current directory )

#### Execution
Putting it all together as follows:

* (Default) fine ratio: 30/3 ---> 10 frames per second
```$ sh excerpt.sh ./data/1_video/2015bsVriot.mp4 ./data/2_images/ 500 300```

* coarse ratio: 30/30 ---> 1 frame per second
```$ sh excerpt.sh ./data/1_video/2015bsVriot.mp4 ./data/2_images/ 500 300 coarse```

yields a series of a few hundred frames from the video, each frame in a file having a name like frame_0####.png

[back](README.md)
