# BiopREL Data Analysis Project

## 🎯 Summary of the project
This project is centered around the exploration and utilization of hydrogels, with a spotlight on methacryloyl salmon and porcine based gelatin-based microgels. The goal is to achieve controlled crosslinking densities and curcumin release profiles via a cutting-edge spray congealing system coupled with UV radiation. The project delves into the advantages of gelatin-based hydrogels in terms of biocompatibility, biodegradability, and the potential to modify mechanical properties through chemical crosslinking. A key part of this endeavor is the calculation of the Young Modulus to unravel the mechanical traits of these hydrogels, which is vital for their application in diverse domains like bioactive compound delivery in functional foods, pharmaceuticals, and tissue engineering, among others.

## 🐟 Salmon and Porcine Gelatin
Salmon and porcine gelatin are the foundation for creating GelMa (Gelatin methacryloyl) and, subsequently, hydrogels. The aim in this poject is to determine the intrinsic differences in the thermal and viscoelastic properties of these gelatins and their impact on the functionality and mechanical strength of the resultant hydrogels when mixing both gelatin sources. The project encompasses the preparation and characterization of gelatin suspensions by blending salmon (SG) and porcine (PG) gelatins at different weight fractions, followed by their functionalization to concoct GelMa with a variety of properties.

## 📊 How Data is obtained
The data treasure will be unearthed from a series of experiments encompassing the preparation and characterization of GelMa macrogels through the use of a rheometer and texturometer obtaining stress and stress data, that can later be utilized to determine the mechanical properties of the hydrogels or gelatin.

## 📈 Young Modulus
Diving into the calculation of Young's Modulus is quintessential to decoding the mechanical behavior of the hydrogels under varied conditions. This mechanical metric is crucial for tailoring hydrogels for specific applications, especially in scenarios requiring a fine balance between flexibility, strength, and elasticity. The correlation between the crosslinking densities, the source of gelatin (salmon or porcine), and the resultant Young's Modulus of the hydrogels will furnish a comprehensive insight into the mechanical properties of these hydrogels for their proposed applications. Through the juxtaposition of compressive modulus among hydrogels derived from different gelatin sources and crosslinking strategies, a clearer comprehension of how to optimize these materials for desired mechanical and functional outcomes will be achieved.

## 🐍 Data Processing using Python

1. **🛠 Initial Setup and File Selection**:
    - Import essential libraries:
    ```python
    import pandas as pd
    import numpy as np
    ```

2. **📦 Data Import, Aggregation, and Initial Viewing**:
    - Loop through each file, read based on their extensions (`.xls` or `.xlsx`), and log any reading errors.
    - Amalgamate data from each file into `master_df` a dataframe with stress and strain data.
    - Display `master_df` contents to view the aggregated data.

3. **🔄 Data Processing, Cleaning, and Filtering**:
    - Create `process_data_from_master_df(row)` to process each `master_df` row, extracting vital information.
    - Process each row using the defined function, convert to `final_df`.
    - Craft `data_cleaned` DataFrame by dropping rows with NaN values in 'Time' and 'Stress' from `final_df`.
    - Prepare for visualization: create 'Legend' column in `data_cleaned`, determine peak stress index, and create `filtered_df`.

4. **📊 Data Visualization**:
    - Employ visualization libraries:
    ```python
    import plotly.offline as pyo
    import plotly.graph_objects as go
    import matplotlib.pyplot as plt
    import seaborn as sns
    import plotly.express as px
    ```
    - Forge interactive visualizations:
        - **Stress vs. Time for All Data**: using cleaned data, color-differentiated by 'Set' and 'File Name' combo.
        - **Stress vs. Time**: using filtered data up to global peak time, color-varied based on the 'Legend' column.
    - Exhibit `final_df` and `data_cleaned` DataFrames in a tabular layout within a Jupyter notebook environment.

## 🔄 Next Steps
With the Python data processing and visualization steps delineated, the following phases will focus on the deeper analysis of the data, correlating the findings with the theoretical framework, and evaluating the implications of the results. The knowledge gleaned from the Young Modulus calculations, alongside the analysis of the crosslinking densities and curcumin release profiles, will be instrumental in steering the subsequent stages of this project.

## 🌐 Collaboration
This project is part of Fondecyt project in the BiopREL laboratory.

## 📬 Contact
For queries, suggestions, or collaborations, feel free to reach out. This project aims to cultivate a community of learners and innovators keen on advancing the understanding and application of hydrogels.

---

This project structure provides a blueprint for how the BiopREL Data Analysis Project is being undertaken. It encapsulates the initial objectives, the methodology for data acquisition and processing, and lays the foundation for subsequent analytical and developmental steps. Through a blend of theoretical understanding and practical application, the endeavor strives to unravel the potential of methacryloyl salmon gelatin-based microgels in various realms, underpinned by rigorous data analysis using Python.
