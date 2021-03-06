What is QMapControl?
====================

QMapControl is a Qt/Qtopia widget which enables your (mobile) applications to
use map data. Simply add the widget to your application, have a look at the API
and start developing a fancy geospatial (mobile) application.

With QMapControl you can use different map providers, like OpenStreetMap or
several WMS-Servers. Then you can modify the view of your QMapControl, writing
a location based application when having a GPS receiver or just browse the
maps. It is possible to have more than one layer, so you can mix maps from
different servers. To enrich the maps you can draw your own object to
coordinates.

Feature list:
- Compatible with multiple map providers (Tile server and WMS server)
- Draw custom objects into maps (lines, points, images, even other Qt widgets!)
- Objects can be added to any coordinate
- Control elements can be added to QMapControl´s layout
- Added objects emit signals on clicks
- The map navigation is customizable (using styles and/or keys)
- GPS parser included for reading gllin output
- Tested on the FIC Neo1973, Nokia N900 (and Linux/Windows)

Compiling the sample application for i386:
==========================================
The folder "Samples" contains several sample applications. They come with .pro files and are ready to build. To do so, just run
- qmake
- make
This will build all sample applications. The binaries can be found in the bin folders of the sample.


Compile the samples for ARM (Neo or Greenphone):
================================================
- cd Samples
- cd Citymap (or any other sample application)
- qtopiamake -project "QT+=network"
- qtopiamake
- make

this will overwrite your .pro files, you can recreate them by calling "qmake -project "QT+=network"

This project hosted on sourceforge: http://sourceforge.net/projects/qmapcontrol/
The project�s website: http://www.medieninf.de/qmapcontrol
