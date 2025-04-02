

## README Summary

This document outlines the **Quality Assurance (QA) Test Plan** for the Endothon Finance website application. The goal of the QA process is to ensure the application accurately retrieves the correct financial data for businesses, based on their age, and handles the logic for businesses younger than five years by forecasting the missing data. The test plan is structured to verify both the functional and non-functional requirements of the application, with a focus on data accuracy, performance, and error handling.

### Key Objectives:
1. **Correct Data Retrieval**: The application should retrieve the last five years of financial data for businesses older than five years, excluding the current fiscal year. For businesses younger than five years, the application must use available historical data and forecast the missing data to complete the five-year span.
2. **Error Handling and Forecasting**: In cases where historical data is insufficient, the application should accurately forecast the financial data for the missing years.
3. **Performance**: The application must retrieve data within a 2-second response time to maintain a seamless user experience.

### Testing Focus:
- **Functional Testing**: Verifying the correct retrieval of historical data for businesses older than five years and the proper forecasting of data for businesses younger than five years.
- **Non-Functional Testing**: Ensuring the system performs within the required response time and that the modular structure supports future updates without disrupting functionality.
- **Testing Strategy**: The testing will begin with unit tests for individual components (historical data retrieval and forecasting logic), followed by integration tests to verify the combination of historical and forecasted data, and system tests to measure the overall performance under load.

### Out-of-Scope:
- The design or enhancement of the user interface and adding new features to the workflow are not part of this QA process. The focus is solely on correcting the data retrieval logic and forecasting functionality.
