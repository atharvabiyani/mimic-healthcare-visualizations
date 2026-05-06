# MIMIC-III Healthcare Visualizations

Exploratory healthcare data visualization project using selected tables from the MIMIC-III clinical database. The notebook builds a concise visual summary of hospital operations, caregiver roles, procedure activity, discharge response delays, diagnosis patterns, and admission timing.

This project was originally completed for an AI in Healthcare course and has been cleaned up for portfolio use.

## Project Highlights

- Visualizes caregiver role distribution with a grouped pie chart.
- Analyzes callout acknowledgement delays after discharge-related requests.
- Compares procedure volume across hospital cost centers.
- Counts common diagnosis keywords such as sepsis, heart conditions, pneumonia, bleeding, and fractures.
- Creates a heatmap of hospital admission activity by weekday and hour.

## Repository Contents

```text
.
├── MIMIC_Visualization.ipynb       # Main analysis notebook
├── MIMIC_Visualization_Slides.pdf  # Companion presentation slides
├── README.md                       # Project overview and setup instructions
├── requirements.txt                # Python dependencies
└── .gitignore                      # Excludes local data, outputs, and environment files
```

## Data

This project expects four local CSV files from MIMIC-III:

- `ADMISSIONS.csv`
- `CAREGIVERS.csv`
- `CPTEVENTS.csv`
- `CALLOUT.csv`

The raw CSV files are intentionally not included in this repository because MIMIC-III contains sensitive clinical data and requires credentialed access through PhysioNet. If you want to reproduce the notebook, request access through the official MIMIC-III process and place the CSV files in the project root.

## Setup

Clone the repository and install the Python dependencies:

```bash
pip install -r requirements.txt
```

Then open the notebook:

```bash
jupyter notebook MIMIC_Visualization.ipynb
```

Before running the notebook, make sure the required MIMIC-III CSV files are available in the same folder as the notebook.

## Tools Used

- Python
- pandas
- NumPy
- seaborn
- Matplotlib
- Jupyter Notebook

## Notes

The notebook is designed as a focused visualization exercise rather than a predictive modeling project. The main goal is to communicate patterns in clinical operations data through clear, reproducible charts.
