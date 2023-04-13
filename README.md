# HermesPy : Queued State Machine Producer-Consumer (QSM-PC) Architecture Implementation in Python

HERMES is a Python project that implements the Queued State Machine Producer-Consumer (QSM-PC) architecture for simulating data acquisition, aggregation, processing, and logging. The project aims to simulate three parallel data acquisition processes (temperature, pressure, voltage) and includes an aggregator, a data processor for basic statistical analysis, and a data logging processor that saves the data to a CSV file.

## Project Objective

The objective of the HERMES project is to implement the QSM-PC architecture in Python to simulate data acquisition, aggregation, processing, and logging. Specifically, the project aims to accomplish the following:

- Simulate three parallel data acquisition processes (temperature, pressure, voltage).
- Aggregate and process the acquired data into time series.
- Perform basic statistical analysis on the processed data.
- Log the aggregated and processed data to a CSV file.

## Prerequisites

To run the HERMES project, you need to have the following Python packages installed:

- queue
- threading
- csv
- time
- datetime

## Getting Started

To get started with HERMES, you can follow these steps:

- Clone the repository to your local machine.
- Install the required Python packages.
- Open a terminal or command prompt and navigate to the project directory.
- Run the main script by executing python main.py.

## Project Structure

The HERMES project follows the following file structure:

├──data_aggregator.py

├──data_processor.py

├──data_logger.py

├──main.py

├──README.md

├──daq_pressure.py

├──daq_temperature.py

└──daq_voltage.py


- `main.py`: Main script that runs the project and creates threads for the DAQs, aggregator, data processor, and data logging processor.
- `daq_temperature.py, daq_pressure.py, daq_voltage.py`: Separate threads that simulate the data acquisition process for each type of data.
- `aggregator.py`: Separate thread that aggregates the data from the DAQs into time series.
- `data_processor.py`: Separate thread that processes the aggregated data by performing basic statistical analysis.
- `data_logger.py`: Separate thread that logs the aggregated and processed data to a CSV file and prints a table of the last 10 processed data items.
- `processed_data.csv`: CSV file that stores the logged data.
- `README.md`: Project documentation that provides an overview of the project, instructions on how to set up and run the project, and a detailed outline of the project structure.

## Conclusion
HERMES is a Python project that demonstrates the implementation of the QSM-PC architecture for simulating data acquisition, aggregation, processing, and logging. It provides an example of how to use Python packages like `queue`, `threading`, `csv`, `time`, and `datetime` to achieve parallel processing and efficient data communication between different processes.