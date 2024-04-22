
# Retail Analysis Project

Welcome to the Retail Analysis project repository. This project manages retail data involving customers and orders, focusing on delivering insights through data transformation and analysis in a structured big data environment. We have set up the project to handle different stages of development and testing through designated environments.

## Project Environments

The project is configured to run under three distinct environments to ensure robust testing and reliable deployment:

- **Development (DEV)**: Used by developers for day-to-day development tasks and initial testing phases.
- **Production (PROD)**: The live environment where the production-ready code is deployed.
- **User Acceptance Testing (UAT)**: Used for pre-production testing to ensure the new features behave as expected before they are moved to production.

## Project Structure

The codebase is organized into several key Python modules:

- **DataReader.py**: This module handles all data loading operations. It is responsible for reading data files into the system, ensuring that data is correctly imported for further processing.

- **DataManipulations.py**: Contains all the data transformation logic. This module processes the raw data into actionable insights and prepares it for analysis, applying various transformations as per the project requirements.

- **Utils.py**: Provides utility functions that support data reading and manipulation tasks, including Spark session management and configuration handling.

## Testing

Unit testing is an integral part of our development process. We utilize `pytest` for this purpose:

- **test_retail_proj.py**: Contains all unit tests for our project. Each new feature undergoes rigorous testing to validate its functionality and ensure that it integrates seamlessly without affecting existing features.

## Running Tests

To run tests and validate the changes after adding new features, use the following command:

```bash
pytest test_retail_proj.py
```

This command executes all tests defined in `test_retail_proj.py`, ensuring that all functionalities meet their expected criteria before progressing through the development pipeline.

## Configuration

The project makes use of configuration files to manage settings across different environments. These configurations dictate how components like Spark sessions are initialized and where data files are located.

## Getting Started

To set up and run the project on your local machine, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   ```

2. **Navigate to the project directory**:
   ```bash
   cd RetailAnalysis
   ```

3. **Install dependencies** (ensure you have `pipenv` installed):
   ```bash
   pipenv install
   ```

4. **Activate the virtual environment**:
   ```bash
   pipenv shell
   ```

5. **Run the application** (substitute `<ENV>` with either `LOCAL`, `PROD`, or `UAT`):
   ```bash
   python application_main.py <ENV>
   ```


---


