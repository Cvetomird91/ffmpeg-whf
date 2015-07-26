Run as root to compile FFMpeg with the following Codecs:

- Xvid 
- Lame MP3 Codec  
- FAAC 
- OpenCore AMR Codec 
- OGG 
- Vorbis 
- Theora 
- x264 
- LibVPX 

Preparation for Debian-based systems: 

### sudo apt-get install automake gcc make aclocal autoconf yasm nasm git wget curl libtool g++

Preparation for RHEL-based systems:

### sudo yum install make automake autoconf yasm nasm git wget curl gcc libtool gcc-c++

The script has been tested on Debian Wheezy 7.8 and CentOS 6.6. 

Things to be added:

- "garbage collection" for downloaded codecs' source code tarballs 
- colorful output for the different steps 
- normal mode with reduced output from compilation steps
- debugging mode with full output from compilation steps 
- options for choosing inbetween different AAC implementations (FAAC, FDK-AAC, libvo-aacenc etc). The default is FAAC. 
- function to check if tarballs are taking too much to download and reattempt if this is the case 
- implement check for compile-time exit statuses

Here are some examples for testing FFMpeg performace with FAAC: 
https://trac.ffmpeg.org/wiki/Encode/AAC

A post on AAC implementations: 
http://spectralhole.blogspot.de/2010/12/androids-stagefright-aac-encoder-or.html
