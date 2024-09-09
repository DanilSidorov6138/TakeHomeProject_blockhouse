# Dashboard Application

## Overview

This Dashboard application provides interactive charts and data visualization features, including Line, Bar, Pie, and Candlestick charts. The application fetches data from an API and displays it using Chart.js and its extensions.

## Libraries and Tools

- **React**: A JavaScript library for building user interfaces.
- **Chart.js**: A powerful JavaScript library for creating charts.
- **chartjs-chart-financial**: An extension for Chart.js to support financial charts like Candlestick charts.
- **React Chart.js 2**: A wrapper to integrate Chart.js with React.
- **Chart.js Adapter Moment**: For handling date-time in charts.
- **TypeScript**: A superset of JavaScript that adds static types.
- **axios**: A promise-based HTTP client for making API requests.

## Setup and Running the Application

### Prerequisites

- Node.js and npm (or yarn) must be installed on your machine.

### Installation

1. **Navigate to the Project Directory**
    in django-backend/dashboard_project
    
    Make Sure to have django and djangorestframework and corsheader installed
    if not pip3 install django djangorestframework django-cors-headers

    if nodejs is not latest version install from here: https://nodejs.org/en

    TAKE HOME PROJECT/frontend/
   - npm install or yarn install

   TAKE HOME PROJECT/frontend/frontend-dashboard
   - npm install or yarn install



2. In TAKE HOME PROJECT/frontend/frontend-dashboard run using 

npm run dev

In TAKE HOME PROJECT/django-backend/dashboard-project run using
python3 manage.py migrate
python3 manage.py runserver 


Open Your Browser

Go to http://localhost:3000 to view the application in your browser.

Fetching Data
The application fetches chart data from the following API endpoints:

Line Chart Data: http://127.0.0.1:8000/api/line-chart-data/
Bar Chart Data: http://127.0.0.1:8000/api/bar-chart-data/
Pie Chart Data: http://127.0.0.1:8000/api/pie-chart-data/
Candlestick Chart Data: http://127.0.0.1:8000/api/candlestick-data/
Ensure that your API server is running and accessible at these endpoints.

Approach and Thought Process
Chart Components

LineChart: Displays time-series data using line graphs. Supports various data sets and customization options for visual appearance.
BarChart: Visualizes categorical data with bar graphs. Supports stacking and color customization.
PieChart: Represents data as a pie chart, useful for showing proportions.
CandlestickChart: Shows financial data using candlestick charts, facilitated by the chartjs-chart-financial extension.
Data Handling

Data is fetched asynchronously from API endpoints and managed using React’s useState and useEffect hooks, ensuring dynamic updates of the charts based on the latest data.

Styling

Basic styling is applied to make the charts responsive and visually appealing. The chart-box class includes hover effects for enhanced user interaction.

Error Handling

Basic error handling is implemented to catch and log any errors encountered during data fetching.

Notes
Ensure that your API server is correctly configured and running to provide data for the charts.
For further customization or development, refer to the individual chart component files in the components directory.
Feel free to reach out if you have any questions or need further assistance.


