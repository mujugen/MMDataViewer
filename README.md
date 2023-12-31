# Data Analysis and Visualization Tool

This tool is designed for data analysis and visualization of time-series data related to various exercises and workouts. It can load data from CSV files, extract timestamps, plot raw data, and even smooth the data using cubic spline interpolation. Additionally, it provides functions for data manipulation, such as deleting records and saving the data to a new CSV file.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Functions](#functions)

## Prerequisites

Before using this tool, make sure you have the following Python libraries installed:

- pandas
- matplotlib
- datetime
- textwrap
- os
- scipy
- numpy
- seaborn

You can install these libraries using `pip`.

## Installation

1. Clone this repository or download the source code.
2. Open a terminal or command prompt and navigate to the project directory.
3. Run the script using Python:


## Usage

You can use this tool to analyze and visualize time-series data from CSV files. Here are the main functions and their descriptions:

## Functions

- `load_data(file_path, column_time)`: Load data from a CSV file, remove rows with NaN values in the specified time column, and convert string columns to lowercase.

- `extract_timestamps(df, column_time, record_index)`: Extract timestamps from the specified time column of the DataFrame.

- `plot_data(df, timestamps, columns, record_index)`: Plot raw data for the specified columns at a given record index. The data is plotted against timestamps.

- `plot_smooth_data(df, timestamps, columns, record_index, smoothness)`: Plot smoothed data for the specified columns using cubic spline interpolation. The data is plotted against timestamps.

- `delete_record_and_save_to_csv(df, record_index, csv_filename)`: Delete a record from the DataFrame by index and save the updated DataFrame to a new CSV file.
