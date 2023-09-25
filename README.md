============================================================================

PROJET/PURPOSE:

UDACITY - DATA SCIENTIST CAPSTONE project


============================================================================

TITLE:

IMPROVING THE ALLOCATION OF HOSPITALZATION RESOURCES IN HAUTE-GARONNE
 DURING THE COVID-19 PANDEMIC THROUGH PREDICTIVE MODELS.


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

Purpose of the project consists in predicting the quantity of means for
 hospitalization and intensive care such that the appropriate means could
 be affected to a geographical area.
It shall be realized sufficiently in advance for logictics concerns and
 with a high level of accuracy for helping bring the appropiate quantity
 of health care means.
By order, I will focus my attention on my department, Haute-Garonne, my
 region Occitanie and the France.


Answering strategy:

For addressing this purpose, I need building an accurate predictive model
 of the number of hospitalization and resuscitation cases per various
 geograpical areas.
For that, I need a large amount of data related to COVID-19 pandemy from
 french hospitals.
Actually, I would present my strategy as follows:

- Explore input data

- Develop a methodology

- Implement my solution

- Present my results

- Conclude


Define my metrics:

My first metrics is based on the predictive model scoring; I will target
 a score equal or higher than 0.9 on a scale from 0 (null) to 1 (perfect)
My second metrics is related to my first target (number of hospitalized
 patient) ... I assume the predictive absolute error shall to exceed 1/5
 of this capacity, i.e. 23 hospitalized people (never exceeding 118).
In amount of department, we goes from 23 for the department 31 to 299
 for the Region Occitanie (76) and 2300 for France.
My third metrics is related to my second target (number of hospitalized
 patient) ... I assume the predictive absolute error shall to exceed 1/5
 of this capacity, i.e. 29 people hospitalized in intensive care (never
 exceeding 145). In amount of department, we goes from 29 for the
 department 31 to 377 for the Region Occitanie (76) and 2900 for France.


============================================================================

DATA EXPLORATION


I will gather data related to COVID-19 patients from all french
 institutional health sites related from all departments of France. Then I
 will explore and describe these data for identifying potential troubles
 for processing them.


WORKSPACE
Calculations, plots and analysis of this project were realized through a
 python Notebook. I coded in Python 3 with basic libraries to get data from
 my files, to handle and plot these data (numpy, pandas, plotly, matplotly
 and seaborn) and with sklearn for modeling then train and evaluate my
 model. I chose sklearn to benefit from the free and the large amount of
 possible models and related metrics solutions.

This Notebook and all related files are available in a dedicated Github
 repository. Before running the code:
 
- Refer to the README file;

- Refer to the Requirements file for knowing the required environment;

- Download the whole content of the dedicated Github repository on your
   workspace and update the variable ‘work_dir’ accordingly.


DESCRIPTIONS OF INPUT DATA SETS
The 29 December 2022, I downloaded data files related to the COVID-19
 epidemic in France reported directly by the hospitals and gathered on the
 french institutional website https://www.data.gouv.fr/fr/datasets
The source web site indicates that data have been gathered along the time
 from various formats and contents. All the files used are under the License
 "Open Data Commons Open Database License (ODbL)".


============================================================================

DATA VIZUALIZATION

I will plot some data for continuing the exploration and finding additional
 clues for further preprocessing and modeling:
 
 - Time-series (all files)
 
 - Data availability and overlapping (Files #3 & #4)
 
 - Distribution of data per region & department  (Files #3 & #4)


============================================================================

METHODOLOGY

It consists in preparing and selecting the most appropriate data sets
 for modeling with accuracy with respect to my targets.


Data preprocessing:

It consists here in all required data preprocessing operations for
 selecting data files, merging and cleaning my data and provide them in
 a understandable way:
 
 - data merging;
 
 - removing missing values;
 
 - adjust the data set to kept data under format that can be used for
    further modeling activities;
	
 - Data set's labels renaming for consistency between data files;
 
 - Convert time series in a consistent format for modeling;
 
 - label description by providing if necessary a literal description of
   labels for further presentation concerns.


Data understanding:

It consists in deepening my understanding of the data sets to identify
 relevant data to properly feed my model with respect to my targets:
 
 - a full description of the input parameters;
 
 - a view of the distribution of the targets per geographical area;
 
 - a view on the correlation between targets;
 
 - a view on the correlation between input parameters and targets;
 
 - make assumptions to reduce the number of input parameters.


Data extraction:

It consists in removing useless input parameters identified during the data
 understanding step and keeping only appropriate data for modeling.
Note: This selection will be done in two steps; first here, second during
      the Refinement phase.

============================================================================

IMPLEMENTATION

This step will consists in building a model according to my targets:

- Multiple targets problem: discuss the purpose to run after two
   targets;
   
- Model selection: I will identify the most appropriate modeling method;

- Model metrics selection: I will identify the most appropriate scoring
   method in accordance with the model selection;
   
- Refinement: I may have to adjust the data sets;

- Hyperparameter tuning: I will set the model for improving its result;

- Vizualization: I will illustrate result of the model implementation.


============================================================================
 
RESULTS

Presentation of my results will consists in:

- Model evluation and validation;

- Justification, including comparison tables and explanations.


============================================================================

CONCLUSION

- Reflection: Summarize the end-to-end problem solution and discuss what
   was interesting/difficult in the solution implementation;
   
- Improvement: Open items that could by studied to improvement the result.

 
============================================================================

VERSION:

ID: 1.4.0

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