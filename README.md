# SEAIRD_Odes
This is a repository created for people who are trying to solve a ode's system related to compartimental epidemiological models. 

## April 2023
The script AjusteNL.py is a class where you can perform a non linear optimization using the curve_fit method included in scipy, this optimization includes the numerical solution of our system of ode's based on compartimental epidemiological models. The first approximation is the most common one, considering 3 classes to clasiffy the total population, susceptible people (S) are those that have not been infected in a time instant $t$, the infected people (I) are those that got the ill and can spread it to the susceptible population, and the recovered people (R), those are the part of the population that have been infected but they are already cured.
The compartimental models have some assumptions to consider: 

- The sum of all the members of all classes in any time $t$ is the same, i.e. constant: $S + I + R  = N$ where N is the total population.
- The dinamic of the populatios it's supposed homogeneous between all the classifications, and each member follows the same behavior, here we made an aproximation to the behavior of the people skipping the social and economic factors   
