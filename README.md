# Tableau - Desktop I: Fundamentals

Tags: done
dashboards: multiple local saved
source link: https://elearning.tableau.com/desktop-i-fundamentals

### About This Course

In this course, I've learnt fundamental skills for analyzing your data in Tableau Desktop, like to connect to and customize data sources, edit field metadata, group fields, and apply sorting and filtering techniques. Exploring the Data pane and Desktop workspace, I grasped the difference between dimension and measure data, and use fields to build essential charts, including line charts for time-based data; crosstabs and highlight tables; axis charts, scatter plots, and maps. I wrote calculations to customize data, and apply table calculations to a view. Finally, I created interactive dashboards that help guide specific data analysis.

### **Time Estimate:**

10+ hours

### **Learning Objectives**

At the end of this course, you will be able to:

- Connect to your data and edit a data source.
- Edit metadata and group fields.
- Sort and filter data.
- Use the Desktop workspace to create visualizations.
- Build essential chart types.
- Create basic calculations, including arithmetic calculations, custom aggregations and ratios; and use quick table calculations.
- Build interactive dashboards and stories to reveal data insights.

## Workflow

1. Connect (preview of 10k rows, and Live connection as default)
2. Analyze
3. Share

## Dimensions and Measures

- **Dimension**: fields that contain **qualitive** data or categorical data, such as product name or city
- **Measure**: fields that contain **quantifiable** data, such as *sales amount* or *quantity sold*

## Tableau File Types:

- **Workbooks (.twb)**

    Tableau workbook files have the .twb file extension. Workbooks hold one or more worksheets, plus zero or more dashboards and stories.(Saves the all the sheets and their connection information in a workbook file. The data is not included.)

- **Packaged Workbooks (.twbx)**

    Tableau packaged workbooks have the .twbx file extension. A packaged workbook is a single zip file that contains a workbook along with any supporting local file data sources and background images. This format is the best way to package your work for sharing with others who don’t have access to the data.(Saves all the sheets, their connection information and any local resources (e.g., local file data sources, background images, custom geocoding, etc.).

- **Data Extract (.tde)**

    Tableau data extract files have the .tde file extension. Extract files are a local copy of a subset or entire data source that you can use to share data, work offline, and improve database performance.

- **Data Source (.tds)**

    Tableau data source files have the .tds file extension. Data source files are shortcuts for quickly connecting to data sources that you use often. Data source files do not contain the actual data but rather the information necessary to connect to the data source as well as modifications you've made in the Data pane such as default properties, calculated fields, groups, and so on.

- **Packaged Data Source (.tdsx)**

    Tableau packaged data source files have the .tdsx file extension. A packaged data source is a zip file that contains the data source file (.tds) described above as well as any local file data sources such as Extract files (.tde), text files, Excel files, Access files, and local cube files. Use this format to create a single file that you can then share with others who may not have access to the original data stored locally on your computer.

- **Bookmarks (.tbm)**

    Tableau bookmark files have the .tbm file extension. Bookmarks contain a single worksheet and are an easy way to quickly share your work.

## **Connection:**

 ****Tableau makes a live connection to the data, by maintaining a connection to the data source, so data refreshes in the workbook.

- **Filters**: Tableau uses AND as a default logic to apply multiple filters.
- **Sort**: computed sort or manual sort. only can be sorted by the Rows.
- **Groups**:  you can create them by right-clicking the value on the Dimensions panel(1), or view the view(2): by clicking the labels or by selecting the marker.
- **Hierarchy**: just drag and drop.

1. Discrete values: represents a specific amount of fields. E.g. Date part
2. Continuous values: Data over time. Could be in different ranges of numerical values . E.g.,  Date value

**Dual Axis**: double measure axis.

**Measures values:** a measure, ****appears automatically whenever we have two or more measures values in rows.

**Measures names**: a dimension that appears automatically whenever we have two or more measures values in rows. It gets placed on the filters card and as a field on columns(as a placeholder).

We can only synchronize the second axis to the first, not vice versa. After synchronized we can hide the second axis(uncheck *show-Header*) and rename the title for more accurate description.

Dual axis charts are also called ***Combo charts**.*

**Combined Charts:** when we remove the measure names , *(that were automatically placed on columns),* we get these types of charts, because each column gets stacked in the same field.

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled.png)

**Scatter plots**: usually created by measure values.

In ANALYSIS tab we can enable/disable *Aggregation,* which is gonna enable us to have more detailed data. 

Also by adding a dimension value into Detail level section , we can have more detailed data.

**Mapping your Data:**

- **Symbol Maps**:
    - Geographical data:
        - **latitude** y-axis (north/south) - rows.
        - **longitude** x-axis (western/eastern) - columns.
    - Tableau by default has a geocode that can be triggered by postal code, country names, etc (8 in total)

- **Fill Maps**:  fills up every part of a region.

## **Crosstabs**

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%201.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%201.png)

- Totals and Aggregations

    Analysis > Totals > Grand Total

    From Analytics Panes > drag and drop Totals.

    If we want to change the aggregation of total , we must change it on the measure values.

- Highlight tables

    Useful when we want to show outliers, trends, odd data.

    From show me, or create two identical measures from ***color*** and ***text*** and select ***square*** as marks method.

    ![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%202.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%202.png)

- HeatMaps

    Need 1 or more dimensions and two measure. Or a single measure.

    then select **Color** and **Size,** on marks panel.

    ![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%203.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%203.png)

## Using Calculations: Customize Your Data

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%204.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%204.png)

    It is only available in the Dimensions Pane.

## Running Total and Percent Total

First select Table calculation

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%205.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%205.png)

Then Compute using:

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%206.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%206.png)

### Default is : "Table Across"

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%207.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%207.png)

### Table Down

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%208.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%208.png)

### Pane Down

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%209.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%209.png)

### Pane Across

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2010.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2010.png)

CEll:

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2011.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2011.png)

HOW ARE TABLE CALCULATIONS DIFFERENT FROM OTHER TYPES OF CALCULATED FIELDS?→ Table calculations are calculated based on the data in the view.                                     →Table Calculation is not automatically added to the measure Pane.

## Pie chart

it's recommended to show from 2 to 5 categories.

## Showing Hierarchy with Tree Maps

- Do not have axes( it doesn't use row or columns), they just use the Marks Pane: **color, size & detail**.
- Color best practices up to 7 different ones.
- A word-cloud can be created using a TEXT mark type.
- A bubble-chart also can be created, using a CIRCLE mark type.

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2012.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2012.png)

# Reference Lines and Bands

BANDS:

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2013.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2013.png)

DISTRIBUTUIONS

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2014.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2014.png)

BOX PLOT

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2015.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2015.png)

# Dashboards

![Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2016.png](Tableau%20Desktop%20I%20Fundamentals%201b48fd674dc44ae1bf2c9ed1796a9dd2/Untitled%2016.png)

there are 3 Actions in Dashboards: hover, select or menu. (Go to Dashboard > Actions)

We can add Filters as Actions as well.

---

# Certification

[Certificate for Desktop I: Fundamentals](https://verify.skilljar.com/c/5ctqvw7e3t66)