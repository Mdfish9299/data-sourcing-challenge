# NASA CME and GST Data Analysis

## Description
This project involves fetching and analyzing data related to Coronal Mass Ejections (CME) and Geomagnetic Storms (GST) from the NASA DONKI API. It's divided into three parts:

1. **Requesting CME Data**
2. **Requesting GST Data**
3. **Merging and Cleaning Data for Export**

## Project Structure
- **data/**: Directory for storing the final CSV file.
- **scripts/**: Contains Python scripts for data retrieval, processing, and merging.
- **README.md**: This file.
- **.env**: NASA_API_KEY="S3Os8PElSF4b1tv2VgJiID2wA07fOtRlllbRGQQ5"

## Dependencies
- Python 3.x
- `requests`
- `pandas`
- `json`
- `python-dotenv`

## Usage

### Setup
1. Ensure Python and required libraries are installed.
2. Add your NASA API key to a `.env` file in the project root:


### Execution
1. **Part 1**: Fetch CME data.
2. **Part 2**: Fetch GST data.
3. **Part 3**: Merge, clean, and export data to `data/` directory.

## Key Steps

### Part 1: CME Data
- Construct `query_url_CME` with parameters.
- Fetch, convert to JSON, process into DataFrame.
- Expand linked events, extract GST activity IDs.

### Part 2: GST Data
- Construct `query_url_GST`, fetch, and process data.
- Extract CME activity IDs from linked events.

### Part 3: Data Merging and Export
- Merge datasets based on activity IDs.
- Calculate time differences between events.
- Export cleaned data to CSV.

## Notes
- Utilizes NASA DONKI API for both CME and GST data.
- The starter CSV was a reference for structure; the final CSV is generated independently.

## License
This work is for educational purposes and does not have a formal license.

## Contact
- **Email:** mr.elliotfisher@gmail.com
- **GitHub:** [\[Your GitHub Profile URL if applicable\]](https://github.com/Mdfish9299/data-sourcing-challenge.git)

**Important:** 
- This project was completed independently. No external code or data was used beyond the NASA API.