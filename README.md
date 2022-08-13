# esa2021

ESA 2021 workshop: community analysis of species, traits, phylogenies, and responses to environment

We will use a dedicated **R** package that contains tutorial material.  Install and test as follows.

### Installation

1.  Download and install **R** from: https://cran.r-project.org/  
2.  Download and install **Rstudio** from: https://www.rstudio.com/products/rstudio/download/#download  
3.  Download our **esa2021** package from:  https://github.com/phytomosaic/taresa2021/raw/main/esa2021_0.0.1-20210722.tar.gz and save somewhere you will remember.  
4.  Open the **Rstudio** console, then run:  

```
### install dependencies
pkg <- c('vegan','labdsv','ade4','ecodist','fso',
         'vegclust','ape','picante','mgcv','learnr')
has <- pkg %in% rownames(installed.packages())
if(any(!has)) install.packages(pkg[!has])

### specify path to wherever you saved the file (change as needed)
path_to_file <- '~/Downloads/esa2021_0.0.1-20210722.tar.gz'

### install the main package
install.packages(path_to_file, repos=NULL, type='source')
```
5. Go to **Usage** below.  

### Usage

To run the tutorial, simply run this in the **R** console:  

```
require('esa2021')
learnr::run_tutorial('esa_tutorial', package='esa2021')
```

This creates a local instance of the interactive tutorial, which can open in a web browser.  The tutorial is a combination of text describing ecological concepts, along with embedded code chunks that let you run live **R** commands.  

### Pre-survey

Don't forget to fill out the survey _before_ the course!  This lets us know which topics you'd like to focus on.  Find it at: https://www.surveymonkey.com/r/K9C9QKP  

### Contributors

**Organizer**: Kyle Palmquist  
**Co-organizers**: Martin Dovciak, Samuel Jordan, Lisa Kluesner, Rob Smith (robert.smith3@usda.gov)  
