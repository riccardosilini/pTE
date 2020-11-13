# pTE

pseudo transfer entropy

This python code can be used in order to compute causality between processes.
N processes may be used as input and the bivariate causality will be computed between each pair,
returning an NxN causality matrix. The results in case of systems composed by only 2 processes are very similar to those
that can be obtained using Granger causality, but faster for time series up to 500 points.

WARNING: For systems composed by 3 or more processes fakes causalities, like indirect causalities, can appear.
This code allows to avoid fake causalities in the case of 3 processes, but for 4 or more, it is still a work in
progress.

# time shifted surrogates

In the pTE.ipynb file it is also possible to find an efficient function to create time shifted surrogates, called
timeshifted().

# Who should use it?

This code can be very useful to drastically reduce the computational time for the computation of causality in case of
large datasets composed by relatively short time series (<500 data points), in particular using time shifted
surrogates for significance testing
