# Database of chemical functions for the CadQuery organic molecule modeling program

## Project Abstraction

CadQuery is an organic molecule modeling program that works as a Python script interpreter. The script describes the mathematical formula for the 3-dimensional model of what could be an organic compound. The User Agent actor types in a script to represent an organic molecule, and CadQuery will model it accordingly. The script can be parameterized to make it polymorphic. Then a third party can fill in the details of the parameters. We can store these formulas and create a database of organic compounds, and this parameterization will make it easier to store related families of molecules. Additionally, we may extend this format to include chemical properties of these organic compounds.

## Project Relevance

Test driven development may be performed by sending an existing molecule model to the database and testing if it matches the expected molecule in function. If the description of the function matches what we expect then it works fine. If not, the function returned may offer a hint to what exactly is wrong.

## Conceptual Design

The design is object oriented, which makes composition and dependency injection possible. Using composition, we can add in a database of organic molecules. The database contains organic molecules and their uses. If the molecule entered by the user resembles existing molecules, then the new contribution will attempt to guess at the function of the new molecule and suggest it to the User Agent actor. If the guess is wrong, it offers the User Agent actor an opportunity to describe the function of the new molecule both to describe it and to provide a possible new description to future similar molecules. Dependency injection offers an opportunity to extend the composition model in the future for other projects to build upon this one.

## Background

https://github.com/CadQuery/cadquery/blob/master/README.md

### Building (from the cadquery README)

```
# Set up a new environment
conda create -n cadquery

# Activate the new environment
conda activate cadquery

# CadQuery development is moving quickly, so it is best to install the latest version from GitHub master
conda install -c conda-forge -c cadquery cadquery=master
```

### Running

## Required Resources
* Group competencies
    * Knowledge of programming in Python
    * Object oriented programming concepts
    * Organic chemistry
* Hardware and software resources
    * Hardware
        * A personal computer (a desktop or laptop will do)
    * Software
        * Linux
        * VirtualBox
        * Python
        * Anaconda
