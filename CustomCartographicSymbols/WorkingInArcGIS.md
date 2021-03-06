Now you're almost ready to use your pin icon in a map in ArcGIS.

### Setting up the Pin File
ArcGIS requires that we use a .emf (Enhanced Metafile) file, so here's how we do that:
1. If it's not already open, open your pin .svg file that you were just working on in the [Instructions Document](/CustomCartographicSymbols/Instructions.md) in Inkscape.
2. Click the File menu (upper left corner), choose Save As.
3. In the "Save Type As" dropdown menu at the bottom of the Save As dialog, select "Enhanced Metafile (.emf)", and click the Save button to finish.
4. In the EMF Output window that pops up, make sure you check the option to "Convert Text to Paths".

### Load Data
Import the vector data you would like to work with.  
* From this repository's [data folder](/Data): FOSS4G_Locations.zip (locations of all of the FOSS4G conferences zipped... you'll need to unzip it before you can use it).
* From the internet: [Natural Earth Country' 1:110m Cultural Admin-0 Country Boundaries](http://www.naturalearthdata.com/downloads/110m-cultural-vectors) and any other data you would like to add to your map (such as the Admin-1 States & Provinces Natural Earth data).

Order your layers with the countries on the bottom, then the lines, and points on top.  Save your work.

### Using your Pin image
Now we can use our pin in ArcMap
1. Right click on the FOSS4G_Locations in the table of contents, choose Layer Properties.
1. On the Symbology Tab, click the button that has the current symbol for the point (it probably looks like a circle if you haven't changed the default yet).
1. In the Symbol Selector dialog that pops up, click the "Edit Symbol..." button.
1. In the Symbol Property Editor dialog, change the Type drop down to "Picture Marker Symbol".
1. Click the "Picture..." button, then navigate to your .emf file and click "Open".
1. Adjust the size to something larger... I picked 15 from the dropdown for my pin.
1. Click "OK" for all of the 3 dialogs Arc opened.  You should see your pin at all the conference locations!

This method does not allow you to change the color of your symbol through the ArcMap interface.  For single-color icons, such as the National Park icon set, you can change the colors by converting your icons to a font.  Reference: https://gis.stackexchange.com/questions/32271/creating-new-custom-vector-marker-symbol-for-arcmap  This is beyond the scope of this workshop, but I would encourage you to explore this if you're interested now that you have some experience making your own icons.
