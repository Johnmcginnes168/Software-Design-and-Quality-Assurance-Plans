## Software Design and QA Testing Plans

This document provides a comprehensive overview of the **Software Design Plan** and **Quality Assurance (QA) Test Plan** for the Endothon Finance website application. The purpose of this project is to correct the data-gathering logic of the application, ensuring it retrieves the correct financial data based on the business’s age. If the business is younger than five years, the application should forecast the missing data to complete a full five-year financial profile. Both the software design and the QA plan focus on ensuring the application operates efficiently, performs as expected, and meets the functional and non-functional requirements.

### **Software Design Plan Overview:**
The Endothon Finance application collects financial data for businesses to generate a loan profile. However, a bug exists in the data-gathering logic, where the application incorrectly retrieves the first five years of financial data from the business’s establishment date instead of the last five fiscal years (excluding the current year). The design plan outlines the following objectives:

1. **Correct Data Retrieval**:
   - For businesses older than five years, retrieve the most recent five years of financial data, excluding the current fiscal year.
   - For businesses younger than five years, use available historical data and forecast future data to create a complete five-year financial profile.

2. **Forecasting and Error Handling**: Ensure that businesses younger than five years have their missing financial data forecasted correctly and handle errors if the application fails to gather the correct data.

3. **Modular Architecture**: Build the app with a modular architecture to enable easy updates and enhancements in future iterations.

4. **Agile Development**: Use an agile methodology to allow for iterative development and continuous testing to meet evolving business requirements.

### **Quality Assurance Test Plan Overview:**
The QA Test Plan ensures that the application meets both functional and non-functional requirements. The goal is to verify that the application retrieves the correct financial data, forecasts missing data for young businesses, and performs within the specified time constraints.

1. **Functional Requirements**:
   - Verify that the application retrieves the last five years of financial data for businesses older than five years.
   - For businesses younger than five years, ensure that the app correctly forecasts the missing years and generates a full five-year profile.
   - **Metrics**: Data accuracy, response time (within 2 seconds), and effective error handling.

2. **Non-Functional Requirements**:
   - **Performance**: Ensure that data is retrieved within 2 seconds.
   - **Scalability**: Confirm that the modular architecture supports future updates and enhancements without disrupting existing functionality.

3. **Testing Strategy**:
   - **Unit Tests**: Test individual components, such as retrieving historical data and forecasting for young businesses.
   - **Integration Tests**: Verify the combined functionality of data retrieval and forecasting.
   - **System Tests**: Measure system performance to ensure that the application meets the required response time under expected load.

4. **Out-of-Scope**:
   - Redesigning the user interface and adding new features to the workflow are not included in the scope of this QA process. The focus is solely on fixing the data retrieval and forecasting logic.

### **Key Goals Across Both Plans**:
- **Data Accuracy**: Ensure the application retrieves the correct historical data or forecasts future data accurately.
- **User Experience**: Maintain a smooth and efficient user experience by meeting the required performance (2-second response time).
- **Adaptability**: Ensure that the application’s modular structure allows for future scalability and enhancements without affecting core functionality.

This comprehensive approach will allow the Endothon Finance website application to function correctly and efficiently, fulfilling both current business needs and future expansion possibilities.

