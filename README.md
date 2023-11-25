# ytuh
## (YouTube URL Helper)

A bash script designed to help with handling YouTube URLs 

## Usage
By default, the script takes YouTube channel name (without the @) as input and returns the channel ID.

```
$ ytuh jawed
UC4QobU6STFB0P71PMvOGN5A
```

The `-r` (reverse) option reverses this behavior: the user inputs a channel ID and the script prints the corresponding channel name.

```
$ ytuh -r UC4QobU6STFB0P71PMvOGN5A
jawed
```

The `-f` (feed) option will cause the script to output the RSS feed for the channel provided.

```
$ ytuh -f jawed
https://youtube.com/feeds/videos.xml?channel_id=UC4QobU6STFB0P71PMvOGN5A
```

It should be noted that `-rf` does work as expected, retrieving a feed URL from a channel ID.
While this may seem useless, and it probably is, I saw no reason why I shouldn't make it work on the off-chance that it might improve someone's workflow, somehow.
