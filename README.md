# FDA ORISE Intern Code
By: Andrew Xu, Eshan Dahal, Aldo Badano

**Purpose**

This repository contains Open-Source Data Analysis Software I wrote in Python and MATLAB to conduct Spectroscopic Photon Counting. It transfers Hexitech files into graphable data to detect radiation.

# Structure and Input/Output

There are three python files: function, main, and hxtV3Read. "function.py" contains all the data analysis and plotting, "main.py" contains the user interface components, and "hxtV3Read.py" contains the hexitech file reading code. To run the program, the user must run 'main.py'.

**Input**

Once the program is run, it will prompt the user to browse two hexitech files for analysis and 4 inputs:
1. Bin Start: The bin layer the program will begin analysis on
2. Bin End: The bin layer the program will end analysis on
3. Bin Width: The bin layer interval the program will do analysis on, which is bin start to bin end.
4. Energy Window: The bin layer interval the program will do analysis and put onto 3d graphs.

**Output**

6 graphs will be produced from the inputs:
- Graph #1: A color mesh of the counts for each pixel of each Energy window interval created
- Graph #2: A color mesh of the counts for each pixel of the overall interval (bin start to bin end)
- Graph #3: A reference graph for graph #2
- Graph #4: 3D Graph of the combined counts of every possible interval created through energy window
- Graph #5: The difference in counts for each pixel between the sample and the background data
- Graph #6: The counts for both the sample and background data (2 lines).

**Sample Input and Output**

- Background Hexitech File: "2020_aug31_1mA_300s_syringe_empty.hxt"
- Sample Hexitech File: "2020_aug31_1mA_300s_caffeine.hxt"
- Bin Start: 30
- Bin End: 45
- Bin Width: 1
- Energy Window: 5

The Outputted Graphs are in the "Figures" folder. Here is an example of all the figures that are printed:

| # | Figure | # | Figure | # | Figure |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| 1  |: <img src="Figures/Figure_1.png" alt="1" style="width:250px;"/>  :| 2  | <img src="Figures/Figure_2.png" alt="2" style="width:250px;"/>  | 3  | <img src="Figures/Figure_3.png" alt="3" style="width:300px;"/>  |
| 4  | <img src="Figures/Figure_4.png" alt="4" style="width:300px;"/>  | 5  | <img src="Figures/Figure_5.png" alt="5" style="width:300px;"/>  | 6  | <img src="Figures/Figure_6.png" alt="6" style="width:300px;"/>  |

