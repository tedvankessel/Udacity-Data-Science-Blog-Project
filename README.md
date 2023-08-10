# Udacity-Data-Science-Blog-Project
## <p>Project: Write a Data Science Blog Post 
## Blog post locations:
>#### Github Pages Blog Repo:  https://github.com/tedvankessel/se4sci-blog
>#### Github Pages Blog Post: https://tedvankessel.github.io/se4sci-blog/2023/08/09/Methane_the_Other_Greenhouse_Gas.html

## Introduction 

Methane is the second largest greenhouse gas contributer (25%) to global warming behind carbon dioxide.
Oil and gas operations are a significant component of the total world methane emissions accounting for 29% 
of all emissions. These are predominantly from leakage from equipment (faulty or under normal use) and flaring. 

In this project I procured a public dataset taken from a NASA JPL aerial survey performed in 2019 to measure methane plumes,
assigne it to a source and compute the emission rate. Approximately 3000 plumes were observed and entered in the dataset.

I felt this project was an opportunity to explore some important questions relative to this data

## Code

The code for this project is fully embodied in the **permean_methane_rev_1.ipynb** Jupyter Notebook file
in this Github repository.

## Datasets

The dataset used for this project is from the NASA/JPL 2019 Methane survey performed with the AVIRIS team.
The Survey was done in West Texas in the permean basin and looked for methane plumes with infrared cameras.
Analysis of the raw data was done by the JPL team to identify source emission location and where possible equipment
types.
This data is public and available from numerous sources. 
It is available from NASA, but it is difficult to find. For this work I accessed it from the ACS
(see reference 2) at the following web addresses (also see reference 3 & 4):
	https://pubs.acs.org/doi/suppl/10.1021/acs.estlett.1c00173/suppl_file/ez1c00173_si_001.xlsx
	https://pubs.acs.org/doi/suppl/10.1021/acs.estlett.1c00173/suppl_file/ez1c00173_si_002.xlsx
 These are in Excel format which I converted to .csv format using Excel and saved in the Github.

 
## Acknowledgments and Sources of Code and Data:

	Udacity project documents 
	README-Template - https://gist.github.com/PurpleBooth/109311bb0361f32d87a2
	ChatGPT
	Udacity GPT
	Google
>### References: 
  1. Methane: A crucial opportunity in the climate fight https://www.edf.org/climate/methane-crucial-opportunity-climate-fight
  2. Cusworth, D.H., Duren, R.M., Thorpe, A.K., Olson-Duvall, W., Heckler, J.W., Chapman, J.W., Eastwood, M.L., Helmlinger, M., Green, R.O., Asner, G.P., Dennison, P.E., & Miller, C.E. (2021). Intermittency of Large Methane Emitters in the Permian Basin. Environmental Science and Technology Letters.
  3. https://pubs.acs.org/doi/suppl/10.1021/acs.estlett.1c00173/suppl_file/ez1c00173_si_001.xlsx
  4. https://pubs.acs.org/doi/suppl/10.1021/acs.estlett.1c00173/suppl_file/ez1c00173_si_002.xlsx
  5. Methodology for EDF’s Permian Methane Analysis Project (PermianMAP) https://www.edf.org/sites/default/files/documents/PermianMapMethodology_1.pdf
  6. Thorpe, A. K., et al., Mapping methane concentrations from a controlled release experiment using the next generation airborne visible/infrared imaging spectrometer (AVIRIS-NG) , Remote Sensing of Environment, 104-115, 2016, https://doi.org/10.1016/j.rse.2016.03.032




## Rubric elements

### Rubric item: Code Functionality and Readability
	Code is readable (uses good coding practices - PEP8)
	Code is functional.
	Write code that is well documented and uses functions and classes as necessary.

I have run Pylint via nbqa with the following result: 

	(SE4Sci) C:\JupyterNotebooks-SE4Sci>nbqa pylint permean_methane_rev_1_0.ipynb
	************* Module permean_methane_rev_1_0
	permean_methane_rev_1_0.ipynb:cell_2:5:0: E0401: Unable to import 'seaborn' (import-error)
	
	-----------------------------------
	Your code has been rated at 9.71/10

Note that the Seaborn module loads fine in Jupyter.
The code is fully functional and heavily commented
 
### Rubric item: Data
	There are 3-5 business questions asked and answered.

Business Questions:
1. Does the 80/20 rule apply to methane emissions?
2. Do methane emissions vary significantly by type of equipment?
3. What fraction of methane emissions occur in the presence of flaring?

These three questions were addressed in the code and the blog post. 
In summary:
> Answer to question 1: the largest 44% of emissions in this data account for 80% of the total emissions.

> Answer to question 2: emissions do not vary significantly by type of equipment in this dataset.

> Answer to question 3: 
>> 1. the vast majority of observed plumes occur in the absence of any observed flares
	(active or inactive).
>> 2. the number of plumes present when active flaring is observed is non-trivial.
>> 3. active flaring accounts for about 5% of the observed emissions in this dataset.
### Rubric item: Github Repository
	Student must publish their code in a public Github repository.
 All project materials have been published in this Github repository including:
> code

> datasets

> blog documents

### Rubric item: Blog Post
	Communicate their findings with stakeholders.
	There should be an intriguing title and image related to the project.
	The body of the post has paragraphs that are broken up by appropriate white space and images.
	Clearly state the business questions and the corresponding solutions
This has been done.
>#### Github Pages Blog Repo:  https://github.com/tedvankessel/se4sci-blog
>#### Github Pages Blog Post: https://tedvankessel.github.io/se4sci-blog/2023/08/09/Methane_the_Other_Greenhouse_Gas.html

### Installing
The jupyter notebook file can be operated with the standard Jupyter Notebook software.
As in all projects, it is recommended to set up an environment with the required packages. These include:

 	pandas 2.0.1
	numpy 1.24.3
	matplotlib 3.7.1
	seaborn 0.10.0
 
 ### NOTE: a requirements.txt file can be found in this Github that contains all the packages used in this project
 
A single notebook was used for this project: 
	Permean Methane Rev 1.ipynb
 
This notebook requires that 2 data files be present in the same directory as the notebook.
These files are:
	Georeferenced plume list ez1c00173_si_001.csv
	Georeferenced source list ez1c00173_si_002_clean_v1.csv
 
## License
This project is licensed under the MIT License  License - see the LICENSE.md file for details

## Built With
	Anaconda
	Eclipse IDE for Developers (used for checking code)
	Jupyter Notebook
## Author
**Theodore van Kessel** 
 


