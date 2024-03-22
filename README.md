# ReadME

## The landscape of preclinical neuroscience systematic reviews: an evidence map

Bernard Friedrich Hild, David Brüschweiler, Sophia Theodora Katharina Hild, Julia Bugajska, Marianna Rosso, Eva Furrer, Kim Elaine Wever, Benjamin Victor Ineichen

OSF Identifier: DOI 10.17605/OSF.IO/WX5TA


### Background
Background: There is an increase in animal systematic reviews. However, there is limited knowledge about their quality, scope, and geographical distribution over time. Objective: This study aimed to assess the quality and demographic trends of animal systematic reviews in neuroscience, including changes over time. Methods: We performed an umbrella review of animal systematic reviews, searching Medline and Embase for reviews until January 27, 2023. A validated data mining method was used to automatically evaluate the quality of these reviews. Results: From 18‘065 records identified, we included 1‘358 systematic reviews in our study. These reviews are widely used across diverse topics, often in translational research. They originate from 64 countries, with the United States, China, the UK, Brazil, and Iran being the most prolific. The automated quality assessment indicated high reliability, with F1-scores over 80% for most criteria. Overall, the reviews were of high quality and the quality improved over time. However, many did not include a pre-registered study protocol. Reviews with a pre-registered protocol generally scored higher in quality. No significant differences in quality were observed between countries. Conclusion: Animal systematic reviews in neuroscience are of overall of high quality. Our study highlights specific areas for enhancement such as the recommended pre-publication of study protocols. Such measures can contribute to the effective translation of animal research findings to clinical applications.
### Overview
This repository contains all the materials and data related to our study titled "The landscape of preclinical neuroscience systematic reviews: an evidence map,". The study assesses the quality and demographic trends of animal systematic reviews in neuroscience, identifying changes over time.
#### Study Selection and Data Extraction Process
The study utilized a two-phase screening and data extraction process. Initial screening of titles and abstracts was conducted using the web-based application Rayyan. Metadata extracted included titles, authors, publication year, journal, number of authors, study country, and author keywords. Quality and reporting metrics of systematic reviews were extracted using a custom-built R tool employing regular expressions for text matching. This tool is documented and available within this repository.
### Repository Content
#### Analysis Files
•	DataViz.Rmd: R Markdown file for data visualization, generating figures from alldata.csv.  
•	RoB Automated/1_lib_regex_sectionsFUN.R: Defines regular expressions for automated risk of bias (RoB) assessment and sections a paper into chapters.  
•	RoB Automated/2_pdfs_to_htmlFUN.R: Converts PDF files of research papers into HTML format for further processing.  
•	RoB Automated/3_Mining.R: Runs mining functions on HTML files to perform automated RoB assessments.  
•	RoB Automated/Mining_Validation.Rmd: Validates the automated RoB process, comparing it against manual assessments.  
#### Data Files
•	alldata.csv: Cleaned dataset used for analysis and visualization, containing detailed metadata for each study.  
•	Rob_predicted.csv: Contains automated RoB scoring for each study.  
•	validation_D.csv, validation_B.csv: Contain manual RoB coding for validation.  
•	Reliability_mining.csv: Accuracy metrics for automated vs. manual RoB assessments.  
•	Metadata: Detailed metadata file  
### Data Analysis
Analysis focused on trends in quality over time and differences based on the presence of a pre-registered study protocol. Statistical analyses were conducted using R, with details provided within the manuscript and the present repository.
### Usage Instructions
1.	Review the Metadata and the manuscript section of the publication.  
2.	For the automated risk of bias assessment: the R files 1_lib_regex_sectionsFUN, 2_pdfs_to_htmlFUN.R, 3_Mining.R should be run in this order. Further information regarding the outputs of each analysis file is detailed in the metadata.  
3.	To recreate the visualizations, please use the “DataViz.Rmd” file.
