# Website Form Autofill - UiPath Project

This project is a UiPath workflow designed to automate the process of filling up forms on any website. The workflow interacts with web pages, inputs required data into fields, and submits the form as necessary.

## Features

- Automatically navigates to the specified website.
- Detects form fields dynamically.
- Fills in predefined input values.
- Submits the form upon completion.
- Handles common errors such as missing fields or webpage loading delays.

## Prerequisites

1. **UiPath Studio:** Ensure you have UiPath Studio installed on your machine.
2. **Web Browser:** Supported browsers include Chrome, Edge, or Firefox (ensure the respective UiPath extension is installed).
3. **Input Data File:** A predefined source for form data (e.g., Excel or CSV file) if applicable.

## Setup and Configuration

1. Clone or download this repository to your local machine.
2. Open the `Main.xaml` file in UiPath Studio.
3. Configure the following variables:
   - `WebsiteURL`: URL of the target website.
   - `InputData`: Path to the input data file (if used).
   - Adjust selectors for specific form fields if required.

## How to Run

1. Open UiPath Studio and load the project.
2. Update the necessary arguments or variables in the workflow.
3. Test the workflow by running it in Debug mode.
4. Publish and run the automation to execute it on the target website.

## Workflow Overview

1. **Initialization**: Loads input data and initializes variables.
2. **Navigation**: Opens the browser and navigates to the specified website.
3. **Form Filling**: Detects and inputs data into the form fields.
4. **Submission**: Submits the form after all fields are filled.
5. **Completion**: Logs the status of the operation and handles errors gracefully.

## Dependencies

- UiPath.UIAutomation.Activities
- UiPath.System.Activities
- UiPath.Excel.Activities (if using Excel for input data)

## Customization

- Modify selectors for form fields to match the specific website.
- Adjust timeouts and retry mechanisms for better reliability.
- Add logic to handle captcha if present on the form.

## Troubleshooting

- **Selectors Not Working**: Ensure that the form field selectors are accurate and dynamic.
- **Browser Issues**: Verify that the UiPath extension is installed and enabled for the selected browser.
- **Data Input Errors**: Double-check the input data file for consistency and completeness.
