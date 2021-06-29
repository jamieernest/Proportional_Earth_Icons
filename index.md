# Welcome to the guide to make proportional icons on Google Earth!
In this guide I will cover how to make proportional icons in a KML icon in Google Earth. This is useful in multiple ways, such as visualizing bedload size in multiple locations (my use case), population data (check Credits, example of that is used here), and earthquake magnitude data.

## Prerequisites 
1. Download the template [here](https://github.com/jamieernest/Proportional_Earth_Icons/releases/download/1.0/water_of_leith_bedload_size_2021_4GGA.kml)
2. Coordinates of locations. If you are not sure, just [create](https://www.google.com/maps/d/mp?hl=en&authuser=0&state=create) a Google custom Map. After you finished putting down points click on the three dots next to the title, click on `Export as KML/KMZ`, check `Export as KML instead of KMZ. Does not support all icons.` and click `Download`. The coordinates should be in blocks like this:<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/coordinate%20block.png?raw=true">
3. [Google Earth Pro](https://www.google.com/earth/versions/#download-pro). Google Earth Web doesn't work because it doesn't support KML files getting resources (in our case, the circle) from another website. It would load, but it would show proportional boxes of crosses, not circles.
4. _Optional:_ [Visual Studio Code](https://code.visualstudio.com/). This can be done with any text editor, but it would look much more organized:<br>Normal text editor (in this case, textedit):<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/textedit.png?raw=true"><br>Visual Studio Code:<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/vsc.png?raw=true"><br>Visual Studio Code also has an [extension](https://marketplace.visualstudio.com/items?itemName=jumpinjackie.vscode-map-preview) which allows you to preview your changes (albeit in pins, not circles).<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/textedit.png?raw=true"><br>Visual Studio Code:<br><img src="https://github.com/jamieernest/Proportional_Earth_Icons/blob/gh-pages/extension.png?raw=true"><br>You can open this by pressing `f1` on your keyboard, then finding/typing `Map Preview`.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/jamieernest/Proportional_Earth_Icons/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
