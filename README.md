# -econ5560-replication-white
Repository for Project 1 in Econ 5560


### Data/paper information
This paper replicates a study published in 2026 titled, "Understanding landowner preferences for traditional and nature-based solutions incentive programs in North Carolina, USA" written by Courtney B Deviney, Rajan Parajuli, Frederick Cubbage, Erin Sills, 
and Robert Bardon. The paper can be found here - https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0347042#sec009. A PDF of the data can be found in the 'Supporting Information' section of the link. To get the data needed for analysis, use the data found in the Github repo, as this data 
was obtained after communication with the authors and is in .xls format rather than PDF format. 


### How to use code/data from the repo
## run_all.R
All of the code to generate the output and run the entire FIML model is located inside the file run_all.R. It automatically creates the logs folder and the output folder in the same directory. 
## outputs 
This file contains the tables and output generated from our code intended to replicate the results in the paper
## logs
This file contains a text file of output associated with running run_all.R
## decoded_data.xls
This is the data actually used in the code contained in run_all.R, and importantly when downloading keep it in the same working directory as wherever run_all.R is upon downloading. 


## Software and Package Requirements
The replication was performed using **R version 4.5.0** on **Windows 11 x64 (build 26200)**. The script requires the following R packages:

| Package | Version |
|---|---|
| readxl | 1.5.0 |
| dplyr | 1.1.4 |
| tidyr | 1.3.1 |
| tibble | 3.2.1 |
| knitr | 1.50 |
| kableExtra | 1.4.1 |
| mvtnorm | 1.4-2 |
| ggplot2 | 3.5.2 |
| sandwich | 3.1-3 |
| lmtest | 0.9-40 |

Additional packages loaded during execution include:

| Package | Version |
|---|---|
| tidyverse | 2.0.0 |
| haven | 2.5.5 |
| readr | 2.1.5 |
| purrr | 1.0.4 |
| stringr | 1.5.1 |
| forcats | 1.0.0 |
| lubridate | 1.9.5 |
| zoo | 1.8-14 |

The master script (`run_all.R`) automatically checks for missing required packages and installs them from CRAN before executing the analysis. RStudio is optional, as the script can also be executed directly using `Rscript`.

The complete software environment, including additional package dependencies, is documented in the `sessionInfo()` output at the end of the pipeline log.


## Run length
A full run of run_all.R takes 3-5 minutes to run, primarily due to the model building segment. 


### What we couldn't reproduce
From the paper we couldn't exactly reproduce the FIML model output primarily due to uncertainty regarding how the authors dealt with missing data in the model-building process. 



























