# Time-Series-Project

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Dataset](#dataset)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [License](#license)

## Overview

This project focuses on process monitoring using the NASA Bearing Dataset, leveraging the Chronos-Forecasting library to predict bearing data and evaluate prediction accuracy through the Mean Absolute Error (MAE) metric. 
For each dataset, pre-trained pipelines from Chronos-Forecasting are used, including:
- **chronos-t5-tiny**: 8M parameters
- **chronos-t5-mini**: 20M parameters
- **chronos-t5-small**: 46M parameters
- **chronos-t5-base**: 200M parameters
- **chronos-t5-large**: 710M parameters

The methodology involves preparing the data from each file to ensure compatibility with Chronos-Forecasting, applying the pre-trained models to predict future bearing values, and evaluating these models using MAE to measure prediction accuracy. The results provide insights into the effectiveness of the different pre-trained models across various dataset configurations, guiding further improvements and optimizations.

## Installation

To set up the project, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/SofiaFranceschi/Time-Series-Project.git
    cd Time-Series-Project
    ```

2. Download the dataset from:
    https://www.kaggle.com/datasets/vinayak123tyagi/bearing-dataset

3. Install the required Python packages:
    ```bash
    pip3 install -r requirements.txt
    ```

## Dataset

The dataset used for this project is sourced from Kaggle and contains 3 sets of bearing measurement data.

- Dataset URL: [NASA Bearing Dataset](https://www.kaggle.com/datasets/vinayak123tyagi/bearing-dataset)

Download the dataset and extract the contents into **Time-Series-Project** folder. We have to place this item at the same level as the `main.ipynb` file. The directory structure should be as follows:
```
📁 Time-Series-Project
└── main.ipynb                  # Main notebook for running the project
└── README.md                   # Project README file
└── requirements.txt            # List of required Python packages
└── 📁 archive                  # Dataset extracted from Kaggle
    └── 📁 1st_test
        └── 📁 1st_test
    └── 📁 2nd_test
        └── 📁 2nd_test
    └── 📁 3rd_test
        └── 📁 4th_test
            └── 📁 txt
```

## Usage

To run the forcasting, execute the main Jupyter Notebook file:

1. Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

2. Open and run all cells in the `main.ipynb` notebook.

This notebook contains all the necessary code to train the model, evaluate its performance, and make forcasting on the data.

## Project Structure

The repository is structured as follows:
```
📁 Time-Series-Project
└── main.ipynb                  # Main notebook for running the project
└── README.md                   # Project README file
└── requirements.txt            # List of required Python packages
└── 📁 archive                  # Dataset extracted from Kaggle
    └── 📁 1st_test
        └── 📁 1st_test
    └── 📁 2nd_test
        └── 📁 2nd_test
    └── 📁 3rd_test
        └── 📁 4th_test
            └── 📁 txt
```

## Results

The performance of the forecasting is evaluated using MAE (Mean Absolute Error). Detailed results are available in the `main.ipynb` notebook.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.


