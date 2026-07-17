# Biofouling Record Book (BFRB)
*Official Living Ledger Imported from Vessel Master Spreadsheet*

The following ledger displays real-time logging data synchronized directly from the ship's operational Excel matrix (`_data/bfrb_data.csv`).

| Date | Location | Activity | Rating | Sign-Off |
| :--- | :--- | :--- | :--- | :--- |
{% for row in site.data.bfrb_data %}| {{ row.Date }} | {{ row.Port_Location }} | {{ row.Activity_Type }} | **{{ row.Fouling_Rating }}** | {{ row.Logging_Officer }} |
{% endfor %}

---
## 🔄 Excel Workflow for the Crew
1. Open the vessel's master logging spreadsheet in Microsoft Excel.
2. Add any new inspection or hardware checks to the bottom row.
3. Save the file as a **CSV (Comma Delimited)** named `bfrb_data.csv`.
4. Upload and replace the file directly inside the `_data/` folder on GitHub.

---
[← Return to Dashboard](/)
