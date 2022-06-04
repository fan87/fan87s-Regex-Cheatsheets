## YouTube Video ID Match
### Use case
If you want to check if an URL is a valid YouTube video, and want to extract the video ID, you can use this regex.

### Tested Engines
- ✅ JavaScript
- ⚠️ Java (It should work, but untested)


### Usage
The first captured group will be the Video ID.

### Regex
To test it, you can go [there](https://regexr.com/6n2mm)

`(?:https?:\/\/)?(?:\w*\.)?(?:(?:(?:youtube\.com\/)watch\?v=)|(?:youtu\.be\/))([a-zA-Z0-9_-]{11})(?:(?:(?:&[\w%]*=[\w%]*)|(?:#[\w%]*))*\/?)*`

### Examples
Things that should match:
- `https://youtube.com/watch?v=aaaaaaaaaaa`
- `http://youtube.com/watch?v=aaaaaaaaaaa`
- `https://www.youtube.com/watch?v=aaaaaaaaaaa`
- `https://www.youtube.com/watch?v=aaaaaaaaaaa#test`
- `https://www.youtube.com/watch?v=aaaaaaaaaaa&list=asdfasdfASDFASDF`
- `https://music.youtube.com/watch?v=aaaaaaaaaaa`
- `https://youtu.be/aaaaaaaaaaa`
- `www.youtube.com/watch?v=aaaaaaaaaaa`

Things that shouldn't match:
- `https://youtube.com/watch?v=aaaaaaaaaa+`
- `https://youtube.com/watch?v=aaaaaaaaaaaa`
- `https://github.com/fan87`
- `https://www.youtube.com/watch?v=aaaaaaaaaaa&list`
- `https://www.youtube.com/watch?v=aaaaaaaaaaa&`
- `ftp://www.youtube.com/watch?v=aaaaaaaaaaa`
