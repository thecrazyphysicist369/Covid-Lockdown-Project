# Covid-Lockdown-Project
This is the repository that houses our covid lockdown project. We tried to check if lockdown really helps in a pandemic like covid19. Also we tried to study what kind of lockdown would be the best for the population and the economy of the population. 

## Abstract
Time immemorial, humans have been in an unending battle with pathogens. The immune systems of humans have evolved to fight against some dreadful microbes. But some have been fatal to mankind. Viruses are such an infectious agent which can replicate within living bodies and have a vast range of hosts to infect and spread. This spread might be within a local place or a country or across a huge number of countries which is recognized as a pandemic. The 2020 pandemic Covid-19 has affected 216 countries and infected 84 million people globally to date and has completely overwhelmed the worldwide healthcare system. Due to the absence of a vaccine or a proven cure, slowing down the spread was the only way to combat the virus. To curb the rate of spread, countries all over the world had adopted the strategy of complete lockdowns or a ‘stay at home’ policy for regular and irregular spans with only minimal success. In this paper, we have tried simulating the pandemic in a small world network model to understand the spread of the virus in different strategical lockdowns and if imposing complete lockdowns in a pandemic is a boon or a bane.

## Components

### Epidemiological Compartmental Model

[Compartmental Models](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology) are mathematical sets of differential equation used to study an epidemic or pandemic through time. These differential equations may be solvable or may be not. There are many kinds of compartmental model which are used by researchers for their specific research. In this project **S-E-I-R-S** model has been used. Each letter in the model means a compartment that is described in details : 
1. ***Susceptibe        (S) =*** _The compartment of Individuals who can get exposed to the virus._
2. ***Exposed           (E) =*** _The compartment of Individuals who has been exposed to the virus by someone infected. The exposed individuals do not show symptoms and do not expose other susceptible. One in every 5 exposed individuals starts to show symptoms and is moved to Infected._
3. ***Infected          (I) =*** _The compartment of Individuals who turned symptomatic are in this compartment. These individuals can expose the virus to susceptible and make them Exposed._
4. ***Recovered/Removed (R) =*** _The compartment of Individuals who have either cured from the virus and no longer Infectious or Susceptible. This also has the individuals who have died in the pandemic._

The time dependent movement of the people from one compartment to another based on the actions of the virus are goverened by sets of differential equations. Each of this equation tells us the rate of change of population in every compartment. That gives epidemiologists and virologists a solid idea of how the virus is infecting the population and how the healthcare measures needs to be placed to incur minimum damage.

### Watts-Strogatz Small World Network
![](https://github.com/thecrazyphysicist369/Voting-in-a-Small-World-Network/blob/master/swn.png)

This is a special type of graph, a small world, which depicts the human dynamics of real world in a fundamental level without all the real world abstractions.
[Watts-Strogatz](https://en.wikipedia.org/wiki/Watts%E2%80%93Strogatz_model) small world network uses 3 variables to define the network.

1. ***Nodes              =  n***   _The total number of nodes in the Small World._
2. ***Nearest neighbors  =  k***   _The number of nodes each node is connected to. Also called close-contacts._
3. ***Probability        =  p***   _This is the length of connection of the edges._

## Strategies of Lockdown

### Low Probability Low Nearest-Neighbors
```
Probability       < 0.3
Nearest-neighbors < 10
```
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/8.png)
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.2/8.png)
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.3/8.png)

_Description_

### Low Probability High Nearest-Neighbors
```
Probability       < 0.3
Nearest-neighbors > 10
```
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/20.png)
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.2/20.png)
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.3/20.png)

_Description_

### High Probability Low Nearest-Neighbors
```
Probability       > 0.7
Nearest-neighbors < 10
```
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/8.png)
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/8.png)
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/8.png)

_Description_

### High Probability High Nearest-Neighbors
```
Probability       > 0.7
Nearest-neighbors > 10
```
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/8.png)
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/8.png)
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/8.png)

_Description_


## Simulation
### Process
describe what runs in a simulation including how the compartmental-network model works in the pandemic. The tests that is conducted and quarantined. The natural recovery that happens etc etc.

### Results
![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/0.1.gif)

_Probability of 0.1_

_Nearest neighbors vary from 10 to 50_

![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Nearest%20Neighbors%2010/k10.gif)

_Nearest Neighbor 10_

_Probability vary from 0.1 to 1.0_

## Built With
Python
Networkx

## Contributing Authors

* **Shaun** - *Author* - [Twitter](https://twitter.com/thecrzyphysicst), [Google Scholar](https://scholar.google.com/citations?hl=en&user=mxc8IfcAAAAJ)
* **Annesha** - *Author* - [Twitter](https://twitter.com/anneshaghosh14)

## Acknowledgments


