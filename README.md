Karamoja Food Security

🔗 Interactive Dashboard (Tableau Public): https://public.tableau.com/views/group5finalproject/districtmap?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

Project Overview
Karamoja, in northeastern Uganda, faces food insecurity due to drought, pests, and low crop productivity. Maize and sorghum are the region’s staple crops, but their performance varies widely across subcounties and districts. This project develops an interactive Tableau dashboard for NGOs. It enables exploration of crop yields, production, and population pressure to inform data-driven decisions for interventions.

Objectives
Compare sorghum vs maize yields at district and subcounty levels.
Highlight spatial disparities in food security risk.
Provide visual insights using interactive dashboards and charts.
Recommend targeted strategies to improve resilience and crop productivity.

Data Sources
Shapefiles
Uganda District Boundaries
Uganda Subcounty Boundaries
Crop Maps (Sorghum, Maize)

Tables
Yields & Population per Subcounty
Yields & Population per District

Key Variables
S_Yield_Ha → Sorghum yield (Kg/Ha)
M_Yield_Ha → Maize yield (Kg/Ha)
POP → Subcounty/District population
S_Prod_Tot / M_Prod_Tot → Total production (Kg)
Crop_Area_Ha, S_Area_Ha, M_Area_Ha → Area under cultivation

Tools & Methods
Tableau → interactive dashboards & visualizations
Data Blending & Joins→ shapefiles + crop & population tables
Calculated Fields → per capita yields, productivity ratios, crop share
Interactive Parameters → view results by district or subcounty
Visualizations → crosstabs, maps, combo charts, scatter plots, bins, sets
Python (Colab) → hypothesis testing & predictive modeling

Dashboards & Worksheets
Dashboards
Karamoja Food Security Dashboard
Sorghum consistently outperforms maize across Karamoja.
Maps highlight disparities at district and subcounty levels.

Total Crop Production Dashboard
District-level comparison of crop output.
Kotido and Amudat lead in total production.

Crop Parameter Dashboard
Shows calculated metrics for maize & sorghum.
Highlights vulnerability of maize compared to sorghum.

Worksheets
Crosstabs → Crop areas & yields by district.
Yield Category → Maize vs sorghum yield per hectare.
Crop Parameter → Calculated metrics across districts.
Combo Chart → Relationship between population (POP) and crop area (Ha).
Population Bins→ categorization of districts by population size.
Total Crop Production → District-level total production.
District Sets (Top 10) → In/Out of top-10 producing districts.
Maize & Sorghum Production Total → Bar chart comparing totals.
Scatter Plot → Yields vs population with reference lines.
Heatmap → District-level yields (dark = higher).
Line Graph → Sorghum vs maize area against population.
Horizontal Bar → Total maize vs sorghum production.

Key Findings
Sorghum is more resilient – consistently higher yields and more reliable under drought.
Maize is vulnerable – yields fluctuate, especially in low-input areas.
Population pressure increases food insecurity in certain subcounties.
Strong disparities exist across districts.

Recommendations
Invest in Sorghum for Stability → prioritize seeds, fertilizers, and inputs in high-yield sorghum areas.
Target High-Population Subcounties → focus interventions where food insecurity is greatest.
Boost Maize Productivity → drought-tolerant varieties, irrigation, and better infrastructure.

Future Work
Integrate climate data (rainfall, temperature) with yield analysis.
Incorporate soil fertility & input usage to explain productivity gaps.
Scale dashboards to other Ugandan regions for national coverage.
Build predictive models for yield forecasting under climate/population scenarios.
Create a Food Security Index combining yield, population, and consumption.

X-Factor Contribution
Beyond Tableau, we extended the analysis in Google Colab (Python) to test hypotheses and build a simple predictive model.
Hypothesis Testing. We compared sorghum vs maize yields using an independent t-test.Result confirmed sorghum outperforms maize with statistical significance.

Predictive Modeling (Scikit-learn).We trained a simple Linear Regression model to predict maize production from maize area planted.

Visualization: 
Scatter plot (actual vs predicted) with regression line.
Slope ≈ X kg/Ha → every additional hectare of maize adds roughly X kilograms of production.
R² score indicated the model explained a strong portion of production variance.

This goes beyond correlation, showing how planners could forecast maize production from land allocation decisions.
