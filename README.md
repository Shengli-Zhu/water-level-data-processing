# Water Level Data Processing and Visualization

This repository contains scripts for processing water level data and calculating flow rates using predefined fitting parameters. The process involves reading CSV files, cleaning and transforming data, applying fitting functions to calculate flow rates, and visualizing the results. The scripts handle multiple CSV files in batch mode and output the processed data and visualizations.

## Sections

### Raw Water Level Data Processing and Visualization

This section processes raw water level data, handling datetime parsing, cleaning, and visualizing the data.

#### Features:
- Reads water level data from CSV files in the `data` directory.
- Cleans and processes the data, marking and dropping invalid entries.
- Outputs processed data to the `processing` directory with filenames suffixed by `_Processed`.
- Generates visualizations of water level data and saves them in the `processing` directory.

### Batch Processing of Water Level Data and Flow Rate Calculation

This section processes all CSV files in the `processing` directory, calculating flow rates using predefined fitting parameters.

#### Features:
- Reads processed water level data from the `processing` directory.
- Applies rise and fall fitting functions to calculate flow rates.
- Outputs calculated flow rates to the `result` directory with filenames suffixed by `_Calculated_Flow_Rate`.
- Generates visualizations of water level-flow rate relationships and saves them in the `result` directory.

## Directory Structure
.
├── data
│ └── [input CSV files]
├── processing
│ └── [intermediate processed CSV files and visualizations]
├── result
│ └── [final processed CSV files and visualizations]
├── Water level data processing.ipynb
├── requirements.txt
└── README.md

## Usage

1. Place your raw water level CSV files in the `data` directory.
2. Run the Jupyter notebook `Water level data processing.ipynb` to process the raw data and generate visualizations.
3. The notebook will also calculate flow rates and generate additional visualizations.

## Requirements

Install the required Python packages using this command: `pip install -r requirements.txt`

## Example
To process the raw water level data and calculate flow rates, open and run the `Water level data processing.ipynb` notebook.

## License
This project is licensed under the MIT License - see the LICENSE file for details.