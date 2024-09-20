# BioGr

BioGr is a Python application designed for biologists to analyze SBML models by converting them into graph form and pushing them to a Neo4j database. With an intuitive graphical interface, users can load models, query graphs, and merge nodes seamlessly.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
  - [System Requirements](#system-requirements)
- [Usage](#usage)
  - [Prerequisites](#prerequisites)
  - [Starting Up](#starting-up)
  - [Model Conversion](#model-conversion)
- [Step-by-Step Guide](#step-by-step-guide)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Upload SBML Models:** Easily upload SBML models for conversion to graph format.
- **Search Functionality:** Find specific compounds or processes within the graphs.
- **Compare and Merge Graphs:** Assess similarities and merge graphs as needed.
- **Graph Visualization:** Intuitive graphical representation of biological data.

## Installation

## System Requirements

- **Python:** Version 3.8+
- **Neo4j Database:** Version 4.0+
- **Required Python Libraries:**
  - `neo4j`
  - `neo4jsbml`
  - `python_cypher`
  - `libsbml`
  - [Add any other necessary libraries here]

To install `neo4jsbml`, you will need Anaconda or Miniconda. Then run:
```bash
conda install -c conda-forge neo4jsbml

To install the other Python dependencies, run:
pip install neo4j python_cypher

## Usage

## Prerequisites
To connect to a Neo4j instance, you will need the following information:

The database URI
The port number
The protocol
Your username for the database
A text file containing your Neo4j password (the file should contain nothing else)

## Starting Up
To start the application, run the following command from the project directory (the directory containing the arrows subdirectory):

You’ll be prompted to enter your database details. Once verified, you’ll be taken to the main menu screen where you can begin using the application.

## Model Conversion
The conversion process is simple. Select the models you’d like to convert, and the program will handle the rest. The default schema used is L3V2.7-9.json.

The application uses libsbml to check for errors in the models. Models containing errors will not be processed. If you wish to change the schema, modify the self.schema_file variable in database_populator.py.

## Step-by-Step Guide

Uploading Models: Click the “Upload Model” button on the main screen, select the SBML file, and the system will begin processing it with a progress bar.
Searching the Graph: Enter the compound or process in the search bar to find relevant nodes and connections.
Comparing and Merging Graphs: After uploading multiple models, use the “Compare Graphs” feature to assess similarities. Click “Merge Graphs” to consolidate the data if needed.
Exporting Results: Once analysis is complete, users can export the graph data in a suitable format for further research or publication.

## Contributing

We welcome contributions to BioGr! If you have suggestions or improvements, please fork the repository and submit a pull request.

## License

No official license for this project, contact UCT IT department for further deatils
