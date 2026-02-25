# MSE465_final_project
### Group Member
1. Cheng-yuan Chen
2. Yu Chen Hsu
3. Hung Chin Lee

# Physically Interpretable Strain Mapping in 2D Heterojunctions Using 4D-STEM

## Dataset Information
### Dataset Source:
1. Nanobeam 4D-STEM raw data of monolayer $WS_2-WSe_2$ lateral heterojunctions
https://zenodo.org/records/10892106 
2. Experimental and Simulated Datasets Used in "Strain Mapping of Three-dimensionally Structured 
Two-dimensional Materials"
https://zenodo.org/records/17246822   

### Dataset Size & Format:
1. Recorded at 27.5 $kx$ magnification with a 1.2 mrad convergence angle. The data includes diffraction 
patterns of monolayer $WS_2-WSe_2$ lateral heterojunctions with in-plane epitaxial interfaces.
2. 256 times 256 scan grid with 128 times 128 pixel diffraction patterns (.raw format) 

## Division of Labor
### Person 1: Diffraction Feature Extraction
1. Probe Center Calibration
2. Background Subtraction
3. Bragg Peak Detection
### Person 2: Strain Calculation
1. Define Reference Lattice
2. Calculate $\epsilon_{xx}, \epsilon_{yy}$
3. Noise Filtering
### Person 3: Physical Consistency & Interpretation
1. Check Strain Magnitude Follow Physics Law
2. Analysize Strain Gradient Near Heterointerface
3. Build Final Visualization Diagram


