# 🌱 Project XYZ

**Plant Health Monitoring** is an analytical tool developed to explore, analyze, and visualize plant sensor data. It features advanced multi-level encoding to capture interactions among abiotic and biotic stressors, delivering actionable insights for optimal plant care and management.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


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
   - Performed descriptive statistical analyses to understand basic data characteristics.
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
| **Understand how environmental factors influence plant health** | Matplotlib Histogram & Boxplot | Clearly displays data distribution, central tendencies, and variability, enabling easy interpretation of environmental influences on plant health. |
| **Develop a framework to evaluate cumulative stress effects** | Seaborn Bar Plot & Plotly Sunburst | Allows for intuitive visual comparison and exploration of multiple stressors and their cumulative impact on plant health. |
| **Provide clear, interactive visualizations for data-driven decisions** | Plotly Sunburst | Facilitates interactive and hierarchical data exploration, enabling stakeholders to make informed, data-driven decisions easily. |

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

**Styling**: Helped style and re-factor/ re-organize pipeline for better readability

**Design Thinking**: Supported visualization selection to enhance clarity and interpretability.

**Code Optimization**: Suggested efficient, readable, and optimized code structures


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

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* Dataset from Kaggle
* Plant physiology literature for threshold values and stress interactions


### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site

## Acknowledgements (optional)
* Thank the people who provided support through this project.