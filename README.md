---

# 📊 Data Analysis & Reporting Pipeline

This project is a **modular data analysis and reporting tool** built with Python. It automates the process of **cleaning datasets, visualizing key insights**, and **generating professional reports** in HTML, PDF, and Word formats.

---

## 🔧 Features

- **Data Cleaning:**
  - Detects and lists missing values.
  - Identifies and drops duplicate or constant columns.
  - Categorizes columns by data type (numeric, boolean, string, datetime).

- **Visualization:**
  - Generates box plots to visualize outliers.
  - Creates histograms and count plots for up to 6 selected columns.
  - Saves plots as images for reuse in reports.

- **Report Generation:**
  - Outputs reports in **HTML**, **PDF**, and **Word** formats.
  - Embeds visualizations and summary statistics into each report.

---

## 🚀 How to Run

1. **Install dependencies:**

```bash
pip install pandas matplotlib seaborn fpdf python-docx
```

2. **Run the script:**

```bash
python your_script_name.py
```

3. **Follow the prompts:**
   - Enter the path to your CSV file.
   - Choose your preferred report format: `html`, `pdf`, or `word`.

---

## 🧪 Example Columns for Visualization

You can customize the columns to visualize by editing this line in the script:

```python
selected_columns = ['AGE', 'TENURE_IN_MONTHS', 'CLOSESTSTOREDISTANCE', 'STATE',
                    'PRIVATELABELTENDERFLAG', 'MDAYREV_L1Y']
```

---

## 📁 Output

The following files will be generated depending on your choices:

- `distribution_plots.png`
- `data_analysis_report.html`
- `data_analysis_report.pdf`
- `data_analysis_report.docx`

---

## 🛠 Technologies Used

- **Pandas** – Data manipulation
- **Matplotlib & Seaborn** – Visualization
- **FPDF** – PDF generation
- **python-docx** – Word document creation

---

## 📌 Notes

- Make sure your dataset is clean enough to parse. Datetime and boolean detection is based on column type.
- Ensure the image path (`distribution_plots.png`) is accessible when exporting to Word or PDF.

---
