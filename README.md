# flacicon

Apple's hate-hate relationship with Free Lossless Audio Compression (FLAC) is so petty, they don't plumb the meta info 
of flac files for album art to make icons for .falc files.  Fine.  Here's a script that will:
1) accept a directory or a list of files (ala "*.flac")
2) extract the artwork from each flac file or accept an image filename to create an icon.

This is intended for MacOS systems only.  I've used code and examples that work with the default bash included with 
MacOS Ventura.  

flacicon is based on "seticon.sh" in this stackoverflow post: 

https://stackoverflow.com/questions/8371790/how-to-set-icon-on-file-or-directory-using-cli-on-os-x

```
usage: flacicon [-e|-f <imagefile>] <filelist>
        -e                      [e]xtract the artwork from metadata
        -f <imagefile>          use given image [f]ile for icon
        <filelist>              list of input files; takes wildcards                                  
                                or a directory with flac files
```
