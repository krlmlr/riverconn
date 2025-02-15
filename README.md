# riverconn
Git repository for R package rivercon.  

Package documentation is available in the vignette and here: https://damianobaldan.github.io/riverconn_tutorial/

Further information on functions implemented in the package and potential uses are described in the paper: https://doi.org/10.1016/j.envsoft.2022.105470

The latest version of the package is available from GitHub: https://github.com/damianobaldan/riverconn

# Installation
devtools::install_github("damianobaldan/riverconn", build_vignettes = TRUE)

# Changelog

0.3.29 to 0.3.30
* removed ggnetwork dependency

0.3.28 to 0.3.29
* fixed issue with param_l in inner_d_index_calculation function 

0.3.27 to 0.3.28
* fixed another bug in index_calculation for index_type = "sum"; added error message

0.3.26 to 0.3.27
* fixed bug in index_calculation for index_type = "sum"

0.3.25 to 0.3.26
* fixed issue in vignette visualization

0.3.24 to 0.3.25
* fixed example in d_index_calculation function

0.3.23 to 0.3.24
* updated documentation for disp_type = "leptokurtic"

0.3.22 to 0.3.23
* added disp_type = "leptokurtic" in the index_calculation function

0.3.21 to 0.3.22
* fixed bug in index_calculation when index_type = "reach" and index_mode = "from"

0.3.20 to 0.3.21
* updated documentation and vignette

0.3.18 to 0.3.20
* updated functions documentation and vignette

0.3.17 to 0.3.18
* fixed a bug that lead to index_calculation crash when similar vertex attributes are used

0.3.16 to 0.3.17
* vignette updated

0.3.16 to 0.3.17
* DESCRIPTION file updated

0.3.15 to 0.3.16
* examples changed

0.3.14 to 0.3.15
* changed matrix-vector multiplication method in index_calculation to avoid running out of memory

0.3.13 to 0.3.14
* fixed bug in t_index_calculation for index_type = "reach"

0.3.12 to 0.3.13
* updated error messages in B_ij_fun

0.3.11 to 0.3.12
* fixed bugs in examples

0.3.7 to 0.3.11
* added examples to exported functions

0.3.7 to 0.3.10
* minor fixes for CRAN upload

0.3.6 to 0.3.7
* vignette updated

0.3.5 to 0.3.6 
* added type = "sum" in index_calculation to calculate barriers attributes sum regardless of the network structure (this facilitates the calculation of area fragmentation indices)

0.3.4 to 0.3.5 
* typos corrected in the documentation

0.3.3 to 0.3.4  
* vignette updated and link to online guide included in the documentation

0.3.2 to 0.3.3  
* term dam replaced with barrier through all the documentation and vignette

0.3.1 to 0.3.2  
* vignette updated

0.2.9 to 0.3.1  
* minor changes in d_index_calculation function to avoid dplyr::join printing messages to screen

0.2.8 to 0.2.9  
* minor changes in d_index_calculation documentation

0.2.7 to 0.2.8  
* minor changes in B_ij_fun and c_ij_fun

0.2.6 to 0.2.7  
* changed architecture of B_ij_fun to improve speed (now relying on dodgr package to speed up shortest paths calculations on graphs)

0.2.5 to 0.2.6  
* changed architecture of c_ij_fun to improve speed (now relying on dodgr package to speed up shortest paths calculations on graphs)
* B_ij_fun is still the slow version

0.2.4 to 0.2.5  
* edited vignette

0.2.3 to 0.2.4  
* fixed bug on t_index_calculation (... argument and partial match issue)
* added error message on index_calculation when nodes_id is not charachter type

0.2.2 to 0.2.3  
* fixed bug on d_index_calculation (inputs pass_u and pass_d not recognized)

0.2.1 to 0.2.2  
* minor changes to functions documentation and error messages
* fixed bug on d_index_calculation (... argument and partial match issue)

0.1.9 to 0.2.1  
* changed architecture of d_index_calculation to simplify debug  
* introduced and documented function one_barrier_removal_index

0.1.8 to 0.1.9  
* fixed bug on d_index_calculation

0.1.7 to 0.1.8  
* fixed bug on set_c_directionality and set_B_directionality when argument "asymmetric" is provided  
* fixed issue on index_calculation and d_index_calculation: now output labels are consistent with user-inputted labels

0.1.7  
* first version on GitHub
