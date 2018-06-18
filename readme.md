# Nanostring analysis

Analysis of three Nanostring datasets from:
Oct 2016
Feb 2017
Nov 2017

Goals:
-Optimise marker set for age discrimination
-Optimise normalisation methods
-Determine the effect of regeneration on molecular age
-Develop method to categorise samples by quality

### Prerequisites

All analysis was performed in RStudio Version 1.0.136, running R version 3.x. 
Packages needed are:

ggplot2
rmarkdown
gplots
RColorBrewer
reshape2
scales
ggbiplot
devtools
NanoStringNorm
gtools
knitr
dplyr
tidyr
e1071
caTools
FinCal

Exact prerequisites depend on script in question. 


### Structure
The following functions are carried out by the following scripts:
All analyses are carried out in notebooks (Rmarkdown format), with visualisation & graphics within

import.r: import and normalisation of raw data (produces .rdata files which other scripts depend on)
markeropt.rmd: optimise marker set
agesepmodelling.rmd: machine learning approaches to classify samples as young or old
qual.rmd: examine sample quality
normal.rmd: compare normalisation methods
rejuvnhyper.rmd: examine effect of regen on markers
labmeeting18-2-7: produces .pdf report
nstringnov17main.rmd: initial analyses

.html files (produced via knitr) corresponding to the .rmd files are available (reports)


All raw data is held in folders with .rcc files (not in repo)


## Samples

Nov 2017:
59 samples in total, including: 
Old and young male and female pools
Old male and female individuals
Females at 0, 10 and 20 days after moulting, pools and individuals
Regeneration experiment sets: each pool individual has three samples taken:
Left T4 & T5 limbs at t0 (bef)
Left T4 & T5 limbs at t30, after regeneration (reg)
Right T4 &T5 limbs at t30 (un)

Feb 2017:
24 samples in total

Oct 2016:
24 samples in total

## Repository

[https://github.com/luke-hayden/nstringn17]

## Authors

* **Luke Hayden** 

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Marie Semon & Michalis Averof for advice
* Paola Oliveri


