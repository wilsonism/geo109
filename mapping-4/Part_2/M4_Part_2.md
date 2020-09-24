# Geography 109:<br>Digital Mapping

# Mapping 4: Introduction to QGIS: Part 2

> [Mapping 4](../README.md) - [Install QGIS](../Install_QGIS/M4_Install_QGIS.md) - [Part 1](../Part_1/M4_Part_1.md) - [**Part 2**](M4_Part_2.md) - [Part 3](../Part_3/M4_Part_3.md)

___

This exercise involves a mapping process commonly used by professional cartographers. As such, you’ll use data in new ways—be patient! By engaging more deeply with data, you’ll start to understand the moving parts of making digital maps that are often hidden from their users.

In particular, this assignment will introduce data preparation in Microsoft Excel and visualization in QGIS, a free and open-source software (FOSS). The 3-part assignment will be completed over the three labs. In Week 6, you imported county geometry. In Week 7, you will download tabular data from the US Census and use Excel to clean the data. In Week 8, you will join the tabular data to the county geometry and produce choropleth maps similar to those produced by Social Explorer in Mapping 3. Take these timelines seriously, otherwise you’ll have trouble completing the assignment. 

### This assignment will take three labs to complete; therefore it is crucial that you attend each lab and arrive on time.

**Due:** Consult the [syllabus schedule](../../syllabus.md#viii-schedule) for the due date of this assignment.

**Note:** You must come to lab week 6 with QGIS installed.

Be conscious of saving and storing your data, either on a thumbdrive, space you know is secure on the UK drive, on cloud storage, or your laptop. It is your responsibility to save your data securely.

### Grading and Deliverables 

The assignment is worth 50 points. Grading will be based on a Word document that you will upload to Canvas. This document should include:

1.  Your two exported maps (20 points),
2.  Your responses to the questions in each part (30 points)

**Note:** Tips for Working with Excel are listed after Step 10. I recommend reading them before getting started, but don’t get hung up on them if they don’t help you; they’re optional. **Do, however, save your work as you go along, and consider bringing a thumb drive to section.**

## Part 2. Downloading and Cleaning Census Data

1. Go to [http://data.census.gov](http://data.census.gov). Click on **_Advanced Search_**.

2. Once the advanced search interface appears, click on **_Geography_** along the left side of your screen.

3. Under **_GEOGRAPHY_** choose **_County_** and then select the state of **_Kentucky_**. Check **_All counties in Kentucky_**. You’ve now specified that you’re interested in county geographies, specifically those within the state of Kentucky.

4. Click on **_Years_** and choose **_2010_**. Now click on **_Surveys_** and scroll down to choose **_DEC Summary File 1_**. You've now added to your filter that you are interested in the decennial census data from 2010. As you know, the Census is decennial meaning every ten years. Finally, click **_SEARCH_**. 

5. A list of tables on the left side of the screen will display. We are looking for specific information about households by single parents, so type "Household Type" in the Search bar. You'll need to continue to click the "Load More" button until you arrive at a table with only the title "Household Type", with the table number "P18". (You may also simply search for "P18" to find this table.) Click on **_HOUSEHOLD TYPE_**.

6. You now need to download the data. To do so, click the **_Download_** button. You'll then need to re-check **_HOUSEHOLD TYPE_** as the table to be downloaded. Then, click **_Download Selected (1)_**. It should be located at the top of the list of tables to the left. If you do not see it, scroll up to find it.

7. Confirm that CSV is selected and click **_DOWNLOAD_**. After a short time, click **_Download Now_**.

    * _For the curious: CSV stands for **C**omma **S**eparated **V**alues and is an example of what’s called a text-delimited file type, meaning that it uses text to separate, or delimit, individual values it stores._

8. You now need to clean the data you’ve downloaded. Find the **_.zip_** file that you just downloaded and extract it. If you’re using a PC: right-click the file and selecting “Extract All.” The default settings should work fine. If you’re using a Mac: double-clicking the .zip file will automatically extract it.

    * **Tip:** Create a folder with a name you will remember on your desktop. When asked where to extract, click Browse, choose the desktop, create a new folder, and name it something like “M4 KY County Data.” Select this folder, and then click “extract.”)

9. Open **_DECENNIALSF12010.P18_data_with_overlays_2020-09-24T100627.csv_** in Microsoft Excel.

10. Save your work as new CSV file called: YourLastName_M4Data.CSV (e.g.“Wilson_M4Data.CSV”). If you are using Mac OS, **you must select Windows-compatible CSV from the drop-down menu below the prompt where you’ve entered the filename.** Save this file in a place where you can easily access it. You may want to **email it to yourself or save it to a USB thumb drive.**

11. We’re only interested in some of the attributes (the columns of data). In particular, we’re looking for data on each county’s **total population, single fathers, and single mothers**. We also need **the GEO_ID** and **the county name**.

12. To make this data easier to work with in Excel, **delete the other attributes in the spreadsheet**. (Keeping or deleting attributes in the Excel chart will not affect our map, just our efficiency and peace of mind in Excel). Deleting a column is like deleting a row (see step 9): right-click the letter above the column and select “delete.”

	- **Tip 1:** You can click and drag to highlight multiple columns for deletion at once. You can also use the “find” function (CTRL+F on PC, command+F on Mac) to find the columns you’re interested in more quickly.

	- **Tip 2:** You can also format the top row with the names to make them easier to find by selecting that row, clicking “Format Cells” then under the “Alignment” tab in the dialogue box that comes up, check the box next to “Wrap Text.” It will then look like the image below:

	- **Tip 3:** You can also use the “find” function in Excel to find these columns: copy the column names listed above in step 11 and paste them into the “find” box. Make sure that no rows or columns are selected before you search, or it will only search in that row/column. Alternately, highlight the entire chart first.

	- **Tip 4:** Once you find the columns you are keeping, you might fill them in with a color to make sure you don’t accidentally delete them.

	- **Tip 5:** Save your work as you go!

13. Rename the remaining five attributes **_“GEOID,” “LABEL,” “TOTPOP,” “SINGDADS,” and “SINGMOMS.”_**.

14. Remove all formatting from the file by selecting every cell in the spreadsheet (CTRL-A on PC, Command+A on Mac), clicking the _Home_ tab up top, and using the clear button (represented by an eraser) to **_Clear formats_**. You won’t see any changes, but this makes the data more readable by QGIS.

15. Format the attribute you’ve renamed “GEOID” as a **text field** – to do so, right click the GEOID column, select “Format Cells,” and select “Text.” Click OK.

16. Format the “TOTPOP,” “SINGDADS,” and “SINGMOMS,” attributes as **number fields** – to do so, select and right-click all the appropriate columns, select "Format Cells,” and select “Number.” You can leave the default setting; click OK. **Save your work!**

### Part 2 Questions

Respond to each of the following questions. Make sure you provide evidence for your claims where necessary, about 2 sentences per question.

1. In the context of this assignment, what is an attribute? List two examples of attributes included in the CSV file you saved.
2. Why did we take the time to “clean up” the census data? (Hint: review the instructions for pointers on this)
3. What kind of data is this census data and what makes it so:
    * individual or aggregate?
    * discrete or continuous?
    * qualitative or quantitative?

___

> [Mapping 4](../README.md) - [Install QGIS](../Install_QGIS/M4_Install_QGIS.md) - [Part 1](../Part_1/M4_Part_1.md) - [**Part 2**](M4_Part_2.md) - [Part 3](../Part_3/M4_Part_3.md)
