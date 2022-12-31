============================================================================

PROJET/PURPOSE:

UDACITY - DATA SCIENTIST CAPSTONE project


============================================================================

TITLE:

DATA SCIENTIST PROJECT RELATED TO THE ANALYSIS OF HOSPITALIZATION DATA IN
 FRANCE DUE TO COVID-19 - Focus on my Region in Occitanie.


============================================================================

PROJECT DEFINITION


Project overview


The UDACITY DATA SCIENTIST CAPSTONE project consists in building a data
 science project of my choice with two deliverables:
 
 - A Github repository of my work;
 - A blog post written for technical audience (my choice).

Considering the rebound of COVID-19 cases in France these last weeks,
 I decided to analyze data of COVID-19 progress in France with figures
 directly reported by the hospitals via an institutional site.
 
1 - I will define the problem I want to solve.

2 - I will analyze this problem through visualization and data exploration
    to have a better understanding of the process to implement.
	
3 - I will implement the algorithms and metrics to solve this problem.

4 - I will collect my results and conclude to what extend I solve the
    problem.
	
5 - I will propose a blog post to document the steps or my work.


The Blog Post here-below gathers my work for this purpose.


Problem Statement

Description:

Using data from institutional site, I will focus my attention on the
 hospitalization, i.e. how COVID-19 fills our hospitals with new patients
 and the capacity of our hospitals to absorb these new patients.

Answering strategy:
I will monitor the hospitalization in the context of the population and
 the rate of people positive to the COVID-19 and the mortality. I will work
 at the scale of the department and even the region. My attention will be
 particularly focused on my department and my region.
The problem to solve consists in providing threshold on parameters to
 identify that would indicate when increase of hospitalization would
 significantly increase the risk of going in resuscitation or intensive
 care, or even the risk of death.

In that perspective, I will also try to propose a model for predicting
 the number of hospitalization.

Metrics
Description and justification:
For measuring efficiency of my solution, I propose using the R2 score
 as metrics.


============================================================================

DATA EXPLORATION

Workspace:

For this project, the initial analysis was realized through a Notebook.
 This Notebook like all related files are available in a dedicated Github
 repository (more information at the bottom of this post). I coded in Python
 3 mainly using Numpy and Pandas libraries.

 
Input data description:

I've gathered several data files reporting various information related to
 the epidemic of COVID-19 in France from the institutional web site:
https://www.data.gouv.fr/fr/datasets
The source web site indicates that data have been gathered along the time
 from various formats and contents. All the files used are under the License
 "Open Data Commons Open Database License (ODbL)".


============================================================================
 
Data access:

I downloaded the following data files the 29 December 2022. All data are
 stored in Github of this project.
 
Before running the code:

-	Refer to the README file

-	Refer to the Requirements file for knowing the required environment

-	Download the whole content of the dedicated Github repository on your
    workspace and update the variable ‘work_dir’ accordingly.


============================================================================

Data visualization:

Visualization related to data exploration:
AT this level, I'd like to merge all dataframes to benefit the maximum data
 to work on later. But is it possible?
My main concern, since I use data file with time series, is that they all
 covers the common time period long enought to keep a lot of data to work
 on.
Let's have a view on the time series on every input file.
Once we would have identified the input data files that I can keep or no,
 I will merge them by the columns 'date' and 'dep'.


============================================================================

METHODOLOGY


Data Preprocessing:

- Data merging

- Description of data (after merging)

- Data cleaning

- Data complementation

- Implementation

- Modeling


   
============================================================================

FINDINGS


Among complication met during this analysis, I would report:

-	Some data were not correctly defined;

-	All data sets do no provide updated values at the same frequency such
    it make difficult the merge and the analysis of these data.
-	The difficulties to find a relevant type of model for this kind of
    complex phenomenon.
-	The difficulties to find a relevant metrics since it requires a long
    period of test before knowing the consistency of such model and such
	metrics with this model for this type of dataset.
 

============================================================================
 
RESULT

- Visualization

- Model evaluation and validation
 

============================================================================

CONCLUSION

- Reflection

- Improvement

 
============================================================================

VERSION:

ID: 1.3.0

In comparison with previous version, this new version brings following
 change:

 - Delivery of a new Blog Post
 
 - Delivery of a new Notebook


============================================================================

INSTRUCTIONS:

- Create local folder as workspace for this programme;
- load and unzip csv data sheet files into this workspace
- Load the Notebook script  file into this workspace;
- Install the required librairies: pip install -r requirements.txt;
- When needed, open the notebook "COVID19_France_workunit.ipynb" in a python
  code editor.
			
============================================================================

PUBLIC RELEASE: UPDATE!

You can find the published results here:
https://medium.com/@laurent.jp.costa/data-scientist-project-related-to-the-analysis-of-hospitalization-data-in-france-due-to-covid-19-17c3df18f5cb


============================================================================

ENVIRONMENT:

Refer to the file requirements.txt


============================================================================

REPOSITORY’S FILES:

File “README.md”
File "requirements.txt" - librairies required for the proper execution of 
 the programme.
File “COVID-19_France_data_epidemic_indicators.csv” – data sheet file under csv format providing
 hospital data related to COVID 19 in France.
 
File "éCOVID-19_France_data_vaccin_indicators.csv"

File "COVID-19_France_data_vaccin_indicators_tot.csv"

File "COVID-19_France_data_vaccin_pathology.csv"

File "COVID-19_France_data_vaccin_population.csv"

File "COVID19_France_workunit.ipynb" is the analysis notebook.



============================================================================

DATA SOURCE:

Hospital data: 

- Name: Santé publique France
- Licence: Open licence version 2.0 / ID 60190d00a7273a8100dd4d38 /
  (https://www.etalab.gouv.fr/licence-ouverte-open-licence/)
- Link: https://www.data.gouv.fr/fr/datasets/synthese-des-indicateurs-de-suivi-de-lepidemie-covid-19/
- Update: 19-Dec-2022
- Data extraction date: 20-Dec-2022
- Request for reuse: Indicate the following link in my presentation of
  results:
  https://www.data.gouv.fr/fr/datasets/synthese-des-indicateurs-de-suivi-de-lepidemie-covid-19/


============================================================================

LEGAL:

Reuse and exploitation of source data: Open licence (refer to DATA SOURCE).