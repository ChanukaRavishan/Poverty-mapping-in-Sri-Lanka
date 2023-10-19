# Poverty-mapping-in-Sri-Lanka
Mapping the spatial distribution of poverty using call detail records and remote sensing data

**Project Overview**
This project aims to map the spatial distribution of poverty using a combination of remote sensing data and call detail records. The analysis includes Principal Component Analysis (PCA) to calculate a ground truth variable, "pc_1", which serves as a proxy for poverty. Three spatial models were tested: Spatial Error Model, Spatial Lag Error Model, and Spatial Durbin Error Model. After careful evaluation, the Spatial Durbin Error Model was selected as the best-performing model.

Data Sources
Call Detail Records
"call_count"
"avg_call_duration"
"nighttime_call_count"
"avg_nighttime_call_duration"
"incoming_call_count"
"avg_incoming_call_duration"
"radius_of_gyration"
"unique_tower_count"
"spatial_entropy"
"avg_call_count_per_contact"
"avg_call_duration_per_contact"
"contact_count"
"social_entropy"
Remote Sensing Data
"travel_time_major_cities"
"population_count_worldpop"
"population_count_ciesin"
"population_density"
"aridity_index"
"evapotranspiration"
"nighttime_lights"
"elevation"
"vegetation"
"distance_roadways_motorway"
"distance_roadways_trunk"
"distance_roadways_primary"
"distance_roadways_secondary"
"distance_roadways_tertiary"
"distance_waterways"
"urban_rural_fb"
"urban_rural_ciesin"
"global_human_settlement"
"protected_areas"
"land_cover_woodland"
"land_cover_grassland"
"land_cover_cropland"
"land_cover_wetland"
"land_cover_bareland"
"land_cover_urban"
"land_cover_water"
"pregnancies"
"births"
"precipitation"
"temperature"
Analysis Workflow
Data Preprocessing: Combine call detail records and remote sensing data. Remove Grama Niladhari divisions(Gnds) with zero population. Log transformation of skewed variables. Calculate "pc_1" using PCA.

Model Selection: Test three spatial models - Spatial Error Model, Spatial Lag Error Model, and Spatial Durbin Error Model.

Model Evaluation: Compare model performance using appropriate evaluation metrics, considering the spatial autocorrelation in the data.

Model Selection: The Spatial Durbin Error Model was chosen as the best-performing model based on the Akike information criterion and Bayesian information criterion and its ability to capture spatial relationships in the data and provide accurate poverty estimates.

Mapping Poverty: Utilize the selected model to map the spatial distribution of poverty across Sri Lanka.

For any questions or assistance, please contact Chanuka at chanuka@lirneasi.net or Merl at merl@lirneasia.net

Acknowledgments
We acknowledge the sources of the data used in this analysis and express gratitude to all contributors who made this research possible.





