# Master Thesis

## Title
**Identification of Electrical Devices Using Machine Learning: A Study in Collaboration with Origin AS**

## Author
**Konrad Jarczyk**

## Supervisor
**Nejm Saadallah**

## Dataset
**UK-DALE** (available at [this link](http://data.ukedc.rl.ac.uk/simplebrowse/edc/efficiency/residential/EnergyConsumption/Domestic))

## Overview
This repository contains the coding part of my master thesis, which is divided into five main Jupyter notebooks. Each notebook includes detailed comments on how to run the code.

### Files
- `preprocessing.ipynb`
- `random_forest.ipynb`
- `rnn_lstm.ipynb`
- `cnn.ipynb`
- `process_mining.ipynb`

## Preprocessing
The `preprocessing.ipynb` notebook contains steps to prepare ready data frames for machine learning models.

### Steps:
1. **Choose the house** from which the analysis will be performed.
2. **Load data**: The algorithm loads all devices into one DataFrame with labels.
3. **Analyze devices**:
    - Perform clustering for each device and decide on the number of clusters for the given device.
    - Select the number of visible states and the name of the device to analyze.
    - Choose to either drop the device from the DataFrame or keep its clustered form.
4. **Save DataFrame**: Save the prepared DataFrame to Parquet files.

## Machine Learning Models
The following notebooks have similar configurations where you can load the prepared Parquet file and choose the devices to analyze.

### Notebooks:
- **`random_forest.ipynb`**: Implements the Random Forest model for device identification.
- **`rnn_lstm.ipynb`**: Implements the RNN with LSTM model for device identification.
- **`cnn.ipynb`**: Implements the CNN model for device identification.
- **`process_mining.ipynb`**: Implements Process Mining techniques to identify interconnections between devices.

Each notebook includes detailed steps and comments to guide you through the process of running the code.

## Instructions
1. **Preprocessing**:
    - Open `preprocessing.ipynb`.
    - Follow the steps to prepare the data.
    - Save the processed data to Parquet files.
2. **Running Models**:
    - Open any of the model notebooks (`random_forest.ipynb`, `rnn_lstm.ipynb`, `cnn.ipynb`, `process_mining.ipynb`).
    - Load the Parquet file.
    - Choose the devices to analyze.
    - Run the code to train and evaluate the model.

## Contact
For any questions or further information, please contact **Konrad Jarczyk**.

