# Spectroscopic Data Analyzer
**By:** Andrew Xu

**Mentor:** Eshan Dahal with Assistance from Aldo Badano

## Purpose

This repository contains Open-Source Data Analysis Software using Python libraries (`Tkinter`, `NumPy`, and `Matplotlib`) to conduct Spectroscopic Photon Counting Analysis with a built-in UI. It transfers Hexitech files into graphable data to detect radiation. I did this project during my time as an ORISE intern at FDA.

# Structure and Input/Output

There are three Python files: function, main, and hxtV3Read. Here is what you'll find in each:
1. `main.py`: User interface components
2. `function.py`: data analysis and plotting
4. `hxtV3Read.py`: contains the Hexitech file reading code.
To run the program, the user must run 'main.py'.

## Input

Once the program is run, it will prompt the user to browse two Hexitech files for analysis and 4 inputs:
1. **Bin Start**: The bin layer of the program will begin analysis on
2. **Bin End**: The bin layer of the program will end analysis on
3. **Bin Width**: The bin layer interval the program will analyze, from bin start to bin end.
4. **Energy Window**: The bin layer interval the program will analyze and put onto 3d graphs.

## Output

6 graphs will be produced from the inputs:
| Figure # | Description |
|:-------------:|:-------------:|
| 1 | Color mesh of the counts for each pixel of each Energy window interval created |
| 2 | Color mesh of the counts for each pixel of the overall interval (bin start to bin end) |
| 3 | Color mesh of the processed data |
| 4 | 3D Graph of the combined counts of every possible interval created through the energy window |
| 5 | Line Graph of the difference in counts for each pixel between the sample and the background data |
| 6 | Line Graph of the counts for both the sample and background data |

## Sample Input and Output

- **Background Hexitech File:** "2020_aug31_1mA_300s_syringe_empty.hxt"
- **Sample Hexitech File:** "2020_aug31_1mA_300s_caffeine.hxt"
- **Bin Start:** 30
- **Bin End:** 45
- **Bin Width:** 1
- **Energy Window:** 5

  
| # | Figure | # | Figure | # | Figure |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| 1  |: <img src="Figures/Figure_1.png" alt="1" style="width:250px;"/>  :| 2  | <img src="Figures/Figure_2.png" alt="2" style="width:250px;"/>  | 3  | <img src="Figures/Figure_3.png" alt="3" style="width:300px;"/>  |
| 4  | <img src="Figures/Figure_4.png" alt="4" style="width:300px;"/>  | 5  | <img src="Figures/Figure_5.png" alt="5" style="width:300px;"/>  | 6  | <img src="Figures/Figure_6.png" alt="6" style="width:300px;"/>  |
