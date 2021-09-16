Leomar Durán
Fall 2021
CIS 3296, Section 003
Project proposal
2021-09-16

# Title

Function Database for CadQuery

# Project Description
https://github.com/CadQuery/cadquery/blob/master/README.md

CadQuery is an organic molecule modeling program that works as a script interpreter. The UA actor types in a script to represent an organic molecule, and CadQuery will model it accordingly. The script can be parameterized to make it a bit more polymorphic. Then a third party can fill in the details of the parameters.

# Technical Contribution

Using composition, we can add in a database of organic molecules. The database contains organic molecules and their uses. If the molecule entered by the user resembles existing molecules, then the new contribution will attempt to guess at the function of the new molecule and suggest it to the UA actor. If the guess is wrong, it offers the UA actor an opportunity to describe the function of the new molecule both to describe it and to provide a possible new description to future similar molecules.

Test driven development may be performed by sending an existing molecule model to the database and testing if it matches the expected molecule in function. If the description of the function matches what we expect then it works fine. If not, the function returned may offer a hint to work’s wrong.
