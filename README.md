# Global Agricultural Analysis Dataset

## Project Overview

This repository contains a comprehensive, curated dataset structured for quantitative analysis of the factors influencing global agricultural production. The primary focus is on exploring the relationships between **Crop Production**, the key **Climate Variable** (**Average Temperature**), and essential **Agricultural Inputs** (Fertilizer and Pesticide Use) across multiple countries and years.

This dataset is suitable for:
* Developing data visualization dashboards and reports.
* Building econometric or statistical models to predict agricultural yields.
* Analyzing the long-term impact of temperature variations on agricultural output.
* Performing time-series and comparative analysis of agricultural trends.

## Data Files and Structure

The data is provided in a structured format, including both pre-processed, merged files ready for immediate use and granular source files for deeper inspection.

### Primary Analysis Files

These files are the most refined and are recommended for direct analysis and dashboard development.

| File Name | Description | Key Contents |
| :--- | :--- | :--- |
| `Agricultural Analysis Dashboard.xlsx - Clean Data.csv` | The master, cleaned, and merged dataset containing all primary variables (Country, Year, Temperature, Fertilizer, Pesticides, and Total Crop Production). | Country, Year, Avg\_Temperature\_C, Fertilizer\_tonnes, Pesticides\_tonnes, Crop\_Production (Total) |
| `Agricultural Analysis Dashboard.xlsx - Slicer.csv` | Summary statistics aggregated by year and country, likely intended for use as filters or high-level indicators in a dashboard environment. | Aggregates of Crop Production, Temperature, Pesticides, and Fertilizer |

### Granular and Component Files

These files contain the specific time-series data for each variable used to construct the primary analysis files.

| File Name | Description | Key Variables |
| :--- | :--- | :--- |
| `Agricultural Analysis Dashboard.xlsx - Crop_Production.csv` | Detailed, item-level crop production data by country, before being aggregated. | Country, Item (Crop Name), Year, Crop\_Production\_tonnes |
| `Agricultural Analysis Dashboard.xlsx - Crop_Production_Summary.csv` | A summary of total crop production aggregated by Country. | Country, Total Crop\_Production |
| `Agricultural Analysis Dashboard.xlsx - Temperature.csv` | Time-series data for average annual surface temperatures by country and year. | Country, Year, Avg\_Temperature\_C |
| `Agricultural Analysis Dashboard.xlsx - Fertilizer_Use.csv` | Time-series data for total fertilizer consumption in tonnes by country. | Country, Year, Fertilizer\_tonnes |
| `Agricultural Analysis Dashboard.xlsx - Pesticide_Use.csv` | Time-series data for total pesticide consumption in tonnes by country. | Country, Year, Pesticides\_tonnes |

### Original Source Files

These files represent the raw, unprocessed data extracts from their original sources, used for data cleaning and transformation.

* `FAOSTAT_data_en_11-7-2025 (2).csv`
* `GDL-Yearly-Average-Surface-Temperature-(ºC)-data (1).csv`
* `Pesticides Usage.csv`
* `Total Fertilizer Use.csv`
