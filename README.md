## Part 1: Climate Data Analysis

Using SQLAlchemy ORM, Pandas, and Matplotlib, the following analyses were performed in `climate_starter.ipynb`:

- Precipitation Analysis:
  - Retrieved and plotted the last 12 months of precipitation data.
  - Summarized precipitation statistics.

- Station Analysis:
  - Counted total weather stations.
  - Identified the most active station.
  - Analyzed the temperature data for the most active station.
  - Created a histogram of temperature observations.

## Part 2: Climate Flask API

The `app.py` script creates a RESTful API with the following routes:

### Available API Routes

- `/`
  - Landing page that lists all available routes.

- `/api/v1.0/precipitation`
  - Returns JSON with date as the key and precipitation as the value for the last 12 months.

- `/api/v1.0/stations`
  - Returns a JSON list of all weather stations.

- `/api/v1.0/tobs`
  - Returns temperature observations (TOBS) for the most active station for the last 12 months.

- `/api/v1.0/<start>`
  - Returns min, max, and average temperature from the given start date to the end of the dataset.

- `/api/v1.0/<start>/<end>`
  - Returns min, max, and average temperature for the given date range.

## Requirements

- Python 3.7+
- Flask
- SQLAlchemy
- Pandas
- Matplotlib
- Jupyter Notebook

Install dependencies (if not already installed):

```bash
pip install flask sqlalchemy pandas matplotlib
