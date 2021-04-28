# pyboiledegg
Python 3 program to predict absorption/distribution characteristics of molecules in the human body through likelyhood of gastrointenstinal absorption and ability to cross the blood-brain-barrier.

The program implements the Brain Or IntestinaL EstimateD absorption (BOILED-egg) method of Daina and Zoete [1] and calculates the topological polar surface area and WlogP for molecules provided in (multi-structure) SDF format. If the TPSA and WlogP values fall within eliptical regions of a scatter plot corresponding to the boundaries of the regression model derived in [1] the corresponding molecule is predicted to display suitable properties for gastrointestinal absorption and also potentially for brain access.

The program has been used with Python >= 3.6 in Linux/MacOS X environments but should work in lower Python 3.x versions (with some small modification for Python 2.x). Changes required to enable running in Windows should also be minimal. Dependencies include RDKit (calculation of descriptors) along with Pandas (data handling) and Matplotlib and Shapely for plotting.

Output is created in spreadsheet format (CSV by default) and as a BOILED-egg scatter plot (PDF format).

[1] Daina, A. & Zoete, V. A BOILED-Egg To Predict Gastrointestinal Absorption and Brain Penetration of Small Molecules. ChemMedChem 11, 1117–1121 (2016).
