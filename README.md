# Emalahleni-twilight-forecast
A case study focused on my coal-dependant hometown.
## **The Twilight of Emalahleni's mining industry: A Macro-analysis** 📉⛏️

📖 ***Executive Summary***

eMalahleni (Witbank) has long held the undisputed throne as the heart of South Africa's coal industry. However, the geological and financial realities suggest that this era is coming to a hard stop much sooner than I anticipated.

This case study exposes that the region's collapse will not be purely geological. By mapping the remaining 3.8 billion tonnes of regional reserves against the Eskom power station decommissioning cliff and aggressive ESG-driven lending freezes from commercial banks, this project identifies the exact timeline where coal reserves structurally transform into stranded assets.

Since I was curious about the actual timeline, I decided to try and estimate just how long is this twilight era going to last. I am by no means trying to save the town or anything, I am just mapping out the timeline of this twilight as a soon to be graduate entering the workforce. Open the files below to see the data unfold.

📂 ***Repository Contents***

To get the full picture of this commercial thesis, please review the files:

[The Twilight of Emalahleni (Harry's forecast).pdf](https://github.com/user-attachments/files/29645136/The.Twilight.of.Emalahleni.Harry.s.forecast.pdf)

[Emalahleni_Twilight_Horizon.xlsx](https://github.com/user-attachments/files/29645148/Emalahleni_Twilight_Horizon.xlsx)


<img width="1661" height="970" alt="Screenshot 2026-07-03 190032" src="https://github.com/user-attachments/assets/6aa1330b-127c-42a3-938b-4cf43e395719" />
<img width="1657" height="1020" alt="Screenshot 2026-07-03 185801" src="https://github.com/user-attachments/assets/b2ff6947-22ca-4e07-8823-b8e8bd2b41e7" />

A look under the hood at the Python terminal during the execution of the serverless SQL architecture.

⚙️ **Technical Architecture** **(The Secret Sauce)**

To move this project beyond a static spreadsheet exercise, I engineered a fully automated ETL (Extract, Transform, Load) pipeline and relational data model using Python.

Instead of manually crunching numbers, I built a Python script that:

Extracted & Transformed: Used pandas to clean and ingest raw geological data spanning 81 operating mines in the Nkangala district.

Serverless SQL Modeling: Utilized sqlite3 to spin up an in-memory, serverless relational database. I designed a custom ESG Risk Matrix (dim_Commercial_Risk) based on actual banking phase-out dates and joined it with the geological data (fact_Operations).

Complex Querying: Executed custom SQL JOIN queries to mathematically filter and identify mines caught in the "Death Spiral" (reserves outliving their off-taker with zero access to private credit).

Automated Reporting: Utilized XlsxWriter to automatically export the SQL outputs, format the cells to a corporate standard, and plot native Excel charts directly into the final Emalahleni_Twilight_Horizon.xlsx master model.

📊 ***Data Sources & Acknowledgements***

This case study is built on real-world data and would not have been possible without the extensive reporting and tracking from the following organizations:

Global Energy Monitor - Global Coal Mine Tracker: The cornerstone of the geological data used in this model. Their tracker provided the exact production rates, reserve volumes, and workforce metrics for the Witbank/Highveld collieries. https://globalenergymonitor.org/projects/global-coal-mine-tracker 

Coaltech research association and their extensive report which helped me map out the data I needed to compliment my case study with the other sources that I used for this project. It provided vital industry-level context and operational baselines. Read their 2025 report here - [CoalTech-IAR-2025-Final.pdf](https://github.com/user-attachments/files/29645309/CoalTech-IAR-2025-Final.pdf)


Krutham Policy Brief: [From-dig-baby-dig-to-stranded-coal-assets.pdf](https://github.com/user-attachments/files/29645418/From-dig-baby-dig-to-stranded-coal-assets.pdf). This report provided the crucial macroeconomic context regarding the withdrawal of traditional capital (FirstRand, Investec, Nedbank) from the sector, allowing me to build the custom ESG Risk Matrix.

