# TOPSIS implementation in python for multi-criteria decision making

## To use via command line
`python3 run.py data.csv 25,25,25,25 -+++`

First argument after run.py is filename with .csv extension. The .csv file is assumed to have a structure similar to one provided in topsis_navkiran/data.csv

That is, the .csv file should have a header with column names and first column should only list alternatives and not attribute values.

## To use in .py script
```from topsis_navkiran import topsis
"""
decision_matrix is 2D numpy array, weights is a 1D array and impacts is a string of the form +-+-- 
where + indicates benefit and - indicates cost
"""
output_dataframe = topsis(decision_matrix,weights,impacts)
```
Based off on a similar package for TOPSIS in R
