# Adding Extra Tracks

During demuxing Extra tracks can be added with the&#x20;

\--extra args

The folder will be  scan add a simple dictionary list will be created



This is meant for adding for example subtitles that from another mkv that you have extracted

Most keys will have placeholders that you will have to manually change

Additionally some keys will only effect some track types



A extra track should have the following values set if enabled is true

* site\_title
* langcode or language
* the correct type&#x20;

### Changing the order of the tracks

Mediainfo will show you the default order of the tracks

If you need to change this order look into&#x20;

\--track-order on [https://mkvtoolnix.download/doc/mkvmerge.html](https://mkvtoolnix.download/doc/mkvmerge.html)

you can pass this to PT-Muxer like



\--otherargs \\"-- track order \[your args]\\"

### Keys

* langcode: \[string:2 char] used by mkvmerge to set track language. This is used to set the track language in "remux" mode   default=null
* lang: \[string] Translation of langcode to the actual language. This is for convenience, and has no effect on "remux" mode  default=null
* filename: \[string] auto retrieved  name of filename used when scanning dir.
* site\_title : used to set title for mediainfo, set to None for no title. This will affect "remux" mode default=placeholder
* bdinfo\_title :  just the title from bdinfo, changing this value has no effect   default=placeholder
* forced: \[bool] whether to set the forced flag. Also can be set by changing the site\_title to include "forced"



* type: \[string] whether this is an audio, video, sub-track. This value should not be changed as it is used during the "remux" process
* commentary: \[bool] Sets the Commentary flag to yes. Should be used for all audio and subtitle tracks that are commentary
* auditorydesc:\[bool] Turn on for tracks that include auditory descriptions, sets the Visual impaired flag. Applies only to audio tracks
* original: \[bool] Turn on for tracks in the movies original language,set the Original language flag. Applies only to audio tracks
* sdh:\[bool] Turns on the Hearing impaired flag. Applies only to sub tracks
* textdesc: \[bool] For subtitle tracks with text-based descriptions for the visually impaired that can be read via a screen reader. Applies only to sub tracks
* extra\_options:\[string] add extra mkvmerge commands
* default :  default=false
* forced :  default=false
* notes default="Enter you own notes here"
* extra\_options= default=null

#### **Unique Keys**

These keys are unique to this section

* enabled: \[bool] Whether or not to enable this extra track
* type: \[string]: What type of track is this must be Audio,Video, Sub or will be ignored

