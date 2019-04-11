Project Goal:  Assessment of the potential value of US county-level
data for studying deaths from heart disease and important factors
determining mortality rates related to heart disease.

Rationale:
600,000 deaths per year in US
$200 billion in losses due to heart disease
Existing studies provide insight but have not changed key behaviors.
County-level data provides a visually-compelling way to present the issues.

General approach:
1)  Collect raw data from various sources
2)  Identify key factors to study
	-- Smoking, obesity, diabetes, health insurance, access to food
	   and exercise, access to physicians, sunlight, pollution, 
	   drug use
3)  Clean and preprocess data
4)  Conduct regression analysis
5)  Create compelling visual graphics

This projects involves a large number of files and notebooks.  Due to file 
size, some files are saved on Google Drive.  The presentation is at:
https://docs.google.com/presentation/d/1MdTTWXT5h05ez_9__E2FJyCU1gtpvQeKJ2AsogndXJg/edit?usp=sharing

1) Collect raw data.
We collected hospital data from healthdata.gov.  This list had
county names and zip codes which enabled us to count hospitals (there
is a notebook in "Extra_Work") but once we found a better source
for physician density, we halted our efforts to count hospitals.
We collected drug use data from the National Drug Use Survey (Department
of Health and Human Services).  We found sunlight data from the 
North American Land Data Assimilation System.  We found an excellent
"treasure trove" of county data from a "Healthy Counties Rankings and
Roadmaps" program from the University of Wisconsin.  Mortality data
were downloaded from the CDC WONDER database.  The Healthy County
data had to be downloaded one state at a time, so we divided and conquered,
merging ten states at a time.  Because these individual tables were
quite short, they were merged together in MS Excel, and Pandas was
reserved for the large merged data sest.  

2) Identify key factors
To keep things reasonable, we settled on just 12 factors.  We aimed
for a mix of factors known to be related to heart disease (e.g. smoking)
and factors that might be related but are not recognized as such (e.g.
sunlight).  Drug use data was available only at the state level.

3) Clean and preprocess data 
The notebook "County_Data" and "County_data_remove_unreliable_label_1" were
used to develop the processing procedures with crude mortality rates and
methods to merge in all data sources.  Using "Merge_Age_Adjusted_Data_2"
notebook, the age-adjusted data were also added into the master data set.

4) Analyze data
Several notebooks were used, 
"Explore_Counties_3", "Data_Explore_2" and "Data_Explore_3" were
used for exploratory analysis and statistics.  "Data_Model_1" was used
to make the final statistical analyses.  

5) Visual graphics
We used plotly to create the county-level graphics, plus Adobe Illustrator
for shape layers, used Adobe AfterEffects for creating animations, and used
Adobe Premiere Pro for final editing of the footage.  The Jupyter notebooks
involved are labeled "Plotly=Copy1", "Plotly2ajg", and "Plotly3ajg"

To summarize the statistical output, we created a 3-D bar chart in Matplotlib
using the notebook "3D Bar Plot of Risk Factors"
