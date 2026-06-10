Project Overview
Patient reviews are a valuable but underutilized resource in healthcare improvement. This project leverages data-driven methods -- including sentiment analysis, regression modeling, and clustering -- to extract actionable insights from real patient feedback at Saint Luke's BGC.
The findings align with UN Sustainable Development Goal 3: Good Health and Well-Being, specifically Target 3.8 (universal access to quality essential healthcare services), and support evidence-based policymaking in the Philippine healthcare sector.

Project Objectives

Identify key factors affecting healthcare quality evaluations
Analyze the relationship between patient feedback and service delivery
Assess the impact of staff performance on patient satisfaction
Examine how patient demographics influence healthcare quality perceptions
Evaluate the role of technology and facilities in quality assessments


Repository Structure
FileDescriptionFinal_Presentation.ipynbMain Jupyter Notebook -- full analysis pipelinefinal_presentation.pyPython script version of the notebookSt. Luke's BGC Reviews Dataset.csvRaw patient reviews datasetDS001_Python_Final_Project_Documentation.docxFull project documentation (Word)DS001_Python_Final_Project_Documentation.pdfFull project documentation (PDF)

Methodology
This project follows the CRISP-DM framework integrated with an NLP Workflow.
1. Data Collection and Loading

Loaded CSV dataset of patient reviews from St. Luke's BGC
Handled missing values and performed initial data profiling

2. Exploratory Data Analysis (EDA)

Distribution of star ratings (1-5)
Roberta sentiment distribution
Review length analysis with quantile visualization
Frequency of reviews over time
Sentiment vs. review length scatter analysis
Rating sentiment categorization (Positive / Neutral / Negative)
Confusion matrix comparing Roberta-predicted vs. rating-derived sentiments

3. NLP Text Preprocessing

Tokenization -- splitting reviews into individual words
Stop Word Removal -- filtering common non-meaningful words
POS Tagging and Lemmatization -- reducing words to their base forms using WordNet

4. Word Cloud Visualization

Generated word clouds for Positive, Neutral, and Negative review clusters

5. Machine Learning Models
ModelPurposeLogistic RegressionSentiment classification with TF-IDF featuresNaive Bayes (Multinomial)Comparative sentiment classification
Both models were evaluated using accuracy, precision, and classification reports.
6. KMeans Clustering

Applied the elbow method to determine optimal number of clusters (k=2)
Cluster 0 -- Reviews focused on emergency care, medical testing, and service timelines
Cluster 1 -- Reviews focused on staff performance, wait times, and overall hospital experience


Key Findings

Positive sentiments dominate reviews, but concerns about wait times and administrative inefficiencies are recurring themes
Cluster analysis reveals two distinct patient experience profiles: operational/functional concerns vs. broader service satisfaction
Logistic Regression and Naive Bayes models both achieved competitive accuracy in predicting sentiment from review text
Staff quality and cleanliness were consistently highlighted as strengths; cost transparency and delays were noted as areas for improvement


Technologies and Libraries
CategoryToolsLanguagePython 3Data Manipulationpandas, numpyVisualizationmatplotlib, seaborn, WordCloudNLPNLTK (tokenization, stopwords, lemmatization, POS tagging)Machine Learningscikit-learn (TF-IDF, Logistic Regression, Naive Bayes, KMeans)EnvironmentGoogle Colab

Alignment with SDGs and Government Priorities
AreaAlignmentUN SDG Goal 3Good Health and Well-BeingTarget 3.8Universal access to quality essential healthcare servicesGovernment PriorityHealthcare Quality Improvement and Evidence-Based Policy MakingTech IntegrationData-driven innovation in healthcare delivery

Authors
Developed as a final requirement for DS001 - Computer Programming 1 (Python)
at the Technological Institute of the Philippines, Quezon City
under Dr. Rosmina Joy M. Cabauatan | 1st Semester, SY 2024-2025
NameJosh Andrei A. IturaldeJuliana Ysabel EC. DeteraJames Andre L. KalawMia Ysabel R. SemillaEzra Paul P. Villa

License
This project is for academic purposes only. All rights reserved by the authors and the Technological Institute of the Philippines.
