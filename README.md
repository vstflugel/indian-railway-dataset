# Indian Railway Stations Dataset

## Overview

This dataset contains a list of all railway stations in India, including station codes, station names, and region codes. It is a comprehensive resource useful for various applications like transportation analytics, geographic studies, mapping, and machine learning projects.

---

## Table of Contents

- [Dataset Overview](#overview)
- [Dataset Structure](#dataset-structure)
- [Usage](#usage)
- [How to Contribute](#how-to-contribute)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Dataset Structure

The dataset is provided in **JSON** format with an array of objects, where each object represents a railway station.

### Example JSON Format:

```json
[
  {
    "station_code": "A",
    "station_name": "ARMENIAN GHAT CITY",
    "region_code": "SE"
  },
  {
    "station_code": "AA",
    "station_name": "ATARIA",
    "region_code": "NE"
  },
  {
    "station_code": "AABH",
    "station_name": "AMBIKA BHAWALI HALT",
    "region_code": "EC"
  }
]
```

## Keys in the JSON:

- **station_code**: A unique identifier for each railway station (e.g., "A", "AA", "AABH").
- **station_name**: The name of the railway station (e.g., "ARMENIAN GHAT CITY", "ATARIA").
- **region_code**: The region to which the station belongs (e.g., "SE", "NE", "EC").

---

## Usage

You can use this dataset for:

- **Transportation Analysis**: Analyze railway stations' distribution, connectivity, and regional coverage.
- **Geographic Studies**: Map railway stations across India using their coordinates and regional data.
- **Machine Learning**: Incorporate station data in predictive models or recommendation systems related to transportation.
- **Mapping and Visualization**: Visualize Indian railway stations and their connections in geographical mapping software.

---
## How to Contribute

If you’d like to contribute to this dataset, here’s how you can help:

- **Data Updates**: If you find any missing or incorrect data, feel free to fork the repository and submit a pull request with the necessary corrections or updates.
- **Improvements**: You can enhance the dataset by adding new columns (such as geographical coordinates) or improving the data format.
- **Documentation**: Help improve the documentation or contribute ideas on how the dataset can be made more useful.

---

## Steps to Contribute:

1. **Fork the repository**.
2. **Make your changes or improvements** in a new branch.
3. **Submit a pull request** with a clear description of the changes.

## Example of how to load the dataset:

If you want to load and use the dataset in **Python** (using `json` module), here's how you can do it:

```python
import json

# Load the JSON dataset
with open('railway_stations_india.json', 'r') as file:
    data = json.load(file)

# Display the first few stations
for station in data[:5]:  # Displaying first 5 stations
    print(f"Station Code: {station['station_code']}, Station Name: {station['station_name']}, Region Code: {station['region_code']}")

```

## License

This dataset is shared under the [MIT License](LICENSE).

You are free to use, modify, and distribute this dataset as long as you include proper attribution.

---

## Acknowledgements

This dataset was created from public data sources of IRCTC and contributed by Vaibhav Singh Tomar.

If you found this dataset useful, consider sharing it or giving credit when using it in your own work.

