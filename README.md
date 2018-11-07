# TileServer-GL initial directory #

This is an example directory for [klokantech/tileserver-gl](https://github.com/klokantech/tileserver-gl/) with custom style and custom data.

![Map screenshot](https://github.com/saveryanov/tileserver-gl-init-directory/blob/master/screenshots/result-example.png?raw=true)

Map data is stored in **data** directory in **mbtiles** format. This file was created via [openmaptiles](https://github.com/openmaptiles/openmaptiles) from [Geofabrik data in pbf format](https://download.geofabrik.de/russia/northwestern-fed-district.html) (all zoom layers, small area of Russia, Saint-Petersburg, Devyatkino metro station).

Map style is stored in **styles** directory. It was created with [Maputnik online editor](http://editor.openmaptiles.org) and based on the "OSM Bright" default style. However some features have been slightly changed: icons are now stored localy and now you can see housenumbers on the map.

## Run ##

Clone this repository:

```git clone https://github.com/saveryanov/tileserver-gl-init-directory && cd tileserver-gl-init-directory```

Run the server with:

```docker run --rm -it -v $(pwd):/data -p 8080:80 klokantech/tileserver-gl```

This will download and start a ready to use container on your computer and the maps are going to be available in webbrowser on localhost:8080.