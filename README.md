# Intrusion Detection System (IDS) using CICFlowMeter

## Overview
This project implements an Intrusion Detection System (IDS) that processes network traffic data to classify and detect potential threats. It leverages the CICFlowMeter tool to extract network flow features and uses a machine learning model to classify the traffic.

## Key Features
- Data preprocessing from PCAP files to CSV format using CICFlowMeter.
- Classification of network traffic using a machine learning model (`model.py`).
- Automation scripts for data processing (`clean_pcap_csv.sh`, `convert_pcap_csv.sh`, etc.).
- Logging of execution time and debugging information.

## Dependencies
- CICFlowMeter
- Python 3.8 and above
- Required Python libraries (see `requirements.txt`)

## Installation and Setup
1. Clone this repository:

   git clone https://github.com/yourusername/IDS_system.git
   cd IDS_system   

2. Install dependencies:
   Use the following command to install the necessary Python dependencies:
     - pip install -r requirements.txt
   
3. Run the necessary scripts to preprocess data:
    pip install -r requirements.txt

3. Run Preprocessing Scripts
After cloning the repository and installing dependencies, run the preprocessing scripts to convert PCAP files to CSV format:

  - Convert PCAP to CSV:
      ./convert_pcap_csv.sh

  - Clean CSV Data:
      ./clean_pcap_csv.sh

4. Model Training and Evaluation
  Once the data is processed, use the classifier to train and evaluate the machine learning model:

    python model.py
  The script will train the model on the processed data and evaluate its performance.


6. Usage Guide
To use the Intrusion Detection System:

Place your network capture (PCAP) files in the pcap folder.
Run the scripts to convert and clean the data.
Train and evaluate the model using the model.py script.

6. File Structure
# convert_pcap_csv.sh: Converts network capture (PCAP) files to CSV format.
clean_pcap_csv.sh: Cleans and formats the converted CSV data.
model.py: Contains the machine learning model for intrusion detection.
classifier.ipynb: A Jupyter notebook for exploratory data analysis and model testing.
requirements.txt: Lists the Python dependencies.

8. Logs and Debugging
Execution time and debugging logs are stored in the logs folder. You can view detailed logs for troubleshooting or performance analysis.

