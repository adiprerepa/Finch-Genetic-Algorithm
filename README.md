# Finch-Genetic-Algorithm

This project is a genetic algorithm that randomly generates a population with each individual having random fitness levels. 
Individuals then mate, and because resources are limited, only a certain number of individuals will move on to the next generation.
There is also a feature for mutations to increase population density. In a nutshell, this is a computer generated model of natural
selection.

## How to run
You need to have java installed. To compile :`javac Main.java`

In order to run the program : `java Main`

## Whats going on
In the background, a population is generated, and each time a reproduction occurs, a new generation is generated. Every time a
generation is generated, it is printed onto the console. Because the fitnesses are random, the algorithm takes a random time to
run. I guess some fixed value implementation with the variables being environmental constants, and the population does better
or worse based on how the environment is, but eh. I am lazy. Here is a picture of how the different levels of genes can be represented
by binary.

![alt text](https://cdn-images-1.medium.com/max/800/1*BYDJpa6M2rzWNSurvspf8Q.png "gEnEs")

## The notion of natural selection

Five phases are considered in a genetic algorithm.

- Initial population
- Fitness function
- Selection
- Crossover
- Mutation

## Fitness Funtion
The fitness function determines how fit an individual is (the ability of an individual to compete with other individuals).
It gives a fitness score to each individual. The probability that an individual will be selected for reproduction is based
on its fitness score.

## Selection
The idea of selection phase is to select the fittest individuals and let them pass their genes to the next generation.

Two pairs of individuals (parents) are selected based on their fitness scores. Individuals with high fitness have
more chance to be selected for reproduction.

## Crossover (SUpEr ImPorTanT)
Crossover is the most significant phase in a genetic algorithm. For each pair of parents to be mated, a crossover
point is chosen at random from within the genes. Offspring are created by exchanging the genes of parents among 
themselves until the crossover point is reached.

## Mutation
In certain new offspring formed, some of their genes can be subjected to a mutation with a low random probability. 
This implies that some of the bits in the bit string can be flipped. Mutation occurs to maintain diversity within 
the population and prevent premature convergence. (The population development ending before developed to full potential.

## Author
Authored by Aditya Prerepa
