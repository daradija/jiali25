# Introduction

Metaheuristics are optimization techniques that seek to find approximate
solutions to complex problems in a reasonable time. These techniques
combine different heuristic strategies to efficiently explore the
solution space and avoid getting trapped in local optima.

Simheuristics are a combination of metaheuristics and simulation. These
techniques use simulation to evaluate the quality of the solutions
proposed by the metaheuristic. Simulation is a mathematical model that
represents a real system and allows one to study its behavior in a
controlled environment. Simulation is used to assess the performance of
the solutions proposed by the metaheuristic and guide the search toward
optimal solutions.

Simheuristics are usually guided by an optimization of a heuristic that
combines multiple objectives.

In simheuristics, simulation takes place after the optimization and
compares the optimization result by introducing noise into certain
variables.

It is found that the optimization is not always the best solution when
noise is introduced into the variables.

From a constructive viewpoint, the workflow moves from optimization to
simulation.

# Development

In this work we aim to complete a workflow that goes from simulation to
optimization. There are objectives that are difficult to optimize but
easy to simulate.

This work is based on the hypothesis that certain simulation objectives
relate to optimization objectives.

Likewise, when working under a multi-objective approach, weighting the
optimization objectives is a difficult task.

With the proposed methodology, we can, for example, aim to minimize
infrastructure costs. This is difficult from the optimization stage but
easy in the simulation stage.

It is feasible to optimize a heuristic function that combines multiple
objectives. It is feasible to determine in the simulation the cost of
other objectives. However, it is difficult to know how these objectives
affect the heuristic function.

Typically, the optimization generates a selection of elements. We can
identify the influence of the simulation objectives on these elements.
For instance, not all elements share the same heuristic. To identify the
elements is a key step in the methodology. Elements that are not
influenced by the simulation objectives can be discarded. Elements must
anotate the simulation objectives, in particular the weights of the
heuristic function. If the simulation receives extra information about
the optimization weights for the working elements, we can try to
identify the relationship between these elements and the simulation
objectives. For this, an autodifferentiation technique and a new element
called the pseudo-gradient are used.

Autodifferentiation is a technique that allows the gradient of a
function to be calculated automatically. If, during the simulation, the
gradient of the utilized elements is computed and these elements carry
information about the optimization weights, the gradient of the
optimization weights can be calculated in relation to the simulation
objectives.

With an iterative process of optimization, simulation, optimization,
simulation, and so on, we can try to minimize the optimization weights
according to the simulation objectives.

# Results

Presentation and discussion of results.

# Conclusions

Final conclusions of the work.
