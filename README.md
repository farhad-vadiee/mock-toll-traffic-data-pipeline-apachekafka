# Educational Project: National Highway Traffic Data Analysis Project

## Overview
This project, part of an educational program, aims to de-congest national highways by analyzing road traffic data from various toll plazas. Using Kafka, we stream data like vehicle_id, vehicle_type, toll_plaza_id, and timestamp as vehicles pass through toll plazas. This repository contains scripts and instructions for setting up a data pipeline to collect this streaming data and load it into a database for further analysis.

## Prerequisites
- Apache Kafka
- Zookeeper
- Python 3.x
- Relevant Python libraries: (list any specific libraries used in the scripts)

## Installation & Setup
1. **Zookeeper Setup**: 
   - Start the Zookeeper server, a prerequisite for Kafka.

2. **Kafka Setup**:
   - Start the Kafka server after initializing the Zookeeper server.
   - Create a Kafka topic named `toll` for streaming the toll data.

## Components
1. **Toll Traffic Generator (`toll_traffic_generator.py`)**:
   - Simulates traffic data at toll plazas.
   - Streams data to the Kafka topic.

2. **Streaming Data Reader (`streaming_data_reader.py`)**:
   - Reads streaming data from Kafka.
   - Processes and loads data into a database.

## Usage
1. **Running the Toll Traffic Generator**:
   - Run `python3 toll_traffic_generator.py`.
   - Ensure Kafka is consuming data from the `toll` topic.

2. **Running the Streaming Data Reader**:
   - Run `python3 streaming_data_reader.py`.
   - Verify data loading into the database.

## Contributing
This project is part of an educational program. Contributions adhering to project standards are welcome.

## License
MIT License

Copyright (c) 2024 Farhad Vadiee
