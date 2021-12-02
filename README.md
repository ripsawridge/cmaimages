# cmaimages
I host my images for mountain trips here

Here is the kind of script I use to transfer:

```
!/bin/sh
rsync --exclude '.git' -arvz cmaimages/ \
   mountai8@mountainwerks.org:~/public_html/cmaimages
```

Thumbnails were created with ImageMagick, like so:

```
magick mogrify -resize 800x600 -path thumbs/2009 2009/*.jpg
```

Files from 2005 and before simply have copies of the original file in
the thumbs directories, because in all cases, the thumbs/ directory was
larger than the original year directory!
