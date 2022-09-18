+++
title = "Truck driver scheduling"
date = "2022-09-08"
tags = [
    "algorithms",
    "vehicle routing",
    "scheduling",
    "academic",
    "human factors"
]
categories = [
    "projects"
]
+++

# Truck driver scheduling
<!--more-->

### Break scheduling with interdependent routes

Truck driver scheduling with interdependent routes was my first research topic in my PhD at KU Leuven. The problem was inspired by a real-world large transportation company in Belgium which needed an automated vehicle routing solver. Among their main requests was the fact that routes should comply with European Union regulations on driving time activities during single-day trips. Essentially this translates to the need of performing break scheduling and departure time selection for the drivers to comply with both resting requirements and maximum working hours.

These driving constraints needed to be respect simultenously to customer time windows and possible synchronization between routes of multiple drivers. In VRP terms, routes could contain load transfers, creating a temporal dependency between them where decisions taken in one route (e.g., scheduling a break period) could have impacts in decision of other routes, leading to a highly complex scheduling problem. We have named this type of route dependency as *interdependent routes* and have been investigating related problems since then.

We have developed two special-purpose algorithms for break scheduling. The first algorithm follows the Truck Driver Scheduling literature and employs a Label Propagation scheme. This worked well only when one type of interdependency constraint existed, namely, the minimum difference constraint which occurs in scenarios with load transfer. When more complex interdependency constraints arise, for example synchronization, overlap or min-max difference, then the label propagation method demonstrated limited performance.

To solve more general types of interdependency, we identified properties of truck driver schedules and developed a Two-stage Algorithm based on recursive tree search. This method showed very promising results in all of our experiments while being conceptually simple.

Our research on this topic has been published in:
1. Sartori, C. S., Smet, P., & Berghe, G. V. (2022). Scheduling truck drivers with interdependent routes under European Union regulations. *European Journal of Operational Research*, 298(1), 76-88.
2. Sartori, C. S., Smet, P., & Berghe, G. V. (2022). Truck driver scheduling with interdependent routes and working time constraints. *EURO Journal on Transportation and Logistics*, 100092.

### Duration-based workload balancing with interdependent routes

In addition to break scheduling, another topic which we touched upon during my PhD research was workload balancing in the context of interdependent routes. In this case, we investigated how to evaluate the workload of drivers whose routes are interdependent and the workload metric is the route's duration. The goal is to define the starting time of each route (or driver's shift) to comply with all constraints and minimize one of the two objective function:

1. Min-max: minimize the longest route duration.
2. Range: minimize the difference between the longest and shortest route.

We presented three approaches to compute these objective functions and provided experimental results comparing the methods to understand which one works best when solving VRPs in practice. The full study has been published in the ALGO/ATMOS 21 conference:

- Sartori, C., Smet, P., & Vanden Berghe, G. (2021). Efficient Duration-Based Workload Balancing for Interdependent Vehicle Routes. In *21st Symposium on Algorithmic Approaches for Transportation Modelling, Optimization, and Systems (ATMOS 2021)* (Vol. 96, pp. 1-15). Dagstuhl Open Access Series in Informatics.

### Achievements

Our paper on workload balancing received the [Best Paper Award](https://drops.dagstuhl.de/opus/volltexte/2021/14869/pdf/OASIcs-ATMOS-2021-0.pdf) at the ALGO/ATMOS 21 conference.
