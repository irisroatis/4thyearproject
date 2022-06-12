# Code for 4th year Masters project
Title of Thesis: ESTIMATING PARAMETERS OF BINNED HAWKES PROCESSES

Supervisor: Dr Ed Cohen

Multivariate_Hawkes.zip contains:
- files `complete_likelihood.m`, `MCEM_algorithm_full.m`, `max_cond_pdf.m`, `disc_time_hp_grid.m`, `complete_sum_likelihood.m`, `generate_uniform_times.m` from https://github.com/lshlomovich/MCEM_Multivariate_Hawkes which implement the MCEM method
- file `fminsearchbnd.m` from https://github.com/AdamSykulski/SPG which optimises any function given
- file `SimulateMarkedHawkesMD.m` from https://karwailim.github.io/ which simulates multivariate Hawkes processes
- file `check_spectra_from_theorem_against_periodogram_multivariate.m` which implements the formula for the spectral density of a discrete-time binned Hawkes process and checks it against periodogram, resulting plots in `real11.png`, `real12.png`, `real21.png`, `real22.png`,`imag11.png`, `imag12.png`,`imag21.png` and `imag22.png`
- file `MSAWvsMCEM.m` which implements the standard Whittle likelihood and also conducts a simulation study to compare it against MCEM
