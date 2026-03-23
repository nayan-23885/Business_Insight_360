# Business_Insight_360
![image alt](https://github.com/nayan-23885/Business_Insight_360/blob/a278af8e128a7c20ced060abb6adcfc220f144cf/Screenshot%202026-03-23%20155347.png)
## Introduction
This project outlines end-to-end development of the Atliq Hardware Power BI analytics suite. The project objective was to transition from siloed, static reporting to a robust, automated Business Intelligence solution. By integrating diverse data systems, engineering a scalable data model, and designing interactive cross-functional dashboards, the project delivers actionable insights across Finance, Sales, Marketing, and Supply Chain operations.

## Data Extraction and the ETL Process
The foundation of the project required establishing a reliable connection to the organizational Data. Raw data was imported from multiple sources to capture a complete business picture, integrating historical transaction logs stored in CSV files with live, operational datasets queried directly from a MySQL database.

To clean and shape this data, Power Query was utilized as the primary ETL (Extract, Transform, Load) tool. The transformation phase involved cleaning missing values, standardizing data types, merging queries, and removing redundancies to ensure the data was primed for accurate analytical modeling.

## Data Modeling and Schema Architecture
A highly optimized relational data model was constructed using principles of the Star and Snowflake schema. This involved normalizing the data by creating dimension tables (such as Date, Geography, Product, and Customer hierarchies) and establishing active and inactive relationships with the central Sales and Finance fact tables. This architectural choice significantly optimized query performance and allowed for seamless, multi-dimensional slicing of the data.

## The Analytical Engine: DAX and Table Structures
The core computational logic of the dashboard was powered by DAX (Data Analysis Expressions). DAX was leveraged extensively to create complex, time-intelligent measures, such as Year-over-Year growth, dynamic Gross Margin % calculations, and variance against targets.

During the development, different table structures were utilized to serve specific needs. Static tables were manually entered or imported to hold fixed reference variables, while Dynamic tables were generated using DAX functions to create contextual, calculated summaries on the fly without burdening the source database.

## Advanced Visualization and User Interactivity
To provide an intuitive and highly engaging user experience for both functional teams and executive leadership, several advanced Power BI features were implemented:

### Parameters & Dynamic sliders: 
These were introduced to allow users to dynamically adjust variables like gross margin targets and instantly see which countries failed to achieve the target.

### Bookmarks: 
Utilized to create app-like navigation experiences, allowing users to toggle between different visual states with a single click.

### Tooltips: 
Custom report page tooltips were designed to reveal granular, secondary insights (like specific product performance) when hovering over high-level visuals, keeping the main interface uncluttered.

### Conditional Highlighting: 
Applied to matrices and charts to instantly draw the eye to critical metrics—for example, automatically formatting missed targets with a downward arrow icon.

### Interactions: 
Visual interactions (cross-filtering and cross-highlighting) were meticulously edited to ensure that selecting a specific region or product category appropriately filtered the surrounding charts, maintaining analytical context.

## Deployment and Automation
The final phase involved transitioning the project from development to production. This was achieved by Deploying the dashboard to the Power BI Service workspace, enabling secure access for organizational stakeholders. To eliminate the need for manual updates and ensure the executive views always reflected the latest operational realities, a data gateway was configured to facilitate Automatic refreshing of the underlying MySQL and CSV datasets on a scheduled cadence.

## Key Learnings
This development cycle provided deep, practical exposure to the entire lifecycle of enterprise data analytics. I moved data from raw, multi-source ingestion through complex ETL pipelines, structured it in a scalable Snowflake schema, and translated it into an interactive, deployed business tool, solidifying my understanding of modern Business Intelligence architecture.

## Preview Live Project
The project may be accessed by clicking the following link. 

[Live Project Link](https://app.powerbi.com/view?r=eyJrIjoiODQ3MmZkMTMtNzViMy00Y2ZlLTgxZTgtZGNmNzQ1YTg1YThjIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)
