# **Visualizing US Natural Disaster Declaration**

# **Problem Statement**

The frequency and intensity of natural disasters in the United States pose significant challenges to emergency management and resource distribution. This project visualizes historical disaster declaration data to identify geographic hotspots, temporal trends, and high-impact incident types to support better disaster preparedness and mitigation strategies.

# **Dataset Description**

The dataset consists of 68,542 records detailing federal disaster declarations in the US from 1953 to 2024 consisting total column of 24.
Dataset Name:
DisasterDeclarationsSummaries - Cleaned Dataset

The dataset contains federal disaster declaration records across U.S. states, including:

Key Columns Used

- declarationType – Type of declaration (DR, EM, FM)

- incidentType – Disaster category (Severe Storm, Flood, Hurricane, etc.)

- state – Affected state

- incidentBeginDate – Date disaster started

- incidentEndDate – Date disaster ended

- declarationDate – Date federal declaration was issued

- fyDeclared – Fiscal year of declaration

- designatedArea – County-level affected areas

- disasterNumber – Unique disaster identifier

Derived Columns & Measures

- Response Lag (Days): 
Calculated using DATEDIFF between incident begin date and declaration date.

- DR % (Major Disaster %): 
Proportion of DR declarations relative to total declarations.

- High Risk States Count (Top 25%): 
States in the top quartile of disaster frequency.

The dataset enables both descriptive and strategic disaster analysis.

# **Key Performance Indicators (KPIs)**

The KPIs were designed to move beyond reporting and support strategic decision-making.

Page 1 – Impact & Trend KPIs

- 1.Total Disaster Declarations

  - Measures overall disaster exposure scale.

- 2.Total States Affected

  - Indicates geographic spread of disasters.

- 3.Total Incident Types

  - Shows hazard diversity.

- 4.Most Frequent Disaster Type

  - Identifies dominant hazard category.

- 5.Latest Year Total Declarations

  - Monitors recent disaster activity.

Page 2 – Strategic Risk & Preparedness KPIs

- 1.Most Vulnerable State

  - State with highest disaster frequency.

  - Supports regional prioritization.

- 2.High Risk States Count (Top 25%)

  - Measures national exposure concentration.

- 3.DR % (Major Disaster %)

  - Severity indicator.

  - Target benchmark: 60%.

  - Trend tracked by fiscal year.

- 4.Avg Response Days

  - Operational efficiency metric.
    
  - Target benchmark: 3 days.
    
  - Tracks responsiveness of federal declaration.

- 5.Most Frequent Incident Type

  - Highlights dominant disaster category for mitigation focus.

# **Dashboard Pages**

## Page 1: US Natural Disaster Impact & Trend Analysis

Purpose:
To provide descriptive insights into disaster frequency, geographic distribution, and hazard composition.

Visuals Used:

- KPI Cards

- Trend line chart (Declarations by Year)

- Stacked bar (Incident Type by Year)

- Bar chart (Incident Type by Declaration Type)

- Map (State-level distribution)

- Slicers (Incident Type, Designated Area)

This page answers:

- What is happening?

- Where are disasters concentrated?

- Which types dominate?

- How have trends changed over time?

## Page 2: Strategic Risk & Preparedness Insights

Purpose:
To transform descriptive data into actionable risk and operational insights.

Visuals Used:

- KPI Cards (Vulnerability & Risk Spread)

- KPI Visuals (DR %, Avg Response Days with targets & trend axis)

- Bar chart (Total Disasters by State)

- Donut chart (Disaster Share by Type)

- Clustered bar (Incident Type by Declaration Type)

- Response time analysis by incident type

- Slicers (Fiscal Year, Declaration Type)

This page answers:

- Where should resources be prioritized?

- Are disasters becoming more severe?

- Is response time improving?

- Which hazard requires preparedness focus?

# **Key Insights**

1. Severe Storm is the most frequent disaster type across years.

2. Certain states (e.g., Texas) show consistently high vulnerability.

3. DR % exceeds the 60% benchmark, indicating rising disaster severity.

4. Disaster trends peaked around 2020 and show long-term fluctuation.

5. Average response time significantly exceeds the 3-day target, highlighting operational inefficiency.

6. Risk exposure is concentrated among a subset of high-risk states.

# **Recommendations**

# **Tools Used**

**Power BI:** Used for data cleaning, modeling, and dashboard development. Power Query helped transform and prepare the dataset for analysis. DAX was used to create key measures such as DR %, Avg Response Days, and risk-based KPIs. It enabled the creation of interactive visuals, maps, and slicers to analyze disaster trends and preparedness insights.

**Google Colab:** Used as the primary environment for data cleaning. Python (Pandas) scripts were executed in Colab to handle missing values, clean strings, and format the dates before exporting the final CSV for visualization.

**VS Code:** The primary Integrated Development Environment (IDE) used to write and run the Jupyter Notebooks and manage project documentation.

**Git:** Employed for version control to track changes in the data cleaning scripts and the README file.

**GitHub:** Used to store, manage, and share the project repository, ensuring the analysis is accessible and reproducible.
