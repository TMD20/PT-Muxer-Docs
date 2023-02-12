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

