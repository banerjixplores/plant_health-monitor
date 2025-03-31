# 🌱 Project XYZ

**Plant Health Monitoring** is an analytical tool developed to explore, analyze, and visualize plant sensor data. It features advanced multi-level encoding to capture interactions among abiotic and biotic stressors, delivering actionable insights for optimal plant care and management.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

![Status](https://img.shields.io/badge/status-active-brightgreen)


## 🧾 Dataset Content
The dataset contains data generated to simulate readings for monitoring plant health in agricultural settings. It includes several key environmental and biological indicators, such as temperature, humidity, soil moisture, pH, nutrient level, light intensity, and an overall health score. The data is structured to support research in plant health monitoring, enabling users to train AI models for predicting plant health status based on biosensor data.

 - Dataset Source: Kaggle Plant Health Monitoring
 - Content: Sensor data (soil moisture, temperature, humidity, light intensity, nutrient levels)
 - Labels: Plant health status (healthy/unhealthy), simulated biotic stress (disease, pests)
 - Size: Lightweight, suitable for local analysis

## 🧠 Business Requirements

The ultimate goal is to promote smart green cities, urban agriculture, and promote deforestation by having more positive control on plant-health.
* Understand how environmental factors influence plant health.
* Develop a framework to evaluate cumulative stress effects.
* Provide clear, interactive visualizations for data-driven decisions.

## 🧪 Hypothesis and how to validate?
1. Combined Stressor Impact
    - Hypothesis: Plants exposed to combined abiotic and biotic stressors experience higher health risks.
    - Validation: Visual comparison via category-specific plots and proportions.

2. Differential Impact of Stress Types
    - Hypothesis: Biotic stressors cause a more significant health decline compared to abiotic stressors.
    - Validation: Comparative visual analysis of biotic-only vs. abiotic-only stress scenarios.

3. Optimal Environmental Conditions
    - Hypothesis: Plants in optimal moisture, temperature, and humidity zones show better health outcomes.
    - Validation: Boxplots and heatmaps demonstrating health distribution across zones.

🌿 Level 1 Encoding (Binary stressor encoding)

- **Combined Stressor Impact:**  
  Plants under combined abiotic and biotic stress show higher average Total Stress Score (2.35), validating Hypothesis 1.

- **Differential Impact of Stress Types:**  
  Biotic stress had marginally lower mean score than abiotic, but combined stresses consistently resulted in higher stress and health decline.

- **Optimal Conditions:**  
  Not evaluated in Level 1.

---

🌿 Level 2 Encoding (Zone-based encoding)

- **Combined Stressor Impact:**  
  The bar plots and category proportions clearly show that combined stress conditions correspond to higher unhealthy plant proportions (~22%) compared to abiotic-only (~17%), biotic-only (~21%), and no-stress (~17%).

- **Differential Impact of Stress Types:**  
  Biotic-only stress category consistently showed slightly higher unhealthy proportions (21%) than abiotic-only (17%) and no-stress.

- **Optimal Environmental Conditions:**  
  Zonal visualization shows that:
  - Moisture: Optimal (17.6% unhealthy), High (21.7%), Low (15.2%)
  - Temperature: Optimal (17.5% unhealthy), High (19.2%), Low (13.5%)
  - Humidity: Optimal (17.6%), High (15.9%), Low (22.2%)
  - Light: Optimal (17.6%), High (13.2%), Low (17.9%)

  The unhealthy percentages drop noticeably in optimal and high zones, supporting Hypothesis 3.

- **Stress Category Shift:**  
  Zone-based encoding resulted in more plants falling under no-stress category (46.6%) compared to binary encoding (40.2%), providing a more nuanced stress identification.

- **Correlation Improvement:**  
  Higher correlations between total stress score and individual abiotic/biotic scores in Level 2 encoding suggest improved feature clarity.

---

## 📅 Project Plan
### High-Level Steps for Analysis:

1. **Data Collection and Loading**
   - Obtained raw data from a reliable Kaggle dataset.
   - Verified data quality and structure through initial exploratory checks.

2. **Data Cleaning**
   - Checked for duplicate entries and missing values to maintain data integrity.
   - Demonstrated missing value management using appropriate methods.

3. **Data Processing and Feature Engineering**
   - Implemented multi-level encoding strategies (binary, zone-based, combined interaction).
   - Calculated stress scores (abiotic, biotic, and total) to quantify plant stress conditions.
   - Generated new insightful features like Stress Category and Stress Fingerprint.

4. **Analysis and Visualization**
   - Created visualizations (Matplotlib, Seaborn, Plotly) to validate hypotheses and clearly illustrate findings.

5. **Interpretation and Reporting**
   - Derived meaningful insights correlating environmental factors and stressors with plant health.
   - Documented key results clearly, with a strong focus on visual communication for clarity.

### Data Management Throughout the Project:

- **Collection:**  
  Data was sourced from Kaggle, ensuring reliability and reproducibility.

- **Processing:**  
  Data was systematically cleaned, transformed, and encoded within a structured ETL pipeline, ensuring accuracy and consistency throughout all analytical steps.

- **Analysis and Interpretation:**  
  Managed processed data within clearly defined and intuitive feature-engineered datasets. Visual and statistical analyses were applied methodically to address clearly stated business requirements and hypotheses.

### Rationale for Research Methodologies Chosen:

- **Descriptive Analysis & Visualization:**  
  Selected to provide an intuitive understanding of data distribution and relationships between variables, facilitating easy interpretation and clear communication to stakeholders.

- **Multi-level Encoding Strategies:**  
  Chosen to effectively capture complex interactions between abiotic and biotic stressors, thus creating nuanced insights relevant for informed decision-making.

- **Interactive Visualizations (Plotly):**  
  Implemented to enable intuitive exploration of complex data structures by technical and non-technical audiences, thus empowering effective decision-making through visual analytics.

## 📊 The rationale to map the business requirements to the Data Visualisations

| Business Requirement | Chosen Visualisation | Rationale |
|----------------------|----------------------|-----------|
| **Understand how environmental factors influence plant health** | Matplotlib & Seaborn: Distribution plots, Boxplots, Correlation Heatmaps (Level 1 & 2) | Clearly illustrates the distribution and variability of microclimate variables and their relationship with plant health. Facilitates pre-encoding understanding and post-encoding analysis. |
| **Develop a framework to evaluate cumulative stress effects** | Seaborn Stacked Bar Plots, Matplotlib Pie Charts (Level 1 vs 2), Total Stress Distribution, Stress Category Comparison plots | Supports visual comparison between Level 1 (binary) and Level 2 (zone-based) encoding to validate hypotheses about combined stress effects and stress score behavior. |
| **Provide clear, interactive visualizations for data-driven decisions** | Plotly Scatter Plot, Pie charts | Enables interactive exploration of plant health in relation to encoded stress scores and categories, enhancing interpretability for data-driven decision-making. |

## 📈 Analysis techniques used

**Data Analysis Methods and Limitations** 

* Descriptive Analysis: Understanding data distribution and central measures.
    - Limitation: Limited ability to infer causation from observed correlations.
    
* Encoding Techniques: Binary, zone-based (pd.cut()), and interaction features.
    - Limitation: Synthetic dataset may limit real-world applicability.

* Visualization Techniques: Matplotlib, Seaborn, Plotly for dynamic and static visualizations.
    - Limitation: Complex interactions might require advanced statistical methods.

**Structure of Analysis Techniques**

- Methods structured in logical sequence to refine raw data progressively into actionable insights aligned clearly with business requirements.
- Feature engineering prioritized to effectively capture nuances in stress impacts.

**Data Limitations and Alternative Approaches**

- **Limitation**: Synthetic dataset lacks real-world variability and biotic stress complexities.

- **Alternative**: Simulated biotic conditions guided by literature to enhance realism and applicability.

**Generative AI Contributions**

**Ideation**: Helped formulate methods for encoding strategies, example pd.cut.

**Styling**: Helped style and re-factor/ re-organize parts of pipeline and README for better readability

**Design Thinking**: Supported visualization selection to enhance clarity and interpretability.

**Code Optimization**: Suggested efficient, readable, and optimized code structures

## Future Outlook

- Add interaction features (e.g., Abiotic × Biotic interactions).
- Add time-series simulation data (growth stages of plants).
- Integrate real-world biotic data sources (VOC sensors, pest databases).
- Create an interactive dashboard (Streamlit).
- Export visualization plots into an interactive web-based dashboard.
- Develop a CLI or automated script version of the ETL process for repeatability.
- Build a simple classification model to predict health status of plants based on available features. Future work could involve hyperparameter tuning, exploring other classification algorithms, or incorporating additional data sources to enhance the model's performance.


## ⚖️ Ethical considerations
* Dataset anonymized; synthetic biotic data ethically generated based on plant physiology literature.
* No identifiable or sensitive data included.

## 🐞 Known Issues
* Biotic stress data may require calibration with real-world conditions.
* More datapoints required to validate correlations and hence hypotheses.
* More factors need to be taken into account to explore nonlinear relations between stress flags and plant health.

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.


## 🛠️ Main Data Analysis Libraries
* pandas
* numpy
* seaborn
* matplotlib
* plotly
* os

## Credits 

### Content 

* Dataset from Kaggle
* Plant physiology literature for threshold values and stress interactions

### Media

- CI logo from Code Institute

## Acknowledgements (optional)
* Thanks to Vasi for facilitating all the resources and clear instructions for
conducting this standalone project.
* Thanks to John's interactive coding sessions on coding, and recapitulating
the concepts through practical examples during the Data Coach sessions, and to 
Niel's SME sessions
* Last, but not the least, to my colleagues in this Cohort :)