# shinyGEO
shinyGEO is a web-based tool that allows a user to download the expression and sample data from a [Gene Expression Omnibus](http://www.ncbi.nlm.nih.gov/geo/browse/) dataset, select a gene of interest, and perform a survival or differential expression analysis using the available data. For both analyses, shinyGEO produces publication-ready graphics and generates R code ensuring that all analyses are reproducible. The tool is developed using shiny, a web application framework for R, a language for statistical computing and graphics.

## Official Website
http://gdancik.github.io/shinyGEO/

## The preferred way of running *shinyGEO* locally is through docker:

1. Download docker from https://www.docker.com/get-started

2. Pull the docker image by running the following from your terminal: 		

    `docker pull gdancik/shinygeo`


3. Run *shinyGEO* by using the command: 

    `docker run -it --rm -p 3838:3838 gdancik/shinygeo`

4. View *shinyGEO* by opening a web browser and entering *localhost:3838* into the address bar.

5. **New**. ShinyGEO datasets can now be updated directly from the web application. Click the Update button to update the datasets (updating data sets once a month is recommended). Then open another terminal or command prompt, as was done for step 3, and enter the following command to save your changes. This updates the gdancik/shinygeo image with the updated datasets:

    `docker commit $(docker ps -alq) gdancik/shinygeo`

## Contributors
- Main contributors: Jasmine Dumas, Michael Gargano, Garrett M. Dancik, PhD
- Additional contributors: Nataliia Romanenko, Ken-Heng Liao, Gregory Harper, Brandon Spratt

## Acknowledgements
This work was supported, in part, by Google Summer of Code funding to JD in 2015. MG, KHL, GH, and BS contributed as part of an independent study in Computer Science / Bioinformatics while undergraduate students at Eastern Connecticut State University, Willimantic, CT,  USA.

