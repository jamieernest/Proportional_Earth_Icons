# Welcome to the guide to make proportional icons on Google Earth!
In this guide I will cover how to make proportional icons in a KML icon in Google Earth. This is useful in multiple ways, such as visualizing bedload size in multiple locations (my use case), population data (check Credits, example of that is used here), and earthquake magnitude data.

## Prerequisites: 
1. Download the template [here](https://github.com/jamieernest/Proportional_Earth_Icons/releases/download/1.0/water_of_leith_bedload_size_2021_4GGA.kml)
2. Coordinates of locations. If you are not sure, just [create](https://www.google.com/maps/d/mp?hl=en&authuser=0&state=create) a Google custom Map. After you finished putting down points click on the three dots next to the title, click on `Export as KML/KMZ`, check `Export as KML instead of KMZ. Does not support all icons.` and click `Download`. The coordinates should be in blocks like this:<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/coordinate%20block.png?raw=true">
3. [Google Earth Pro](https://www.google.com/earth/versions/#download-pro). Google Earth Web doesn't work because it doesn't support KML files getting resources (in our case, the circle) from another website. It would load, but it would show proportional boxes of crosses, not circles.
4. _Optional:_ [Visual Studio Code](https://code.visualstudio.com/). This can be done with any text editor, but it would look much more organized:<br>Normal text editor (in this case, textedit):<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/textedit.png?raw=true"><br>Visual Studio Code:<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/vsc.png?raw=true"><br>Visual Studio Code also has an [extension](https://marketplace.visualstudio.com/items?itemName=jumpinjackie.vscode-map-preview) which allows you to preview your changes (albeit in pins, not circles).<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/extension.png?raw=true"><br>You can open this by pressing `f1` on your keyboard, then finding/typing `Map Preview`.

## Steps:
When you open the file everything may seem intimidating, but don't worry, it's just copy and paste :)<br>
1. Find the average of all results.
2. Find the scale of all results, referring to the average. For example, if the average of all results is 2 units, the scale for 1 units would be 0.5, and the scale for 4 units would be 2.
3. Open the template file.
4. Change the name and description (line 4 - 5) to what you want.
5. In the template, there are 15 sites. If there are too many sites, delete the extra blocks (example below). If you need more sites, make a new line after line 313 and paste this in (repeat as many times as you need):<br>
```xml
    <Placemark>
        <name>Site 1 (14.61cm)</name>
        <LookAt>
            <longitude>-3.4638007</longitude>
            <latitude>55.8197572</latitude>
            <altitude>0</altitude>
            <range>3200000</range>
            <tilt>0</tilt>
            <heading>0</heading>
        </LookAt>
        <styleUrl>#defaultStyles</styleUrl>
        <Style>
            <IconStyle>
                <scale>1.35</scale>
            </IconStyle>
        </Style>
        <Point>
            <coordinates>-3.4638007,55.8197572,0</coordinates>
        </Point>
    </Placemark>
```
6. Scroll down to the first block. You will see different attributes, such as name, longitude, latitute etc... The only attributes we care about are name, longitude, latitude, scale, and coordinates.
7. Change the name of the block to whatever you like. This name will show up next to the circles in the map.
8. Change the scale of the block to the scale of the first result, in relation to the average. You should have this calculated in Step 2.
9. Change the coordinates attributes to the coordinates for the first point, in the format of `longitude,latitude,altitude (should be 0)`
10. Change the longitude, latitude and altitude according to the coordinates you have.
11. Repeat Steps 6-10 for every result.

## Result:
<img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/result.png?raw=true">

## Support or Contact:

Having trouble? Please make an issue on the [repo](https://github.com/jamieernest/Proportional_Earth_Icons) and I will help you ASAP :)

## Credits:
1. [Microsoft](https://www.microsoft.com/) for [Visual Studio Code](https://code.visualstudio.com/) (I still dislike you Microsoft.)
2. [Google])(https://google.com/) for [Google Earth Pro](https://www.google.com/earth/versions/#download-pro) and [Google Maps](https://maps.google.com/).
3. [jumpinjackie (Jackie Ng)](https://github.com/jumpinjackie) for the VSCode Map preview extension.
4. [Template](http://thematicmapping.googlepages.com/population_2005_icons.kmz) I referenced to, and also the [website](https://blog.mastermaps.com/2008/04/making-proportional-symbols-in-kml.html) (this is for population data).
5. Ms Vardy and Set 4GGA of 2020-2021, especially Edward and Edo. Without you all, I would not have the motivation to do this.
6. You for reading this :)