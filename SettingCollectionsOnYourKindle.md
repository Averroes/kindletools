# Setting Collections On Your Kindle #

## Introduction ##

The Kindle device does not recognize folder structure of your books. This means that if you arrange books in directories, when opening the home page in Kindle, they will be all put at one place probably sorted by last visited. Kindle has its own system to manage groups called collections. A collection is with depth 1, which is you can have books in only one subdirectory in your documents.

Managing collections through the device itself is very annoying and uncomfortable and if you have hundred books in different sections it is a time consuming task. Also if you have not registered your Device in Amazon the functionality of setting collections is turned off.

## Creating Your Own collections.json ##

Kindle manages collections through a file:
```
<kindle-device>/system/collections.json 
```
The script collgen in Kindle Tools project is aimed at generating such file by parsing a book path. It is recommended this path to be:
```
<kindle-device>/documents/
```

The steps to create and load collections are:

  1. Plug in kindle device;
  1. Run:
```
python collgen.py -d "<kindle-device>/documents" -o "<kindle-device>/system"
```
  1. Plug out kindle device;
  1. In your kindle's menu go to Settings, then click your options key again and choose Restart. This will reboot the Kindle's OS and will reload collections from the generated file;
  1. After reboot go to the sorting bar which is on top. You go there by clicking the move up key several times;
  1. Sort books by collections;
  1. That's it - you see only your collectoins;