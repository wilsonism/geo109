# Geography 109

# Mapping 4: Introduction to QGIS: Part 1

This exercise involves a mapping process commonly used by professional cartographers. As such, you’ll use with data in new ways—be patient! By engaging more deeply with data, you’ll start to understand the moving parts of making digital maps that are often hidden from their users.

In particular, this assignment will introduce data preparation in Microsoft Excel, and visualization in QGIS, a free and open-source (FOSS) software. The 3-part assignment will be completed over the three recitation sections. **Before section** week 6, download QGIS to your computer. In section, you will import county geometry. Second, during week 6, you will download tabular data from FactFinder2 and use Excel to clean the data.

### This assignment will take three recitation sections to complete; therefore it is crucial that you attend each recitation and arrive on time.

**Due:** Submitted via Canvas by **11:59PM Friday of Week 8, March 4th**

**Note:** You must come to recitation week 6 with QGIS installed.

Part 1 questions must be answered and shown on your screen at the beginning of section Week 7

You will receive points in section for having these parts done. Be conscious of saving and storing your data, either on a thumbdrive, space you know is secure on the UK drive, on cloud storage, or your laptop. It is your responsibility to save your data securely.

### Grading and Deliverables 

The assignment is worth 50 points. Grading will be based on a Word document that you will upload to Canvas during Week 11. This document should include:

1.  Your two exported maps (20 points),

2.  Your responses to the questions in each part (30 points)

**Due:** Submitted via Canvas by **11:59PM Friday of Week 8, March 4th**

## Part 1. Importing Geospatial Data

1. Now that you’ve successfully installed QGIS, it’s time to download some geospatial data. Navigate to http://census.gov/cgi-bin/geo/shapefiles2010/main. Under “Select a layertype,” choose “Counties (and equivalent)” and click submit.

![Image28](images/Image28)

2. Under the 2010 dropdown menu (not the 2000 menu below), select Kentucky and click Download.

![Image28](images/Image28)

3. The shapefile you just downloaded is in a compressed folder – a ZIP file – that you must _extract_. Use the technique you learned in M2, being sure to extract _all_ the files, and save themto somewhere easy to find again, like a folder on your desktop made for this purpose.(Remember that the shapefile is actually 5 different files. All of these files are necessary components of the shapefile’s data structure. They must all stay in the same folder or the filewill not work correctly.)

![Image28](images/Image28)

![Image29](images/Image29)

4. Open QGIS. The interface should look familiar, after learning ArcGIS. The two platforms are fairly similar and ‘think’ in the same way (mostly).

5. Click “Add Vector Layer” on the left side of the screen. In the Add Vector Layer dialogue box, click the “Browse” button to locate your shapefile.

![Image36](images/Image36)

![Image33](images/Image33)

6. Locate the folder that contains your shapefile and click the file ending in “.shp.” **Note: this is potentially confusing as there are other files that also have the .shp extension (e.g.,shp.xml)** and sometimes the extension will be hidden. Take a close look; you may have toexperiment a bit before you find the right file. Click “Open”, and “Open” again in the “Add vector layer” dialogue box.

![Image45](images/Image45)

Congratulations; you’ve just made a map in QGIS! Your shapefile should now be displayedin the map window and in the QGIS list of active layers.

![Image28](images/Image28)

7. Open the attribute table of the layer: you will see this option when you right-click the layer. You can use the information in here to answer Question 2.

![Image57](images/Image57)

### Part 1 Questions

Respond to each of the following questions. Make sure you provide evidence for your claims, in 150 to 300 words for question 1. For question 2 you can also provide an explanation of how you came up with your percentage.

1. What does it mean to say that QGIS is free and open-source software (FOSS)? What are the implications for ‘expert’ cartography and access to mapmaking technology? Do some research – the index of your Crampton textbook is a good place to start. **Cite Crampton**.

2. How much of Bourbon County is under water? Use the attribute table to find **this percentage**. Hint: ALAND10 and AWATER10 will be helpful here. If you are not sure what these variable names mean, try a Google search. Note that these attributes are given in units of square meters.

**_You will continue with Part 2 of the lab in Week 6._**
