+++
title = "Short industry-related projects"
date = "2022-04-14"
tags = [
    "metaheuristics",
    "optimization",
    "industry",
    "application"
]
categories = [
    "projects"
]
+++

# Short industry-related projects
<!--more-->

These are two projects developed during my PhD at KU Leuven which are related to companies in Belgium. However, the projects are by no means related to each other in terms of the problem being solved, they are merely projects unrelated to any other part of my research.


### Project A: Production scheduling

In the first project, a company that manufactures components needed help to schedule production on two parallel machines. However, they had additional constraints involving staff availability and cost to operate these machines, skills, preventive maintenance in addition to stock constraints given that they had a limited amount of space to store produced components before shipping them. Shipping could be performed in a few specific days and part of the solution process was also deciding when shipment of components should take place in order to respect stock limitations.

We developed a metaheuristic algorithm using Late Acceptance Hill Climbing and specialized local search moves to schedule production blocks. Our research included a sensitive analysis about parameters of the production process and how revenue could potentially be increased.

A paper describing our research was published:
- Sartori, C. S., Gandra, V., Çalık, H., & Smet, P. (2021, September). Production Scheduling with Stock- and Staff-Related Restrictions. In *International Conference on Computational Logistics* (pp. 142-162). Springer, Cham.

### Project B: Periodic vehicle routing

The second project involved a valuable goods transportation company. Their customers required periodic visits throughout Belgium for collection and delivery of goods. Some customers had fixed delivery schedules while others where flexible and only stipulated a minimum visit frequency. Additional constraints included vehicle capacity, time windows, maximum working hours and flexible start times. The goal was to minimize costs incurred by travel time (fuel consumption) and personnel cost to operate the routes. 

We have also developed a LAHC-based metaheuristic with specialized moves for scheduling visits in multiple days (periodicity) combined with vehicle routing procedures within the same day (period) to improve solution cost. The research also considered how certain objectives could interact with solution characteristics.

A paper with out findings was published:
- Gandra, V., Sartori, C. S., Çalık, H., & Smet, P. (2022, July). Multi-depot periodic vehicle routing with variable visit patterns. In *Proceedings of the Genetic and Evolutionary Computation Conference Companion* (pp. 2019-2026).
