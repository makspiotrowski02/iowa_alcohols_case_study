# Iowa Alcohol Sale Case Study

![Title](/Images/Title.jpg)
## Project Overview

Welcome to the case study documentation for the Vodka Sales and Marketing Analysis. This analysis focuses on identifying optimal store locations and times for marketing a new american vodka product based on historical sales data.

## Useful Links

- [See the case study report](/presentation.pdf)
- [Link to  the dataset](https://data.iowa.gov/Sales-Distribution/Iowa-Liquor-Sales/m3tr-qhgy/about_data)

## Tools Used
- **Data Cleaning**: Python 
- **Data Aggregation**: SQL (SQLite3), Python
- **Data Analysis**: Excel, Jupyter Notebook
- **Data Manipulation**: SQL (SQLite3), Python
- **Visualizations**: Power BI, PowerPoint
- **Documentation**: Markdown, GitHub

## Workflow

1. **Data Collection**: Initially dataset was found on Kaggle, but then original source was used for 10 times more records.
2. **Data Cleaning**: Performed quick operations to rename columns, identify, and analyze missing values. After analysis few columns were dropped and records with missing values were deleted.
3. **Data Aggregation**: Using Python with SQLite3 and Pandas data was aggregated into csv files for further analysis in Excel.
3. **Data Analysis**: Conducted analysis in Excel and Jupyter Notebook to understand sales trends, identify key factors affecting vodka sales, and spot potential growth opportunities. 
4. **Visualization**: From Excel and csv files data was imported to Power BI to create meaningful visuals.
5. **Reporting**: Compiled the analysis results into a report in PowerPoint outlining strategies for effectively marketing the new vodka product. Then completed project was uploaded to GitHub.

## Challenges Encountered

- **Data Volume(SQL)**: 

    The dataset contains 28 million records and is approximately 7GB in size. Initially, I attempted to load it into Excel, since it was consolidated into a single CSV file. However, Excel's limit is 3 million records, so it was not enough.

    Next, I attempted to import the data into a local XAMPP installation. Despite modifying the configuration file to change maximum size and time limits, the import consistently failed with errors after about 6 minutes.

    Then, I turned to Google’s BigQuery, successfully uploading the file to a container and attempting to create a table from it. While the upload was successful, the process generated numerous errors that I couldn't indentify, resulting in an unusable table.

    Finally, I experimented with SQLite3, a Python library that simulates an SQL database environment. This approach was successful and the performance was quite nice.
- **Data aggregation**: 
    
    Because of using SQLite3, the entire query process was conducted within a Jupyter Notebook. To streamline the workflow and save time, I wrote several functions for querying, printing, and saving results. I organized the notebook into distinct sections: one for the functions, another for initializing the server, a separate section for executing queries, and a library section that included some of the initial queries. This structure made the notebook easier to navigate and use.

- **Filled map**: 
    
    I really wanted to use the filled map visual in Power BI for state-level visualization, but it didn’t turn out as expected. The customization options for this visual were quite limited, preventing me from achieving the desired appearance. Additionally, the visual was laggy, and the zoom steps were too big, making it difficult to adjust the view so that a state perfectly filled the whole page. Another limitation was the absence of an option to use a color range to illustrate differences between counties. Because of it I had to calculate the gradations in Excel and then manually assign a color from the color scale to each step which worked, but wasn't perfect.


## Conclusion

The project had some problems, but i think it turned out great. It is simple, comprehensive, well balanced and complete from start to finish. If i would make it over again I would put more text on the presentation to explain visuals, but I was worried that it would bcome too cluttered.

