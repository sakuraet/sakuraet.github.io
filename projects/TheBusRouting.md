---
layout: project
type: project
image: img/bus.png
title: "Optimal Pathing of TheBus Routes"
date: 2024
published: true
labels:
  - Optimization Theory
  - Mathematical Modeling
  - Gephi
  - Python 
  - Rstudio
summary: "I contributed research in accordance with Alan Tong under HCREAM (Hawaii Center for Research and Excellence in Applied Mathematics) pertaining to TheBus routes in Oahu."
---

*Using optimization methods and graph theory, a multidimensional map was coded into Python so that using an abstract topological space, the nodes with the highest degree could be fixed. This allowed for optimization algorithims could find the shortest path based on situational parameters.*

Thompson paradox states the following: the equilibrium speed of car traffic on a road network is determined by the average door-to-door speed of equivalent journeys taken by public transport. In other words, the speed of all traffic on a road is controlled by the speed of the public transportation along that road. It is a paradox because worsening the road for private driver to improve public transportation will create more motivation to use public transportation, improving private transportation as well. This motivates research improving bus transportation in high traffic areas, such as that of Honolulu, Hawai'i. Honolulu ranks 18th worst city in the United States for the annual global traffic scorecard for 2023 by INRIX.

City bus networks are comprised of a set amount of bus stops and bus routes carrying passengers between the bus stops according to a fixed time schedule. This schedule is publicly available for almost every city bus system, with Honolulu as no exception. Therefore, Honolulu is a valid choice to perform a network analysis on.

One may perform a network analysis on a bus network by setting bus stops as vertices and bus routes connecting bus stops as edges. This creates a directed graph with multiple edges between vertices. With this structure, one may then perform a mathematical analysis of the graph and its structure.

Here is some code that illustrates how we preserved degree ranking when randomizing the bus stops:

```cpp
byte ADCRead(byte ch)
{
IGRAPH cc2c7b7 D-W- 3755 4496 -- Bus Network Rewired
+ attr: name (g/c), label (v/c), r (v/n), g (v/n), b
| (v/n), x (v/n), y (v/n), size (v/n), latitude (v/n),
| longitude (v/n), id (v/c), weight (e/n)
}
```

You can learn more at the [HCREAM Website!](https://hcream.org/blog/2024/12/31/using-network-analysis-to-research-the-oahu-bus-network/).
