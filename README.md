# Artificial Intelligence
This was a small project i did for artificial inteligence while studying in Poland, the idea was to find the shortest path that would pass by a defined number of cities, in a data set.
And do it both both in a brute force manner and by using a genetic algorithm and comparing the performance of both and how this changes when the dataset grows.

# Information about the project
__Initialization__ - The population can be initialized from a .txt file or at random. It can be chosen at the beginning of the main method which mode is used. There are 2 Data files (Data.txt and Data2.txt). 

__Selection__ - For the selection of the parents the roulette wheel method is used, based on the fitness of each individual. 

__Stop Condition__ - As a stop condition, the number of generations was used, and the value for that can be set up in the main method.

# Output

[![1.png](https://s4.postimg.org/fy4tiqb2l/image.png)](https://postimg.org/image/lmb49mfex/)

__Ouput of last generation found by GA__

[![2.png](https://s3.postimg.org/g8uup01pf/image.png)](https://postimg.org/image/7du0ehcwv/)

__Output of shortest path found by Brute Force__

# Fitness During Genetic algorithm

[![3.png](https://s3.postimg.org/pyy6b5tyr/image.png)](https://postimg.org/image/mfc8lcr8v/)

__Graphical Representation of 15 Cities/0.05Mutation Rate/0.85 Crossover Rate__

[![4.png](https://s3.postimg.org/xswtyjopv/image.png)](https://postimg.org/image/fdcd15alb/)

__Graphical Representation of 15 Cities/0.10Mutation Rate/0.65
Crossover Rate__

# Comparing Genetic Algorithm with Brute Force

In the main method it can be chosen whether to use Brute Force or Genetic Algorithm through a Boolean variable. While Brute Force seems to always give the optimal solution but as the number of cities to visit increases, the computation time increases exponentially and it becomes unusable, on the other hand the Genetic algorithm always finds a good solution (Might not be the optimal) but its computation is rather fast, and on a big number of cities it is the smart choice.

[![5.png](https://s3.postimg.org/cdsf6vr6r/image.png)](https://postimg.org/image/v64aagnkv/)

# Most Interesting Results

As the number of cities increases the Genetic Algorithm becomes more and more useful, considering the time it takes to find a good solution, even though it’s not the best solution, it has a good deal of time/quality of solution. For example on a 30 cities problem the initial population best fitness could be something like:

[![6.png](https://s3.postimg.org/yimq4tucz/image.png)](https://postimg.org/image/mgrcaol4f/)

__Output of a random population of 30 where the best fitness at the start was 174 and the cost 572.__

And after running the algorithm it would find a path with 289 fitness and a cost of 345, which is a big reduction.

[![7.png](https://s4.postimg.org/kmmooa2z1/image.png)](https://postimg.org/image/515d4br0p/)

__Output of the best solution found by the GA.__

The most important thing to observe is that, algorithm took 725674210 nano seconds to find a good solution, while the optimal solution would take ages to be found for example using Brute Force.
