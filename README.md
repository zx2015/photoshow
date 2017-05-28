# PhotoShow
Photoshow is gallery software at its easiest, it doesn't even require a database.
Home Page for PhotoShow
http://www.photoshow-gallery.com/

This project customized PhotoShow container.

docker create \
--name=photoshow \
-v <path to pictures>:/opt/PhotoShow/Photos \
-v <path to config>:/opt/PhotoShow/generated/Conf \
-v <path to store thumbs>:/opt/PhotoShow/generated/Thumbs \
-p 80:80 \
zx2015/photoshow

Parameters:
/opt/PhotoShow/Photos             Place to store pictures
/opt/PhotoShow/generated/Conf     Place to store configuration files. PhotoShow will initilized the configuration if the folder is empty
/opt/PhotoShow/generated/Thumbs   Place to store generated Thumbs
