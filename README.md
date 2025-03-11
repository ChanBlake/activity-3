# Activity 3: Creating Metadata in Dataspice
Overview
This project is part of Activity 3 for metadata creation using `dataspice` in RStudio. The goal is to structure metadata files for a selected dataset, generate a JSON-LD metadata file, and publish the final results to GitHub.

Steps Completed

1. Set Up the Project
- Initialized an RStudio project named **dataspice.qmd**.
- Installed and loaded required R packages:  
install.packages(c("jsonlite", "listviewer", "here", "magrittr", "pkgdown"))
library(jsonlite)
library(listviewer)
library(here)
library(magrittr)
library(pkgdown)

2. Populated Metadata Files
Used interactive editors to fill out the following metadata files:
access.csv (file access information)
attributes.csv (variable details)
biblio.csv (dataset citation and description)
creators.csv (author and contributor details)

3. Created and Compiled JSON-LD Metadata
Compiled all metadata into a structured JSON-LD file:
write_spice()

4. Generated and Published the Quarto (.qmd) File
Created a Quarto file (metadata.qmd) documenting the dataset and metadata process.
Rendered the .qmd file to an HTML format using:
quarto::quarto_render("metadata.qmd")

6. Committed and Pushed to GitHub
Initialized a Git repository, added files, and pushed to GitHub:
system("git init")
system("git add .")
system('git commit -m "Initial commit with dataspace metadata files"')
system("git push origin main")
