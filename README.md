# cmaimages
I host my images for mountain trips here

Here is the kind of script I use to transfer:
  
    !/bin/sh
    cd
    rsync --exclude '.git' -arvz cmaimages/ \
        mountai8@mountainwerks.org:~/public_html/cmaimages

