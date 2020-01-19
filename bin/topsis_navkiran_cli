#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Sun Jan 19 12:36:27 2020

@author: navkiran
"""
import pandas as pd
import sys
from topsis_navkiran import topsis

arguments = sys.argv[1:]
assert len(arguments) == 3, "Insufficient number of arguments provided, 3 required -> filename with extension, weights separated by comma and impact string"

filename = sys.argv[1]
assert filename, "Filename must be provided"
assert '.csv' in filename, "File extension must be .csv"
    
data = pd.read_csv(filename,header=0,index_col=0)
weights = sys.argv[2].split(',')
impacts = sys.argv[3]
assert len(impacts) == len(weights), "Mismatch between length of impacts and weights"

print(topsis(data,weights,impacts))
