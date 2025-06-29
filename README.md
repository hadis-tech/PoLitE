# PoLitE
AI-Enhanced Litter Pollution Mapping: Integrating Citizen Science with Geospatial and Social Data
This repository contains the Python implementation of the method described in our paper:
(Submitted to Science of the Total Environment)

The code enables standardisation, clustering, and enrichment of citizen-reported litter data using artificial intelligence, spatial analysis, and demographic datasets.

📊 Overview
This project integrates data from Marine Debris Tracker and Litterati to build a unified, enriched dataset of litter observations across the UK.
Key steps include:

Material Classification: Assigning standard material labels to litter items.

Material-Based Clustering: Grouping items within 200-meter radii by material type.

Amenity Association: Linking litter clusters to nearby amenities using OpenStreetMap.

AI-Powered Tie-Breaker Logic: Resolving ambiguous amenity assignments based on litter material.

Demographic Enrichment: Associating clusters with population and health data from the 2021 UK Census.

Below is a diagram illustrating the workflow:
PoLitE Diagram.png

🛠 Files
This repository includes the following Jupyter Notebooks:

File Name:	Description
1- Find_All_Amenities-G.ipynb:	Extracts and processes amenities from OpenStreetMap

2- Amenity_Category-G.ipynb:	Categorizes amenities into 13 types using AI-powered rules

3- Litter-Categorize_Center_Material-G.ipynb:	Performs material-based clustering of litter observations

4- Find_Amenity_based_on_Material_Center-G.ipynb:	Links clusters to surrounding amenities with tie-breaker logic

5- Find_OA_&_Population_&_per-G.ipynb:	Enriches clusters with demographic and health indicators

Each script corresponds to a step in the workflow described in the paper.

💾 Installation
Clone this repository:

git clone https://github.com/yourusername/your-repository.git

cd your-repository

Create a Python environment (optional) and install dependencies:

pip install -r requirements.txt

Typical dependencies include:

pandas

numpy

geopandas

scikit-learn

folium

matplotlib

nltk

osmnx

Please refer to each notebook for specific requirements.

🚀 Usage
You can run each notebook in sequence:

1️⃣ Material and Amenity Data Extraction
2️⃣ Amenity Categorization
3️⃣ Material Clustering
4️⃣ Amenity Association
5️⃣ Demographic Enrichment

Outputs include enriched datasets ready for analysis and visualization.

📄 Citation
If you use this code or reproduce our results, please cite our work:

Rezaei, H., Roberts, K. P., Arabikhan, F., et al. 
AI-Enhanced Litter Pollution Mapping: Integrating Citizen Science with Geospatial and Social Data.
Science of the Total Environment, 2025.

🔗 Links
Marine Debris Tracker: https://debristracker.org/
Litterati:https://opendata.litterati.org/
OpenStreetMap:https://www.openstreetmap.org/#map=5/55.79/-5.98

📝 License
This project is released under the MIT License.
Please see LICENSE for details.

🤝 Acknowledgements
We thank citizen scientists who contributed data and the University of Portsmouth for supporting this research.
