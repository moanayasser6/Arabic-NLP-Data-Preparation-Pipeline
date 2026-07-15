# Arabic Fatwa Dataset Preprocessing Pipeline

This project presents a complete preprocessing and data standardization pipeline for Arabic Islamic fatwa datasets collected from multiple Excel sources. The pipeline was developed to address common challenges in Arabic NLP datasets, including inconsistent schemas, missing values, duplicate records, text normalization, and retrieval-oriented document preparation.

The dataset was compiled from 21 Excel files originating from different fatwa sources. Since the files contained variations in column names, missing fields, and inconsistent formatting, a unified preprocessing workflow was implemented to transform all records into a standardized structure consisting of three core fields: title, question, and answer.

## Key Features

* Automatic discovery and loading of multiple Excel files.
* Standardization of heterogeneous column names into a unified schema.
* Handling of missing values and incomplete records.
* Automatic generation of missing titles from question text.
* Arabic text normalization.
* Arabic diacritics removal.
* Special character and formatting cleanup.
* Duplicate detection and removal.
* Retrieval document construction for information retrieval tasks.
* Long-document flagging to support future chunking workflows.

## Dataset Processing Workflow

1. Load and merge all Excel files.
2. Standardize column names.
3. Align all records to a common schema.
4. Handle missing values.
5. Generate missing titles when necessary.
6. Normalize Arabic text.
7. Remove Arabic diacritics.
8. Clean special characters and formatting artifacts.
9. Remove duplicate records.
10. Build retrieval-ready document representations.
11. Export the final cleaned dataset.

## Technologies Used

* Python
* Pandas
* NumPy
* OpenPyXL
* Regular Expressions (Regex)

## Output

The pipeline produces:

* clean_fatwas.xlsx
* clean_fatwas.csv

These outputs contain a unified and cleaned corpus of Arabic fatwas suitable for information retrieval experiments, search applications, and future NLP workflows.

## Project Outcome

After preprocessing and standardization, the final dataset contains more than 117,000 cleaned fatwa records collected from 21 source files. The resulting corpus provides a structured foundation for Arabic information retrieval, question answering, and other downstream NLP applications.

