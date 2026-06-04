# Final Year Project: Benchmarking Identity-by-Descent Segment Detection in Highly Polymorphic Anopheles gambiae Populations Using Coalescent Simulations


This repository contains the complete codebase, simulation scripts, and analysis pipelines developed for my undergraduate thesis at Imperial College London (2026).

1. Environment & Prerequisites:
To replicate the results, ensure you have the following environments and tools installed:
	•	Python 3.13.9 (with libraries: msprime, tskit, pandas, numpy and matplotlib.)
	•	Java v21.0.10 (required for executing toolchains in bash_scripts)
2. Project Structure:
	•	/data - Contains simulation input/output files.
	•	/result - Contains IBD algorithmic files (IBDseq, Refined IBD) and figures.
	•	01_Baseline_Simulation.ipynb - Core simulation script.
	•	README.rtf - This instruction file.
	•	bash_scripts - Contains the exact command lines used to execute IBDseq and Refined IBD via the terminal (bash).
3. Execution Steps:
	•	Step 1: Run 01_Baseline_Simulation.ipynb to simulate genetic data. (Outputs are saved using relative paths in the /data folder).
	⁃	Note: To test different simulation scenarios, simply modify the recombination rate (r) and mutation rate (µ) parameters in the setup cell of this notebook.
	•	Step 2: Run the command lines for IBDseq and Refined IBD (The exact command lines I typed in terminal are all recorded in bash_scripts.rtf).
	•	Step 3: Run '02_IBDcallerAnalysis.ipynb' to process the tool outputs and plot length distribution figures.
	•	Step 4: Run '03_Power&Accuracy.ipynb' to process the tool outputs and evaluate performance against the ground truth.
	•	Step 5: Run '04_Plotting.ipynb' to reproduce the final metrics plots.

4. Notice:
	•	To run simulations with different recombination rates (r) and mutation rates (µ), simply modify the recombination_rate and mutation_rate parameters



