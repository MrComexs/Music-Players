## Work in progress
I will appreciate you feedback about this article. There is going to be a lot of basic mistakes so if you could be so kind and submit a new issue so we can work it out. If you find something confusing don't be afraid to point it out so that I could add more context if needed.

# Music Players
- [Gramophone](#gramophone)
- [Musicolet](#musicolet)
- [Poweramp](#poweramp)
- [Namida](#namida)
- [Samsung Music](#samsung-music)
- [Symphony](#symphony)
- [VLC](#vlc)

## about me
Hi I'm Comexs and I mostly listen to music on my computer but on occasion I listen on my android phone. Most of my music library consists of 16 bit flac with some 24 bit flac as well as some other codecs like mp3, 32 bit float wavpack and one opus track ripped from youtube. At the time of writing, I have 550 tracks in my library. I would perfer to have opus over mp3 but most artist would rather upload a mp3 than any other lossy codec. I'm currently looking into inserting mp3 into ogg containers.

I use the official cli encoder for example flac and wavpack. I used to ffmpeg for this but found better results though very marginal when using own respective codec's cli tool.

### History of my music players choices
#### Android
I have been using Musicolet for the last three-ish years. I have also bought the "Lifetime access" around the time I started to use it. I have been mostly happy with the product but since the purchase I have gain interest in the FOSS movement and I now somewhat regret my decision to purchase the "Lifetime access" for Musicolet not because I see the product as inferior to FOSS music players but because the conflict of interest of my support of the FOSS movement.

I have also used Samsung Music for a year before Musicolet until they added ads.
#### Desktop
My music player of choice on tablet is VLC only because of the great support for landscape orientation.
On windows I'm currently use MusicBee but I'm starting to replace it with foobar2000 when I feel more comfortable with it and on Linux which is where I spend most of my time but I rarely listen to music; I mainly use Harmonoid unless I want to listen to a wavpack file than I have to use mpv since Harmonoid isn't pickup any of my wavpack files.

### How I format metadata in my music library
#### Which metadata editor do I use?
I use a mixture of three apps and some cli tools to edit the metadata of my music library.
- kid3
- MusicBrainz Picard
- ~~MusicBee~~
- foobar2000
- metaflac
- wvtag
- *searching for opus/mp3 ogg metadata editor*

I'm currently using Picard as my default metadata editor for now, though I'm currently very inexperience with the tool the main reason for interest in using the tool is own open source proprietary online metadata music database. I use Kid3 as a backup to embed the more additional images to the file such as if the track has both a single and album artwork. I'm no longer planning to use MusicBee as my default music player for windows so I will replace it with foobar2000 until I find a Linux to windows cross platform music player. I also use metaflac, and wvtag. I plan to automate artwork embedding with local files since I always try to source the highest quality artwork for my music library. I could also use Picard but still very unsure of its capabilities.
##### metadata format
I only put one album artist even its a collaboration. I separate multiple entries in a data field with semi colons `;` but I just learned that you could make a new metadata field with the same value for example you could have two artist field though I should do more research witch metadata schemes support this since I mostly use Vorbis (flac, opus, and mp3?), ID3 (mp3) and APEv2 (wavpack). I like to have multiple artwork embed into my music if the song has some so for example lets say there is a artist that released a single and a some time later in was re-released into a EP/Album/special edition album than I like to attach the the single artwork as well as the album artwork; I do this because some music players support artwork slideshow which is neat. Most of my artwork is JPEG and some PNGs but I have a interest in webp, jpgxl, and most of all avif. I will talk more about these in [future metadata format](#future-metadata-format). I also use the lyrics metadata field but with synced (lrc format non-end-tag format) and non-synced lyrics. I very rarely use the genre field since I don't both bother because of my confusion with all the sub-genres. I don't use the two disc fields unless they have multiple disc.
# reviews
### extra info
This is the name format I use for my music library `Album_artist - Track_number ⌊Title⌉.flac`. I like it because its easy on the eyes for me so I will mentioned in the review section for each app if they are having problems with the filename format. It should be very unlikely to happen since either android has dealt with this or the developers understood that there end user are going to have the most horrendous file name and file folder structure. I don't use any hidden folder in my music library so if that is a use case that you use than you are going to have to do some independent research though I do use blacklist feature if supported which I feel is necessary because of tool like syncthing. I use syncthing to sync my music to my phone. I have also use Trash can file versioning which so there might be some extra tracks that aren't supposed to appears in the apps library if the blacklist is active and set correctly.

#### Codec Info
the 2nd column is the codec support. 
the image column is if the app is how the image.
the metadata column is if it pickups any metadata field other than the image.

flac, opus, and vorbis use the vorbis metadata schemes
wav, and mp3 use ID3v2.3.0
wavpack uses APEv2

For research purposes I'm using two flac files but encoded with libFLAC 1.4.3 one 24 bit and another in 32 bit. I also have a 8 bit mp3 encoded with LAME3.100. I have two opus files with just with the file extension ogg and the other with opus (the only difference is the extension in the file name since they still use the same container). a vorbis ogg file encoded with libogg 1.3.5. A 32 bit float point wav file. And finaly a 32 bit float point wavpack, encoded with wavpack 5.7.0.

all tracks have the same 3000x3000 JPEG image but the two flac files have a extra image to test if the player supports rotating artwork feature

## Gramophone
6.03MB size
GPL 3.0
active devolvement

|  Codec   |     | Image | Metadata |
|:--------:|:---:|:-----:|:--------:|
| flac 24  |  ✔  |   ✔   |    ✔     |
| flac 32  |  ✘  |   ✘   |    ✘     |
|   mp3    |  ✔  |   ✔   |    ✔     |
|   opus   |  ✔  |   ✔   |    ✔     |
|  vorbis  |  ✔  |   ✔   |    ✔     |
| wavpack  |  ✘  |   ✘   |    ✘     |
|   wave   |  ✔  |   ✘   |    ✘     |
### Pros
- Basic codec support
- Very simple theme
- list and grids support (limited)
- Album Artist filter
- synced lyrics support
- metadata viewer
### Cons
- bad blacklist (listed each sub folder)
- no custom library folder
- no black theme
- no rotating artwork support 
- no metadata editor
- makes a `gramophone_favourite.m3u` in music folder. can't set to another location
- The `Filesystem` and `Folders` tabs aren't alphabetize
- there isn't a sort menu in `Filesystem` and `Folders`

## Musicolet
### Pros
### Cons

## Poweramp
### Pros
### Cons

## Namida
I'm personally not a fan of the animations and the theme 

82.26MB
Proprietary License but open source
active devolvement

can't play 32 bit flac but can view the metadata. can't read opus metadata but able to view the image. it can use read images off a wavpack file
|  Codec   |     | Image | Metadata |
|:--------:|:---:|:-----:|:--------:|
| flac 24  |  ✔  |   ✔   |    ✔     |
| flac 32  |  ✘  |   ✔   |    ✔     |
|   mp3    |  ✔  |   ✔   |    ✔     |
|   opus   |  ✔  |   ✔   |    ✘     |
|  vorbis  |  ✔  |   ✔   |    ✔     |
| wavpack  |  ✘  |   ✔   |    ✘     |
|   wave   |  ✔  |   ✔   |    ✔     |
### Pros
- feature rich
- very animated
- unique theme
- youtube playback and downloader
- cross-fade support
- synced lyrics support
- video support
- built in equalizer
- list and grids support
- For you page
- automated playlist
### Cons
- artwork in the menus is low quality 
- very overwhelming
- animations are locked to the software

## Symphony
5.72MB
AGPL 3.0
active but mostly one developer

32 bit flac show up on in the app but skips after a few seconds
|  Codec   |     | Image | Metadata |
|:--------:|:---:|:-----:|:--------:|
| flac 24  |  ✔  |   ✔   |    ✔     |
| flac 32  |  ✘  |   ✘   |    ✘     |
|   mp3    |  ✔  |   ✔   |    ✔     |
|   opus   |  ✔  |   ✔   |    ✔     |
|  vorbis  |  ✔  |   ✔   |    ✔     |
| wavpack  |  ✘  |   ✘   |    ✘     |
|   wave   |  ✔  |   ✘   |    ✘     |
### Pros
- custom scaling
- black theme
- custom tabs
- Basic codec support
- synced lyrics support
- for you tab
- cross-fade support?
### Cons
- no metadata editor or viewer
- no rotating artwork support
- no custom list and grids

## VLC
111MB size
GPL 2.0
very active devolvement

|  Codec   |     | Image | Metadata |
|:--------:|:---:|:-----:|:--------:|
| flac 24  |  ✔  |   ✔   |    ✔     |
| flac 32  |  ✔  |   ✔   |    ✔     |
|   mp3    |  ✔  |   ✔   |    ✔     |
|   opus   |  ✔  |   ✔   |    ✔     |
|  vorbis  |  ✔  |   ✔   |    ✔     |
| wavpack  |  ✔  |   ✔   |    ✔     |
|   wave   |  ✔  |   ✔   |    ✔     |
### Pros
- Great codec support
- Black theme (doesn't work for me)
- video play
- list and grids support (limited)
### Cons
- mostly a video player
- no rotating artwork support
- no metadata editor
- no cross-fade

