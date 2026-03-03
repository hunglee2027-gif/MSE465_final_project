# MSE465_final_project
### Group Member
1. Cheng-yuan Chen
2. Yu Chen Hsu
3. Hung Chin Lee

# Physically Interpretable Strain Mapping in 2D Heterojunctions Using 4D-STEM

## Dataset Information
### Dataset Source:
1. Experimental and Simulated Datasets Used in "Strain Mapping of Three-dimensionally Structured 
Two-dimensional Materials"
https://zenodo.org/records/17246822   
2. Nanobeam 4D-STEM raw data of monolayer $WS_2-WSe_2$ lateral heterojunctions
https://zenodo.org/records/10892106 

### Dataset Size & Format:
1. Recorded at 27.5 $kx$ magnification with a 1.2 mrad convergence angle. The data includes diffraction 
patterns of monolayer $WS_2-WSe_2$ lateral heterojunctions with in-plane epitaxial interfaces.
2. 256 times 256 scan grid with 128 times 128 pixel diffraction patterns (.raw format) 

## Division of Labor
### Person 1: Diffraction Feature Extraction
1.Load the experimental 4D-STEM datasets and standardize the dynamic range for the EMPAD detector. 

2.Noise Filtering: Apply image filtering techniques (e.g., Gaussian blur or Wiener filter) prior to physical calibration to remove background noise and enhance the signal-to-noise ratio of the Bragg peaks. 

3.Perform Center of Mass (CoM) analysis or center-beam alignment at each probe position. 

4.Complete probe center calibration and execute background subtraction based on the alignment results. 
### Person 2: Strain Calculation
1.Compute the spatially averaged diffraction pattern from the entire dataset to define the system's reference lattice. 

2.Conduct dominant Bragg peak detection within the diffraction pattern at each probe position. 

3.Apply sub-pixel peak localization techniques to determine the exact positions of the peaks with high precision. 

4.Construct the local reciprocal lattice vectors for each scanning point based on the precisely located peaks. 
### Person 3: Physical Consistency & Interpretation
1.Calculate normal strain components ($\varepsilon_{xx}$, $\varepsilon_{yy}$) by comparing local reciprocal lattice spacing changes against the reference lattice. 

2.Estimate small-angle lattice rotation using linear approximations, intentionally omitting shear strain and higher-order tensor terms to ensure algorithmic robustness. 

3.Check Physical Consistency: Verify that the calculated strain magnitudes fall within physically reasonable boundaries (e.g., within the elastic limits of 2D materials) and confirm symmetry consistency. 

4.Analyze Strain Gradient: Conduct a detailed spatial analysis of how strain varies and relaxes specifically across the WS₂–WSe₂ and MoS₂–MoSe₂ heterointerfaces. 

5.Build Final Visualization Diagram: Synthesize the data arrays into intuitive, publication-quality 2D spatially resolved strain and rotation maps. 

