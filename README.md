# Custom Quad Chart Visual in Power BI using ggplot2

Power BI enables you to create custom visualizations using R. In this repo I demostrate how you can use the R programming language to create a quad chart in Power BI. The data used in the demo is NFL combine data. I use filters in Power BI to select the year and position that I want to based the quad chart on and R to create the visualization.

A complete coverage of the code is contained in the ***Create_Custom_Visualizations_in_PowerBI_with_ggplot2*** Jupyter Notebook. PBI_QuadChart is the pbix file that contains the Power BI example.

Known limitations of R visuals in the Power BI desktoop ([Source Website](https://docs.microsoft.com/en-us/power-bi/desktop-r-visuals)):
- Data size limitations – data used by the R visual for plotting is limited to 150,000 rows. If more than 150,000 rows are selected, only the top 150,000 rows are used and a message is displayed on the image.
- Calculation time limitation – if an R visual calculation exceeds five minutes the execution times out, resulting in an error.
- Relationships – as with other Power BI Desktop visuals, if data fields from different tables with no defined relationship between them are selected, an error occurs.
- R visuals are refreshed upon data updates, filtering, and highlighting. However, the image itself is not interactive and cannot be the source of cross-filtering.
- R visuals respond to highlighting other visuals, but you cannot click on elements in the R visual in order to cross filter other elements.
- Only plots that are plotted to the R default display device are displayed correctly on the canvas. Avoid explicitly using a different R display device.
- In this release, RRO installations are not automatically identified by the 32-bit version of Power BI Desktop, so you must manually provide the path to the R installation directory in Options and settings > Options > R Scripting.

Additional Resources:

- [R for Data Science](http://r4ds.had.co.nz/): I believe this book is the best introduction to the R programming language.

- [Guy in a Cube](https://guyinacube.com/): Great YouTube for all things Power BI. Patrick and Adam does a group job of keeping you informed with what's new in Power BI and they also provide great tutorials on how to use the tool.

- [Excel on Fire](https://www.youtube.com/channel/UCZgOVykPoRbSZQfY9YysiRQ):  Oz does a great job creating a tutorials on how to use Power Query for data munging.

- [Mico Yuk](http://bibrainz.com/aof/author/micoyuk/): Mico Yuk provides great training on how to effectively use data visualization to tell amazing stories about your data.

In addition to the resources above I plan to add content covering how you can leverage R in Power BI as well as in the rest of the Microsoft ecosystem in my [blog](https://dieselanalytics.com/). Be on the look out!
