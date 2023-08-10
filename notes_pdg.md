# FFMPEG

install ffmpeg (via imagemagick or ffmpeg)

add to houdini.env

    PDG_IMAGEMAGICK = "C:\Program Files\ImageMagick-7.1.0-Q16-HDRI\magick.exe"
    PDG_FFMPEG = "C:\Program Files\ImageMagick-7.1.0-Q16-HDRI\ffmpeg.exe"

### ISSUE

change 'Frame List File' parameter to a local directory that works.

speed. Running an opengl node natively is a lot faster than via PDG... after tweaking settings and reading on cgwiki, something that helps:

    Change 'Cook Type' to 'Services'
    Turn on 'Service' by drop-down menu from 'Tasks' ---> 'PDG Services'.
    On the ropfetch node remember to tick 'Use ROP Fetch Service'

    still some issues cooking certain frames... 