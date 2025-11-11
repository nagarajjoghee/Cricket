# Automation Metrics Dashboard

A web-based dashboard for tracking and monitoring automation test metrics across multiple projects (REIM, RMS, ReSA, RPM).

## Features

- **Project Metrics Tracking**: Monitor test metrics for four projects: REIM, RMS, ReSA, and RPM
- **Comprehensive Metrics**: Track total test cases, pass/fail counts, execution time, pass rate, and execution dates
- **Historical Trends**: Visualize metrics over time with interactive charts
- **Data Persistence**: All data is stored locally in your browser using localStorage
- **Data Export/Import**: Export data as JSON or CSV, and import previously exported data
- **Responsive Design**: Works on desktop, tablet, and mobile devices

## Metrics Tracked

For each project, the dashboard tracks:
- Total automated test cases
- Pass count
- Fail count
- Execution time (in minutes)
- Pass rate percentage (automatically calculated)
- Last execution date

## Getting Started

1. **Open the Dashboard**
   - Simply open `index.html` in any modern web browser (Chrome, Firefox, Edge, Safari)
   - No server or installation required!

2. **Add Metrics**
   - Select a project from the dropdown (REIM, RMS, ReSA, or RPM)
   - Fill in the form with your test metrics:
     - Total Test Cases
     - Pass Count
     - Fail Count
     - Execution Time (in minutes)
     - Execution Date
   - Click "Add Metrics" to save

3. **View Dashboard**
   - The main dashboard displays the latest metrics for each project
   - Metrics are color-coded:
     - Green: Pass rate ≥ 80%
     - Blue: Pass rate 50-79%
     - Red: Pass rate < 50%

4. **View Historical Trends**
   - Scroll down to see interactive charts showing:
     - Total test cases over time
     - Pass rate trends
     - Execution time trends
   - Each project is represented by a different colored line

## Data Management

### Export Data
- **JSON Export**: Click "Export Data (JSON)" to download all metrics as a JSON file
- **CSV Export**: Click "Export Data (CSV)" to download metrics in CSV format for Excel

### Import Data
- Click "Import Data" and select a previously exported JSON file
- Imported data will be merged with existing data

### Clear Data
- Click "Clear All Data" to remove all stored metrics
- This action cannot be undone, so make sure to export your data first if needed

## Technical Details

- **Technology**: Pure HTML, CSS, and JavaScript (no frameworks required)
- **Storage**: Browser localStorage (data persists across sessions)
- **Charts**: Chart.js library (loaded via CDN)
- **Browser Compatibility**: Works in all modern browsers

## File Structure

```
/
├── index.html          # Main dashboard page
├── styles.css          # Styling and layout
├── script.js           # Data handling and chart logic
└── README.md           # This file
```

## Usage Tips

1. **Regular Updates**: Add metrics after each test execution to maintain accurate historical data
2. **Data Backup**: Regularly export your data to prevent loss
3. **Validation**: The form validates that pass count + fail count does not exceed total test cases
4. **Date Selection**: The execution date defaults to today, but you can select any past date for historical entries

## Notes

- Data is stored locally in your browser. Clearing browser data will remove all metrics
- Each browser profile has its own separate data storage
- For team sharing, export and share JSON files, or use a shared browser profile

## Support

For issues or questions, ensure you're using a modern browser and that JavaScript is enabled.

