# Elections Results Processing

This repository contains R code designed to process election results data. The code performs several tasks including reading raw data from a CSV file, filtering and renaming columns based on specific criteria, and compiling election results into a structured format.

## Overview

The script starts by setting up the necessary R packages. If any required package is not installed, it will be installed automatically. It then reads election data from a CSV file, filters columns based on a specific pattern in their headers, and renames these columns to more concise names based on predefined mappings. The final part of the script calculates the frequency of votes for each candidate and organizes the results in a structured data frame, ready for analysis or export.

## Required Packages

- dplyr
- tidyverse
- stringr
- stringi

## Key Features

- **Data Filtering:** Filters columns based on header content to retain only those relevant for ranking preferences.
- **Column Renaming:** Applies a mapping to rename columns with long titles to more manageable abbreviations, incorporating the position and rank number.
- **Results Compilation:** Calculates and sorts the frequency of votes for each candidate across different positions and ranks, producing a comprehensive results data frame.

## Usage

Ensure the `ElectionResults.csv` file is placed in the `./data` directory. Run the script to process the election results. The final results are stored in a data frame called `results_df`, which can be exported to a CSV file if needed.
