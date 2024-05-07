## Work in progress
I will appreciate you feedback about this article. There is going to be a lot of basic mistakes so if you could be so kind and sumbit a new issue so we can work it out. If you find something confusing don't be afraid to point it out so that I could add more context if needed.

# Music Players
- [Musicolet](#Musicolet)
- [Poweramp](#Poweramp)
- [Gramophone](#Gramophone)
- [Samsung Music](#Samsung-Music)

## about me
Hi I'm Comexs and I mostly listen to music on my computer but on occasion I listen on my android phone. Most of my music library conists of 16 bit flac with some 24 bit flac as well as some other codecs like mp3 and 32 bit float wavpack. At the time of writing, I have 550 tracks in my library. I would perfer to have opus over mp3 but I don't have any opus track in my library because it would be a fruitless endeavor to re-encode a mp3 to opus. I'm currently looking into inserting mp3 into ogg containers.

I use the official cli encoder for example flac and wavpack. I used to ffmpeg for this but found better results though very marginal when using own respective codec's cli tool.

### History of my music players choices
#### Android
I have been using Musicolet for the last three-ish years. I have also bought the "Lifetime access" around the time I started to use it. I have been mostly happy with the poduct but since the purchase I have gain interest in the FOSS movement and I now somewhat regret my decision to purchase the "Lifetime access" for Musicolet not because I see the poduct as inferior to FOSS music players but because the conflict of interest of my support of the FOSS movement.

I have also used Samsung Music for a year before Musicolet until they added ads.
#### Desktop
My music player of choice on tabet is VLC only becacuse of the great support for landscape orientation.
On windows I'm currently use Musicbee but I'm starting to replace it with foobar2000 when I feel more comfortable with it and on linux which is where I spend most of my time but I rarely listen to music; I mainly use Harmonoid unless I want to listen to a wavpack file than I have to use mpv since Harmonoid isn't pickup any of my wavpack files.

### How I format metadata in my music library
#### Which metadata editor do I use?
I use a mixture of three apps and some cli tools to edit the metadata of my music library.
- kid3
- MusicBrainz Picard
- ~~Musicbee~~
- foobar2000
- metaflac
- wvtag
- *searching for opus/mp3 ogg metadata editor*

I'm currently using Picard as my default metadata editor for now, though I'm currently very inexperience with the tool the main reason for interest in using the tool is own open source proparatary online metadata music database. I use Kid3 as a backup to embed the more additional images to the file such as if the track has both a single and album artwork. I'm no longer planning to use Musicbee as my default music player for windows so I will replace it with foobar2000 until I find a linux to windows cross platform music player. I also use metaflac, and wvtag. I plan to automate artwork embeding with local files since I always try to source the highest quality artwork for my music library. I could also use Picard but still very unsure of its capabilites.
##### metadata format
I only put one album artist even its a collaboration. I separate multiple entries in a data field with semi colons `;` but I just learned that you could make a new metadata field with the same value for example you could have two artist field though I should do more research witch metadata schemes support this since I mostly use Vorbis (flac, opus, and mp3?), ID3 (mp3) and APEv2 (wavpack). I like to have multiple artwork embed into my music if the song has some so for example lets say there is a artist that released a single and a some time later in was re-released into a EP/Album/special edition album than I like to attach the the single artwork as well as the album artwork; I do this because some music players support artwork slideshow which is neat. Most of my artwork is jpg and some pngs but I have a interest in webp, jpgxl, and most of all avif. I will talk more about these in [future metadata format](#future-metadata-format). I also use the lyrics metadata field but with synced (lrc format non-end-tag format) and non-synced lyrics. I very rarely use the genre field since I don't both bother because of my confusion with all the sub-genres. I don't use the two dics fields unless they have multiple disc.
### reviews
#### extra info
This is the name format I use for my music library `Album_artist - Track_number ⌊Title⌉.flac`. I like it because its easy on the eyes for me so I will mentioned in the review section for each app if they are having problems with the filename format. It should be very unlikely to happen since either android has delt with this or the developers understood that there end user are going to have the most horrentdous file name and file folder structure. I don't use any hidden folder in my music library so if that is a usecase that you use than you are going to have to do some independent research though I do use blacklist feature if supported which I feel is necessary because of tool like syncthing. I use syncthing to sync my music to my phone. I have also use Trash can file versioning which so there might be some extra tracks that aren't supposed to appears in the apps library if the blacklist is active and set correctly.
