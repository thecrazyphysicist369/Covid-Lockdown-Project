# Covid-Lockdown-Project
This is the repository that houses our covid lockdown project. We tried to check if lockdown really helps in a pandemic like covid19. Also we tried to study what kind of lockdown would be the best for the population and the economy of the population. 

## Abstract


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


## Running the tests

![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Probability%200.1/0.1.gif)

_Probability of 0.1_

_Nearest neighbors vary from 10 to 50_

![](https://github.com/thecrazyphysicist369/Covid-Lockdown-Project/blob/main/Images/Nearest%20Neighbors%2010/k10.gif)

_Nearest Neighbor 10_

_Probability vary from 0.1 to 1.0_


### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing
* **Shaun** - *Author* - [Twitter](https://twitter.com/thecrzyphysicst), [Google Scholar](https://scholar.google.com/citations?hl=en&user=mxc8IfcAAAAJ)
* **Annesha** - *Author* - [Twitter](https://twitter.com/anneshaghosh14)
## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
