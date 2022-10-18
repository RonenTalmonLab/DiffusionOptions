# DiffusionOptions

The code in this repository creates the figures presented in this article:
http://proceedings.mlr.press/v119/bar20a/bar20a.pdf

The code is self contained and was tested using Matlab 2018b.

The main file is "Main.m". It calls all the other functions and scripts.

Inside Main.m, in lines 14-16 there are flags controling the created domain. 
Please note that only one of the flags should have a logical '1' value at a time. 
The parameter _DiffusionTime_ in line 23 sets the t scale parameter of the algorithm.

Figures 1 and 2 in the paper are created by running "Main.m" with different domain flags and a scale parameter t.

Figure 3 in the paper is created by running "Main.m" using the flag _IsStochasticDomainFlag = 1_ (line 19).

The data in Table 1 was created by running "Main.m" using the flag _IsExplorStepsStatesFlag_ (line 21).
Choosing between diffusion options, eigen options and random walk is done by setting the flags in the file "DiffutionTimeCalcWithOptions.m", lines 13 and 14. 
The flag _DiffusionOptionsFlag_ controls which set of options is used, and the flag _OnlyPrimitiveAction_ enforces only primitive actions (thus, should be disables when options are used).

The results (for the corresponding aforementioned flags) appear in the console at the end of the run.
