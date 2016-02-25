Hypothesis

A CPU-bound Ruby process (i.e. a Ruby process with enough threading such that IO waiting time is negligible) should be utilizing 1 out of N CPU cores at any given time.

Thus, an optimal tuning strategy would be to create N Ruby processes and increase number of threads until performance gains are no longer observed.
