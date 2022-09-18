+++
title = "Vehicle routing planner for uMov.me"
date = "2019-10-30"
tags = [
    "metaheuristics",
    "vehicle routing",
    "industry",
    "application"
]
categories = [
    "projects"
]
+++

# Vehicle routing planner for uMov.me
<!--more-->

### The project

[uMov.me](https://www.umov.me/) is a software company with headquarters located in the south of Brazil, in the city of Porto Alegre. They offer codeless solutions for a wide variety of customers in Brazil including large retailers, pharmaceutical chain companies and logistic players.

Among their components is an automated vehicle routing planner. In 2019, I was hired by uMov.me to provide specialized Operations Research consultancy, implement and integrate an efficient vehicle routing planner into their platform to replace their previous routing technology. This project heavily used the knowledge I had developed during my BSc. and MSc. research projects.

The solver deals with many common real-world constraints in VRPs, such as time windows, vehicle capacity, pickup and delivery (paired precedences), drivers' breaks and rest periods, maximum working hours, multiple depots and flexible departure locations. In terms of objectives, one may minimize distance travelled, makespan or number of vehicles used. The solver itself uses metaheuristic techniques to provide fast, good quality and feasible solutions. In particular, it employs a combination of Iterated Local Search, Large Neighborhood Search and a specialized procedure to minimize vehicle usage. The final framework of uMov.me further allows customers to reoptimize routes in case of disruptions or last-minute orders through an intuitive user interface.

### The outcome

The routing planner, named *VRPlanner*, is actively used by many of uMov.me's customers together with other applications provided by the company, including tracking of the driver location, digital signature, photos, SMS,  and a lot more. For some of uMov.me's customers these codeless applications assisted business growth thereby helping the local economy in Brazil.

In addition to this direct impact to uMov.me's customers, uMov.me made available a [free version of VRPlanner](https://rotas.umov.me/) so that smaller business and the community can make use of the technology, while other medium and large sized business can get to know the tool and check whether it can be a valuable asset in their operations in which case they may signup for the full-fledged VRPlanner solver. 





