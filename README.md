# NHSBSA Quarto Website Template

This repository contains the framework for writing and deploying the NHSBSA Quarto Website Template.

The Quarto Website Template is used to provide a starting point for Quarto websites built by the NHSBSA.

The live version of the Quarto Website Template can be found [here](https://nhsbsa-data-analytics.github.io/quarto-website-template/).

## Getting started

The Quarto Website Template is created using [Quarto](https://quarto.org/docs/get-started/).

You can run the document by:

1. Opening the repository in Rstudio or VS Code
    - For Rstudio usage, you simply require the latest version of Rstudio. You must open it via the R project file, `quarto-website-template.Rproj`. 
    - For VS Code, you must install the Quarto extension and install the Quarto CLI. When running Quarto for the first time, you will be prompted with instructions on how to install this. **Please note this is not currently possible with the Azure Virtual Desktop (AVD)**.
1. Opening [index.qmd](/index.qmd) in the repository root
1. Click 'Compile' or 'Preview' respectively.

## Folder Structure

The playbook is structured into a series of sections and pages. A section can be navigated to via the navbar dropdown. Alternatively, the sidebar can be used to navigate directly to any section or page. The navbar and sidebar are always available. The landing page and each section page also has a listing allowing navigation to sections, or pages within a section, respectively.

Each section and sub-section is populated by a `.qmd` file and supporting `.jpg` file to provide the image for each page listing. The sections and pages should be numbered according to their desired order in the navigation elements.

The following folder structure highlights how this is setup up from a coding perspective.

```
├───sections ............................# Folder containing all of the playbook content separated into sections
|   ├───_metadata.yml ...................# Additional settings applied to all pages
|   ├───01-section ......................# First section folder, containing content separated into pages
|       ├───index.qmd ...................# Section 'top-level' page 
|       ├───pages .......................# Folder containing all content for first section
|           ├───01-page .................# First page of first section
|           ├───01-image.jpg ............# Image for listing of first page of first section
|           ├───02-page .................# Second page of first section
|           ├───02-image.jpg ............# Image for listing of second page of first section
|           ├───etc.
|   ├───02-section ......................# Second section folder, containing content separated into pages
|   ├───etc.
```

The full folder structure is detailed below.

```
Quarto Website Template
|───_extensions .........................# Folder automatically created when first adding a quarto extension
├───_quarto.yml .........................# File that controls most of the page layout and settings for the quarto website
├───.github .............................# Folder for GitHub related code such as templates and workflows
├───.gitattributes ......................# Sets end-of-line conversion to auto (CRLF vs LF)
├───.gitignore ..........................# Ignore certain files, including quarto folders that are created locally when running website
├───about.qmd ...........................# An additional .qmd that populates the 'About' page
├───accessibility.qmd ...................# An additional .qmd that populates the 'Accessibility' page
├───CONTRIBUTE.md .......................# Guidance on contributing to the repo
├───index.qmd ...........................# The primary .qmd file, used as landing page and to compile the website
├───post-load-accessibility-fixes.html ..# HTML containing a JavaScript script that performs multiple accessibility fixes
├───quarto-website-template.Rproj .......# The R project file
├───README.md ...........................# This README file
├───sections ............................# See detailed folder structure above
├───skip-link.html ......................# HTML containing a JavaScript script that adds an accessibility feature
├───static ..............................# A folder containing the static assets of the website
├───styles.css ..........................# A file containing additional styling for the website
```

## Using this repo as a template

TODO: Add guide

## Contributing to Quarto Website Template

We welcome contributions from community members. Please see our [contributing guide](./CONTRIBUTE.md) for information on how you can get involved!
