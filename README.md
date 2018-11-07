# TileServer-GL initial directory #

This is an example directory for [klokantech/tileserver-gl](https://github.com/klokantech/tileserver-gl/) with custom style and custom data.

Map data is stored in **data** directory in **mbtiles** format. This file was created via [openmaptiles](https://github.com/openmaptiles/openmaptiles) from [Geofabrik data in pbf format](https://download.geofabrik.de/russia/northwestern-fed-district.html) (all zoom layers, small area of Russia, Saint-Petersburg, Devyatkino metro station).

Map style is stored in **styles** directory. It was created with [Maputnik online editor](http://editor.openmaptiles.org) and based on the "OSM Bright" default style. There are small differences: the housenumbers were added and the icons were stored in local folder.

## Run ##

1. Clone this repository ```git clone https://github.com/saveryanov/tileserver-gl-init-directory && cd tileserver-gl-init-directory```
2. Run the server with ```docker run --rm -it -v $(pwd):/data -p 8080:80 klokantech/tileserver-gl```