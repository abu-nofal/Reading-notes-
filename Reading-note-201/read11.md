# Images 

The `<img>` tag is used to embed an image in an HTML page.

Images are not technically inserted into a web page; images are linked to web pages. The` <img>` tag creates a holding space for the referenced image.

The` <img>` tag has two required attributes:

src - Specifies the path to the image
alt - Specifies an alternate text for the image, if the image for some reason cannot be displayed
Note: Also, always specify the width and height of an image. If width and height are not specified, the page might flicker while the image loads.

Tip: To link an image to another document, simply nest the `<img>` tag inside an `<a>` tag (see example below).


Attribute |Value 
----------|--------
alt       |	text
src       |URL
height  | pixels 
width | pixels


## HTML `<audio>` Tag
> Definition and Usage

The `<audio>` tag is used to embed sound content in a document, such as music or other audio streams.

The `<audio>` tag contains one or more `<source>` tags with different audio sources. The browser will choose the first source it supports.

The text between the `<audio>` and `</audio>` tags will only be displayed in browsers that do not support the `<audio>` element.

There are three supported audio formats in HTML: MP3, WAV, and OGG.



Attribute | Value 
-----------|--------
autoplay  | autoplay(Specifies that the audio will start playing as soon as it is ready)
controls  | controls (Specifies that audio controls should be displayed (such as a play/pause button etc))
loop | loop (Specifies that the audio will start over again, every time it is finished) 
src |Url 



## HTML` <video>` Tag

Definition and Usage
The `<video>` tag is used to embed video content in a document, such as a movie clip or other video streams.

The `<video>` tag contains one or more` <source>` tags with different video sources. The browser will choose the first source it supports.

The text between the `<video>`and `</video>` tags will only be displayed in browsers that do not support the `<video>` element.

There are three supported video formats in HTML: MP4, WebM, and OGG.

Attribute | Value 
-----------|--------
autoplay  | autoplay(Specifies that the audio will start playing as soon as it is ready)
controls  | controls (Specifies that audio controls should be displayed (such as a play/pause button etc))
loop | loop (Specifies that the audio will start over again, every time it is finished) 
src |Url 
height| 	pixels
poster | URL(Specifies an image to be shown while the video is downloading, or until the user hits the play button)
