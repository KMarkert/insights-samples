# Route Registration Script

This script creates routes in Google Roads API from a CSV file.

## Prerequisites

- Python 3
- `requests` and `PyYAML` Python packages

## Installation

1.  Install the required packages:
    ```
    pip install requests PyYAML
    ```

## Configuration

1.  Open the `config.yaml` file.
2.  Set your Google Project ID in the `google_project_id` field.
3.  Configure the `csv_format` section to match your CSV file's structure.
    - Use `combined_coordinates` if your CSV has origin and destination in single columns.
    - Use `separate_coordinates` if your CSV has latitude and longitude in separate columns.
4.  (Optional) Set a `route_name_prefix` to be added to each route name.
5.  (Optional) Customize the `log_file` and `max_routes_to_create`.

## Usage

Run the script from the `route_registration_script` directory:

```
python3 create_routes_in_jurisdiction.py your_data.csv
```

Replace `your_data.csv` with the path to your CSV file.