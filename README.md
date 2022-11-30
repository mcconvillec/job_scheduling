# job_scheduling

This repository provides a simplifed/sanitzed version of a constraint programming model developed to help optimise the scheduling of customer product migrations for a major company, overall enabling them to more proactively manage their product lifecycle.

Several constraints exist on the solution space that must be navigated by the solver, notably:

1) Each job consists of a sequence of tasks which must be performed in a given order
2) Each task must be completed by a specific machine/resource

The objective is to minimise the length of time it takes to complete all tasks.

A key reason constraint programming was chosen for this problem rather than MILP or other forms of integer programming was the fewer number of constraints/decision-variables that needed to be included in the model given the lack of a linearity requirement.

View code <a href="https://github.com/mcconvillec/job_scheduling/blob/main/job_scheduling.ipynb">here</a>
