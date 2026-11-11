NOTES ON THE DATA SET FROM FEHR AND GOETTE (2006), "DO WORKERS WORK MORE WHEN WAGES ARE HIGH? EVIDENCE FROM A RANDOMIZED FIELD EXPERIMENT"

Ernst Fehr and Lorenz Goette

These notes describe how the results from Fehr and Goette (2006) can be replicated. They also describe the information we omitted to protect confidential business information and confidential personal information.

For every section below, there is a dta-file and a do-file that perform parts of the data analysis. The sections explain which part is of the analysis is performed and what information is omitted.

If the dofiles and data sets are put in the same directory, and stata is switched to that directory (using the cd command), they will run through, reproducing the entries to all our regressions, and the data in the descriptive tables and figures.

1. dailycorrs
Reproduces the correlations in total revenues between Flash and Veloblitz.

2. tables1to4
Reproduces the results in Tables I through IV. To protect the privacy of the messengers on which we have data have replaced the actual messenger IDs used by the firms with a messenger identifier (the variable is called "fahrer").
The key variables are: (i) odd: A dummy variable, indicating what group a messenger was assigned to (odd messenger ID = group A, even messenger ID = group B). Careful, it's based on the real messenger ID, not the identifier we provide here. (ii) maxhigh: An indicator variable for those messengers participating in the experiment.All other variables should be clear from the context when comparing the output to the tables in the paper. Comments in the do-file indicate which statement produces which table.
Standard errors of the means for any table are not computed in Stata, but later in Excel, by simply dividing the appropriate standard deviation by the square root of the number of observations.

3. tables5to6
This reproduces the regression results for Tables V and VI, as well as Figures 1 and 2.
The key variable is log revenues per shift, called lnum. All other variables are explained in the dofile or self-explanatory when compared to Tabless V and VI in the paper.
