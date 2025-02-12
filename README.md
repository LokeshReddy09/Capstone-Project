# CAPSTONE-PROJECT

# SpaceX Launch Dashboard

## Project Overview

The **SpaceX Launch Dashboard** is a data visualization tool built using **Dash** (a Python framework for building analytical web applications) to interactively explore and analyze SpaceX's launch history. It provides a user-friendly interface to visualize various metrics, including the success rates of SpaceX launches, payload impact, and comparisons across different launch sites. The dashboard is designed to give users insights into the historical performance of SpaceX launches and the relationship between payloads and launch success.

The key features of the dashboard include:
- Interactive visualizations such as pie charts, scatter plots, and sliders to dynamically explore launch data.
- Detailed analysis of launch success rates based on different criteria, including launch site and payload type.
- Comparisons of launch sites and their success rates.

## Project Structure

The project is organized into several folders for better organization and separation of concerns. Here’s a breakdown of the folder structure:

### Folder 1: `Data`
- **Purpose**: Stores the dataset used for visualization.
- **Contents**: 
   - `spacex_launch_dash.csv`: The primary dataset containing records of SpaceX launches. This dataset includes information such as launch date, success/failure status, launch site, payload details, etc.

### Folder 2: `App Code`
- **Purpose**: Contains the main code that launches the Dash application.
- **Contents**: 
   - `spacex_dash_app.py`: This is the central script that initializes the Dash application. It contains the layout of the dashboard and sets up the callbacks for interactivity.
   
### Folder 3: `Components`
- **Purpose**: Holds reusable components that can be included in the main application to enhance modularity and reduce redundancy.
- **Contents**: 
   - Various Python files that define custom Dash components such as charts, dropdowns, and other UI elements. These components can be imported and used in the main application to streamline the development process.

### Folder 4: `Callbacks`
- **Purpose**: Contains Python scripts that define the callbacks for interactivity within the dashboard.
- **Contents**:
   - Callback functions that link user actions (e.g., dropdown selections, slider movements) to changes in the dashboard’s visualizations. These functions will handle user input and update the plots accordingly.

### Folder 5: `Visualizations`
- **Purpose**: Includes Python scripts or figures for visual representation of the data.
- **Contents**: 
   - Pre-generated plots and figures that are used in the dashboard to represent launch data in various formats (pie charts, scatter plots, etc.). These scripts might contain the logic for creating these visualizations, which will then be rendered in the application.

### Folder 6: `Styles`
- **Purpose**: Contains the CSS stylesheets used to improve the user interface and the visual appeal of the application.
- **Contents**:
   - Custom CSS files to style the layout and individual elements in the dashboard. This can include color schemes, font choices, and element positioning to ensure a clean and professional look.

### Folder 7: `Documentation`
- **Purpose**: Stores documentation related to setting up, configuring, and using the application.
- **Contents**:
   - Detailed instructions on how to install the required dependencies, run the application, and customize it as needed. It also includes troubleshooting guides and any necessary background information on the dataset and its columns.

### Folder 8: `Main Application Code`
- **Purpose**: Contains the main script that launches the web application.
- **Contents**:
   - `spacex_dash_app.py`: This is the entry point of the application, responsible for initializing the app, setting the layout, and configuring the callback functions. Running this script starts the Dash app and makes it accessible via the web browser.

## Running the Application

Once the application is complete, you can run the application with the following command:

```bash
python spacex_dash_app.py
```

This will launch the Dash app locally on your machine. Open your web browser and navigate to the following address to access the dashboard:

```bash
http://127.0.0.1:8050/
```

The application will be displayed, allowing you to interact with the visualizations.

## Features

The dashboard provides several features to help users explore the launch data:

**Dropdown for Launch Site Selection**:
        Users can select different launch sites from a dropdown menu. The data and visualizations will be updated accordingly to reflect the chosen site.

**Pie Chart for Successful Launches**:
        A pie chart visualization shows the distribution of successful and unsuccessful launches, making it easy to compare the success rates.

**Payload Slider:**
        A slider allows users to filter launches based on payload values. This is helpful for analyzing how different payload sizes affect the launch success rate.

**Scatter Plot for Payload vs. Success:**
        A scatter plot displays the correlation between payload weight and launch success, helping to analyze how payload size influences the likelihood of success.
