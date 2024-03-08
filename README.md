# BiopREL Data Analysis Project

## 🎯 Summary of the project
This project explores the development and analysis of hydrogels, focusing on methacryloyl derivatives from salmon and porcine gelatin (GelMa). Our objective is to control the crosslinking densities and study the release profiles of curcumin, which could have significant implications in bioactive compound delivery systems. This research is pivotal for advancing applications in functional foods, pharmaceuticals, and tissue engineering, with a particular emphasis on optimizing the Young Modulus to tailor the hydrogels' mechanical properties.

## 🐟 Salmon and Porcine Gelatin
The core of this project lies in comparing salmon (SG) and porcine gelatin (PG) to create GelMa hydrogels. By understanding the thermal and viscoelastic differences between SG and PG, we can fine-tune the hydrogels' mechanical strengths and functionalities. The methodology includes blending these gelatins in various ratios, followed by UV-induced crosslinking to fabricate hydrogels with diverse properties.

## 📊 How Data is obtained
Data is sourced from experimental setups involving rheometers and texturometers, which measure the stress and strain of gelatin macrogels. This empirical data forms the foundation for analyzing the mechanical characteristics of the developed hydrogels.

## 📈 Young Modulus
The Young Modulus calculation is crucial for understanding the elasticity and strength of hydrogels, impacting their suitability for different biomedical applications. We analyze how varying crosslinking densities and the origin of gelatin affect the hydrogels' Young Modulus, providing insights into their mechanical adaptability.

## 🐍 Data Processing using Python

### 🛠 Initial Setup and File Selection
- **Libraries Imported**:
  - `matplotlib.pyplot`: For plotting graphs and visualizing data trends.
  - `pandas`: Essential for data manipulation and analysis.
  - `ipywidgets`: Creates interactive elements in Jupyter notebooks.
  - `PyQt5.QtWidgets`: Facilitates file selection dialogs in the notebook environment.
  - `winsound` and `time`: Used for notification sounds and time tracking during data processing tasks.

### 📦 Data Import, Aggregation, and Initial Viewing
- **Data Handling**: Scripts automate the import of data from various file formats, compiling them into a master DataFrame. This initial aggregation phase is crucial for subsequent analysis phases.
- **Initial Data Checks**: Quick visualizations and summaries help identify data inconsistencies or missing values right after import.

### 🔄 Data Processing, Cleaning, and Filtering
- **Outlier Removal**: Utilizes statistical methods (e.g., IQR) to identify and exclude outliers, ensuring the reliability of subsequent analyses.
- **Data Transformation**: Transforms raw data into a structured format, suitable for in-depth analysis and comparison between different test conditions.

### 📊 Data Visualization
- **Visualization Techniques**: Leverages libraries like `plotly` for interactive plots and `matplotlib` and `seaborn` for static visualizations. These tools are instrumental in analyzing stress vs. time relationships and other critical parameters.
- **Insights and Patterns**: By visualizing data, we can uncover underlying patterns and relationships that are not immediately apparent from raw datasets, aiding in hypothesis testing and model building.

## 🔄 Next Steps
Armed with the processed and visualized data, the next phase involves deeper statistical analysis and theoretical modeling. The ultimate goal is to correlate empirical data with theoretical frameworks, optimizing hydrogel formulation for targeted applications.

## 🌐 Collaboration
This initiative is part of the broader Fondecyt project within the BiopREL laboratory, aiming to foster a collaborative environment for students and researchers passionate about biomaterials.

## 📬 Contact
We encourage anyone interested in hydrogel research or looking for collaboration opportunities to reach out. This project is a platform for shared learning and innovation in biomaterials science.

## 👥 Team 
- Francisco Kirhman 

## 🚀 Getting Started

To begin working with the BiopREL Data Analysis Project, please follow these instructions:

1. **Clone the repository to your local machine:**
   ```bash
   git clone https://github.com/FranciscoKirhman/BiopREL-Data-Analysis-Project.git
   ```

2. **Open the cloned repository in your preferred development environment:**

   - **For Visual Studio Code users:**
     Navigate to the cloned directory and open it with Visual Studio Code:
     ```bash
     cd BiopREL-Data-Analysis-Project
     code .
     ```

   - **For Jupyter Notebook users:**
     Navigate to the `notebooks/` directory within the cloned repository and launch Jupyter Notebook:
     ```bash
     cd notebooks/
     jupyter notebook
     ```

3. **Install required Python packages:**
   Before running any code, ensure all necessary packages are installed. Use the following command in your terminal or command prompt:
   ```bash
   pip install -r requirements.txt
   ```

4. **Running the project:**
   You can now run the notebooks directly within Jupyter Notebook or execute Python scripts in Visual Studio Code. The project is configured to use data directly obtained from a rheometer, allowing immediate analysis of real experimental data.

**For any issues or additional questions, please contact Francisco Osorio at [francisco.osorio@ug.uchile.cl](mailto:francisco.osorio@ug.uchile.cl).**
