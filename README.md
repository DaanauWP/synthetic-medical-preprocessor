# Synthetic Medical Data Preprocessing Pipeline

This repository contains a Python-based pipeline for preprocessing synthetic medical data generated via GAN (or Synthea). The pipeline transforms raw JSON files containing synthetic medical records into structured, validated data models, and extracts key event data for further analysis.

## Overview

The preprocessing pipeline extracts and standardizes various components of synthetic medical data, including:
- **Clinic Information:** Extracting clinic details and addresses.
- **Subscriber and Patient Information:** Validating and structuring patient demographics and addresses.
- **Payer and Claim Information:** Parsing billing, claim, and procedure details.
- **Event Data:** Extracting encounters, immunizations, conditions, and procedures into a tabular format.

By leveraging [Pydantic](https://pydantic-docs.helpmanual.io/) for data validation and [Pandas](https://pandas.pydata.org/) for data manipulation, the pipeline ensures the data is clean and ready for analysis.

## Features

- **Structured Data Models:** Uses Pydantic to define and validate data models.
- **Event Extraction:** Processes events such as encounters, conditions, and procedures.
- **Data Cleaning:** Utilizes Pandas to merge, clean, and export data into CSV format.
- **UUID Validation:** Checks for valid UUIDs to maintain data integrity.

## Requirements

- Python 3.7+
- [pandas](https://pypi.org/project/pandas/)
- [pydantic](https://pypi.org/project/pydantic/)
- Standard libraries: `json`, `uuid`, `datetime`, etc.
