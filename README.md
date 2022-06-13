# Code for 4th year Masters project
### Title: ESTIMATING PARAMETERS OF BINNED HAWKES PROCESSES

plot_intensity_counting_process_hawkes.zip contains:
- files to generate conditional intensity plot and its corresponding counting process, modified version of https://uk.mathworks.com/matlabcentral/fileexchange/17983-simulate-a-hawkes-process?s_tid=prof_contriblnk


Univariate_Hawkes.zip conrains:
- files `complete_likelihood.m`, `MCEM_univariate.m`, `max_cond_pdf.m`, `disc_time_hp_grid.m`, `complete_sum_likelihood.m`, `generate_uniform_times.m`,`complete_likelihood_univariate.m`, from https://github.com/lshlomovich/MCEM-Univariate-Hawkes which implement the MCEM method
- file `fminsearchbnd.m` from https://github.com/AdamSykulski/SPG which optimises any function given
- file `SimulateMarkedHawkes1D.m` from https://karwailim.github.io/ which simulates multivariate Hawkes processes
- file `example_run_likelihood.m` which generates univariate Hawkes and estimates parameters from observed event times (NOT BINNED)
- file `plot_check_periodogram_against_spectra_univariate.m` which implements the formula for the spectral density of a discrete-time binned Hawkes process and checks it against periodogram
- file `Simulating_1D_binned_data.m` which simulates the artificial data to be used, results in `simulation_1d_binned1.txt` and `simulation_1d_binned2.txt`
- file `lwitt.m` and `lwittD.m` code the different versions of Whittle (SW, STW, SDW, SAW, STAW, DW, DTW, DF), inspired by https://github.com/AdamSykulski/SPG
- file `compare_estimation_methods.m` which implements the versions of Whittle likelihood and also conducts a simulation study to compare it against MCEM
- folder `figures` contains the resulting figures

Multivariate_Hawkes.zip contains:
- files `complete_likelihood.m`, `MCEM_algorithm_full.m`, `max_cond_pdf.m`, `disc_time_hp_grid.m`, `complete_sum_likelihood.m`, `generate_uniform_times.m` from https://github.com/lshlomovich/MCEM_Multivariate_Hawkes which implement the MCEM method
- file `fminsearchbnd.m` from https://github.com/AdamSykulski/SPG which optimises any function given
- file `SimulateMarkedHawkesMD.m` from https://karwailim.github.io/ which simulates multivariate Hawkes processes
- file `check_spectra_from_theorem_against_periodogram_multivariate.m` which implements the formula for the spectral density of a discrete-time binned Hawkes process and checks it against periodogram, resulting plots in `real11.png`, `real12.png`, `real21.png`, `real22.png`,`imag11.png`, `imag12.png`,`imag21.png` and `imag22.png`
- file `MSAWvsMCEM.m` which implements the standard Whittle likelihood and also conducts a simulation study to compare it against MCEM, resulting saved estimates in `my_parameters.mat` and `mcem_parameters.mat` and comparison plots in `a11.png`, `a12.png`, `a21.png`, `a22.png`, `b11.png`, `b12.png`, `b21.png`, `b22.png`, `l1.png`, `l1.png`
