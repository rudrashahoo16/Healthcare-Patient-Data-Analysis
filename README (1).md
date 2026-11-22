# Healthcare Patient Data Analysis

A beginner-friendly Python data analysis project that explores synthetic patient records and medical appointment data.

## Project objectives

- Handle missing age and test values.
- Remove duplicate patient records.
- Create age groups.
- Calculate BMI and create BMI categories.
- Visualize patient distribution and appointment status.
- Export a cleaned CSV file.

## Files

| File | Description |
|---|---|
| `Healthcare_Patient_Data_Analysis.ipynb` | Jupyter Notebook containing the full analysis |
| `patient_data.csv` | Synthetic raw dataset with missing values and duplicate rows |
| `README.md` | Project documentation |

The notebook creates `cleaned_patient_data.csv` after it is run.

## Tools and libraries

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Setup

1. Clone or download this repository.
2. Open a terminal in the project folder.
3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

4. Start Jupyter:

```bash
jupyter notebook
```

5. Open `Healthcare_Patient_Data_Analysis.ipynb` and run all cells.

## Dataset columns

| Column | Description |
|---|---|
| `patient_id` | Synthetic patient identifier |
| `age` | Patient age (some values are missing) |
| `gender` | Gender category |
| `height_m` | Height in metres |
| `weight_kg` | Weight in kilograms |
| `test_value` | Example numeric test value (unit intentionally unspecified) |
| `department` | Hospital department |
| `appointment_date` | Appointment date |
| `appointment_status` | Completed, Cancelled, or No-show |

## Data-cleaning approach

- Exact duplicate rows are removed with `drop_duplicates()`.
- Missing numeric values are filled with the median.
- Age groups are created using `pandas.cut()`.
- BMI is calculated as `weight_kg / height_m²`.
- BMI categories use common adult descriptive ranges. These are not appropriate for interpreting children's BMI.

## Visualizations

The notebook generates:
1. Patient distribution by gender.
2. Patient distribution by age group.
3. Patient distribution by BMI category.
4. Appointment status distribution.

## Privacy and responsible use

**All records in `patient_data.csv` are synthetic and generated for learning purposes.** They do not represent real people or real clinical measurements. Do not use this dataset or this notebook for diagnosis, treatment, or other clinical decisions. For real healthcare data, follow applicable privacy, security, consent, and governance requirements.

## Author

Rudra
