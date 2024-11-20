---
layout: default
title: Homework 6.1 Visualizations
---

# Homework 6.1 Visualizations
## - By Janhavi Tushar Zarapkar (jzarap2@illinois.edu)

## Visualization 1: Building Count by Decade for top 10 Counties




<iframe src="bar_chart.html" width="1000" height="550"></iframe>

## Writeup for Vizualization 1:
## Why I Chose to Visualize This:
I chose this visualization to explore trends in building acquisitions across the top 10 counties and to see how these trends varied by decade. The bar chart provides a straightforward way to compare counts over time, helping identify patterns such as surges or declines in building activity. By focusing on the top counties, I ensured that the visualization remains concise and relevant to key regions.

##  Encoding Types:

- **X-axis (Decade)**: I encoded the Decade as an ordinal variable because decades represent distinct time intervals that are easy to understand and compare. This emphasizes the chronological order and makes trends over time more evident.

- **Y-axis (Building Count)**: Encoding the Count as a quantitative variable made sense because the heights of the bars directly represent the number of buildings acquired. This allows for an intuitive comparison of values.

- **Color**: I used color to encode the Decade variable. Different colors for each decade help visually separate and compare data points within a county. I specifically chose the category10 palette because it provides a diverse set of easily distinguishable colors, suitable for a maximum of 10 categories.

- **Tooltip**: I included tooltips to provide additional information (County, Decade, and Count) without cluttering the chart. This way, users can get precise details by hovering over bars.

## Color Scheme:
I used the category10 color scheme because it is designed for categorical data and ensures that each decade has a unique, distinct color. This helps prevent confusion when comparing data across decades. By using decade-based color encoding, I reinforced the temporal focus of the visualization, ensuring that users can quickly distinguish trends.

## Transforming the Data:

- **Creating the Decade Column**: I transformed the Year Acquired column into a Decade column to group data into meaningful time intervals. This simplification allowed me to focus on broader trends rather than yearly fluctuations, which might have introduced noise.

- **Selecting the Top 10 Counties**: I identified the top 10 counties using value_counts() because focusing on the counties with the most data ensures that the visualization highlights significant trends rather than being diluted by less relevant data.

- **Filtering Data**: By filtering the dataset to only include the top 10 counties, I reduced clutter and ensured that the visualization remains focused and interpretable.

- **Grouping and Aggregation**: Grouping the data by Decade and County allowed me to calculate the total number of buildings acquired for each combination. This summarized the data effectively and prepared it for visualization.


## Interactivity:

- **Dropdown for County Selection**: I added the dropdown to let users focus on one county at a time. This way, users can explore individual trends in detail without being overwhelmed by data from all counties at once.

- **Improved Clarity**: Interactivity simplifies the chart by letting users filter the data dynamically, as I did for county. This reduces visual noise and helps highlight specific insights.

- **Hover Tooltips for Precision:** I included hover tooltips to show the building count for a specific county and decade. This feature enhances usability by providing detailed information on demand without cluttering the chart, making it easier to analyze trends and exact values interactively.


## Impact of this Vizualization:

I designed this visualization to balance simplicity and depth. The bar chart is easy to interpret, while the interactivity and use of color add layers of engagement and detail. By transforming the data thoughtfully and focusing on meaningful categories, I created a chart that is both informative and user-friendly.





## Vizualization 2:  Average Square Footage by Usage Description with Filters for Top 15 Counties and their Building Status



<iframe src="bar_plot.html" width="1100" height="550"></iframe>

## Writeup for Vizualization 2 :

## Why I Chose to Visualize This:
I chose this visualization to analyze the average square footage of buildings by their usage description across the top 15 counties. The horizontal bar chart provides a straightforward and accessible way to compare the average square footage of buildings for different usage types. By focusing on the top 15 counties, I ensured that the visualization highlights the most significant areas, ensuring it remains relevant and not overwhelmed by smaller datasets. The interactivity, such as the county and building status filters, allows for an in-depth exploration of how these variables influence the results.

##  Encoding Types:


- **Y-axis (Usage Description):** I encoded the Usage Description as an ordinal variable on the y-axis. This choice allows the chart to display the building types in a logical order and makes it easier for users to compare different categories.

- **X-axis (Average Square Footage):** The average square footage is represented as a quantitative variable. The x-axis directly measures this, with the length of the bars providing an intuitive way to compare the average size of buildings across different usage types.

- **Color (County):** I used County:N for the color encoding. By applying the viridis color scheme, I ensured that each county is represented with a distinct color, allowing for easy identification. The scheme was explicitly set to cover the top 15 counties, helping visually separate the counties in the dataset.

- **Tooltip:** I added tooltips to show additional details for each bar, including the usage description, average square footage, county, and building status. This interactive feature allows users to explore the data without cluttering the chart with excessive text, offering precise values on demand.

## Color Scheme:
I used the viridis color scheme, which is designed for categorical data and works well for differentiating between multiple categories, as it’s perceptually uniform. This ensures that each county is easily distinguishable by its unique color. While viridis is effective in distinguishing counties, it also maintains clarity when displaying the data interactively.

## Transforming the Data:
- **Top 15 Counties:** To keep the focus on the most relevant data, I identified the top 15 counties by the total number of records. This approach helped streamline the dataset and made the visualization more manageable while highlighting the regions with the most significant building activity.

- **Filters:**  I have added 2 Interactive filters for county and building status. These filters allow users to narrow down the data based on their preferences, improving the chart's interactivity. If no records exist for a selected combination (e.g., a county and a particular building status), the chart will not display any bars, leaving the view blank.

## Interactivity:

- **Dropdown for County and Building Status Selection:** The dropdown filters for both County and Building Status let users explore the data dynamically. Users can select individual counties or building statuses, and the chart will update accordingly, showing only the relevant data.

- **Hover Tooltips for Precision:** I included hover tooltips that display detailed information about each data point, such as the usage description, average square footage, county, and building status. This feature enhances the usability of the visualization, allowing users to explore the exact data values without adding unnecessary clutter.

## Impact of This Visualization:
This visualization strikes a balance between simplicity and depth. The use of horizontal bars makes it easy to compare the average square footage across different usage descriptions, while the interactivity allows users to filter the data according to their specific interests. The explicit color differentiation between counties makes it easy to identify trends across regions, and the tooltips provide additional context to help users understand the data. By transforming and filtering the data effectively, I’ve created a visualization that is both informative and user-friendly, giving clear insights into the relationship between usage descriptions, square footage, county, and building status.


#### Resources

- [The Data](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv)
- [The Analysis](https://github.com/zarapkarjanhavi/Homework_6.1/blob/main/Workbook.ipynb)
