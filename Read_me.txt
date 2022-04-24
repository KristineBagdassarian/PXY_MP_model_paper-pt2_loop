**Read Me file for the folder with data for the paper**

This folder contains folder 'Code' which has the codes:
- For generating the 2500 parameter sets sampled from a uniform distribution
- For solving the equations to steady state using the the parameters
- For analysing the parameter sets

Folder with all of the generated parameter sets, the solved and analysed parameter sets.

- There is a folder for all parameter sets and simulations for the case with the PXY-MP negative
feedback loop and without

- The folder 'Analysing the parameter sets' has the parameter sets generated but no solutions

- The folder 'Simulation results' contain the parameter sets and the steady state solutions resulting 
from them

- Four intervals were considered: [0,0.1], [0,1], [0, 10], [0,20]; Three independently generated
parameter set 'collections' were ran in each case, resulting in 12 sets of 2,500 parameter sets 
each for the case 'with loop' and 12 sets of 2,500 parameter sets fort he case 'no loop'.

- Simulation results contain folders for each interval. Each of those contains 3 folders with the
first, second and third iteration of the simulations. In each there is a file with the 2,500 uniformly
randomly generated parameter sets.

- The files of the 2,500 parameter sets are named Network_no_loop_uniform_interval_0_xx where xx
stands for the endpoint of the intervals

- Each folder with these simulations of the interval contains an analysis folder 'Analysis of 2500 parameter sets'
obtained from the code Testing_networks_GitHub.m

- 6 files can be found in each of those folders:

      -- All parameters that do not pattern_long - parameters and concentration 
      for all failed parameters 

      -- All parameters that do not satisfy condition and do not pattern_long - parameters and concentration 
      for all failed parameters that also don't satisfy the condition

      -- All parameters that satisfy condition but not pattern_long - parameters and concentrations of all
      parameter sets that satisfy the condition in the analysis but don't pattern

      - All parameters that do not satisfy condition and pattern_long - this file is always empty and 
      show that no parameter sets pattern without satisfying the condition

      -- Successful parameter sets_long_long - this one is
      important for further analysis as it contains the parameters and concentrations of all successul
      paramter sets from the Network_loop_uniform_interval

      -- Vector with percentage success_long - this one contains the percentage that the successful
      parameter sets make of the 2,500 (cell one); the number in the second cell is the number of successful
      parameter sets, while cell 3 has the percentage of 2,500 parameter sets

- The files of the 2,500 parameter sets for the case with the loop ALSO
 contains an analysis folder 'Successful parameter sets analysis' which usess the parameters in
Successful parameter sets_long_long.m to find which parameter sets also require the loop to be 
successful (code Separate_sets_which_require_loop_and_which_dont.m)


      -- Parameters_that_require_the_loop_to_succeed - all parameter sets that require the loop
      to succeed

      -- Parameters_that_succeed_in_both_networks - parameter sets that succeed both with and without 
      the loop

      -- Percentage_parameter_sets_that_require_loop - this one contains the percentage that the successful
      parameter sets make of number of successful parameter sets (cell one); 
      the number in the second cell is the number of successful parameter sets which require the
      loop while cell 3 has the percentage



- The folder contains a file with the analysis results summarised: 3 tables, first of which
has the number of successul parameter sets in the table with no PXY-MP loop. A table with
the number of parameter sets 