# Geography 109:<br>Digital Mapping<br>Mapping 2: Introduction to ArcGIS Pro

University of Kentucky
<br>Matthew W. Wilson

In this exercise, you will bring in, and edit the design of, a map of the commonwealth of Kentucky to become familiar with the basic functions of Esri’s ArcGIS Pro, an industry-standard geographic information system (GIS). After completing this assignment, you will have 1) the ability to navigate ArcGIS Pro and 2) a basic understanding of the file and data structures used by ArcGIS Pro.

**Note:** There are xx steps in this assignment.

## Grading.

The assignment is worth 30 points, based on a Word document (or PDF) you will upload to Canvas containing:
1. Three screenshots: the unstyled Kentucky layer, the 'ugly map', and your much-improved 'attractive' map. Paste these three images into your Word document (15 points).
2. Responses to the three questions in the assignment (15 points).

Consult the [syllabus schedule](../syllabus.md#viii-schedule) for the due date of this assignment. **Note:** Late submissions will be penalized, as discussed in the syllabus.

**Note:** This assignment assumes that you are using ArcGIS Pro in the teaching lab (CB313). We recommend completing the lab in one sitting.

## Instructions.

1. Before you open ArcGIS Pro, there are some steps you can take to make it easier to stay organized. In a simple project like this one, organization may seem unimportant, but it is never too early to start thinking about directory structures (i.e., which things go in which folders). First, right-click your desktop and select New > Folder. Name this new folder “GEO109_M2".

2. Open your new folder. You will now create a folder within a folder. Right-click anywhere in your empty folder, select New > Folder, and name the new folder “data”. You now have a general project folder (GEO109_M2) and a subfolder for data files (data).

3. Download the [geo109m2_ky_shapefile.zip](assets/data/geo109m2_ky_shapefile.zip) file to your GEO109_M2/data folder. After it finishes downloading, locate the file (this should be easy to do, as your new folder is on your desktop). Right click on the ZIP file, and select 7-Zip > Extract Here.

4. You’ll see that five files have been extracted from the ZIP file. Esri, the company that owns ArcGIS Pro, developed the shapefile as a way of storing spatial data. It includes location, shape, and attributes. A shapefile is always made up of at least four files that work together like a little basketball team. **Although only one has the .shp extension, if you do not extract them all, or you delete any, it will not work.**

<!---
Need to update the instructions below for ArcGIS Pro. 
--->
5. Open ArcMap. The “Getting Started” screen will appear. Create a new map using the “Blank Map” template (it should be selected by default).

6. Once you have a blank map, click the “add data” button. Many of the buttons are intuitive: even if we didn’t tell you where they were, you would be able to figure it out. This one has a big plus sign.

7. The program will ask you where to find the data. Arc is a little quirky – it doesn’t just let you add any old file. First, you must connect Arc to the folder that contains your project. Find the “Connect to Folder” button at the top of the dialogue box.

8. Select your project folder. This will connect Arc to your project folder, after which ArcMap will be able to access any file within it.

9. Navigate into your Data folder, select your shapefile, and click “Add.” Note the differences between the five files on your desktop, and the single one that appears when you connect to the desktop from ArcMap!

10. Congratulations! You’ve just made your first map. Take a screenshot.

11. Now you get to change how it looks. This map of Kentucky is called a “layer” and it is the only layer you currently have. Go into the “layer properties” of this layer by right-clicking the layer and scrolling to “layer properties” or double clicking the layer. Explore the different menu tabs in this dialogue box to get a sense of the different things you can do to each layer.

12. Now go to the “Symbology” tab and explore your options here. Below is an example of a bad map choice; I chose the mangrove pattern, made the fill purple, then removed the outlines (so you can no longer see the census tracts).

13. Make your own ugly map; and make it even worse. We’re going to change the background color. Go to View > Data frame properties. Now we are changing not just the layer, but the whole map. Once in properties, go to the “frame” tab, and choose your background color. Return to the layer properties screen (see step 5). Change the layer’s symbol fill color and outlines, as well as the map background to make your own ugly map. Screenshot it!

14. You’ve put some work into making your map ugly... it would be a pity to lose it! Select “Save As” from the File dropdown menu. Save it to your project folder, and name it “M2.mxd”. You’ve just saved an ArcMap project file, or an .mxd.

15. Now go back into the “Symbology” tab and fix it. Pick a fill and outline color of your choice, adjusting line weight and anything else you would like. Change the background color (your choice; white is fine). Capture a screenshot of your attractive map.

16. In a Word document, include your three screenshots, and answer these three questions in about a paragraph each. Reference readings and material covered in lecture and recitation:
* Q1. Explain choices for your maps; what made one bad and the other good? Think about who your audience might be, and issues of readability as well as aesthetics. There is no wrong or right map, as long as you can think through and defend your choices. (Think about Krygier & Wood, Ch. 2: What’s Your Map For?)
* Q2. What is a Shapefile? Who was it developed by, and what does it do? You don’t have to be too technical, just write your observations from this lab. Feel free to search online to help clarify things, though you should be careful to cite your sources.
* Q3. Write a short review of ArcMap. Now that you’ve made a map using Google My Maps, you can compare issues of cost, accessibility, ease, interface, design, and to some extent, what the different mapping programs allow you to do. You might think about expert/amateur mapping (See Crampton, Ch. 1 and 2).

17. Upload a Word document or PDF to Canvas. This document must include your three screenshots and your response to the prompt.