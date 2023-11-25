# Question-4-Brownian-motion
Q4 of reproducible research homework 

**Question 4.1**  
**Execute the code to produce the paths of two random walks. What do you observe?**  
The code shows an example of modelled randomness through Brownian motion, which can be used to model the motion of particles as a result of their collisions with other surrounding particles. These collisions are random, but can be observed through the execution of random walks. 
When the provided code is executed, two plots are produced which each demonstrate a randomly generated walk (with the same number of steps), using the ggplot2 and gridExtra packages. The plots are produced simultaneously using ncol, and demonstrate the path of the walk and the progression of time, shown through a colour gradient (earlier times are darker blue, later times are light blue). The graphs can therefore be used to show the random motion of a particle within a two-dimensional plane (x,y) according to time, and the previous movement of the particle- determined through the random orientation/angle of the particle in the 2π range, and also coordiantes randomly generated through sine and cosine functions. 
<img width="774" alt="Screenshot 2023-11-24 at 2 46 36 pm" src="https://github.com/lanonmymoush/Question-4-Brownian-motion/assets/151572854/2ea9353b-c341-4c01-bfa2-df773fdb2edb">  

**Question 4.2**  
**Investigate the term random seeds. What is a random seed and how does it work?**  
As seen in RStudio, a seed is simply an integer vector that can either be inputted into the system as a defined value or can be randomly generated through random number generators (RNGs) therefore creating a random seed. A random seed function in R will contain an RNG to produce a "randomly generated number" from a set of predefined values, i.e. a random number between 1 and n. Randomly generated integers/seeds can be either saved within a file, or saved in a specific data set which allows function to become "reproducibly random", as seen in the Brownian motion modelling, where a random angle/coordinate is generated but can then be reproduced. 
In order to make the seed more reproducible, the set.seed fucntion can also be used to ensure the initial value is the same, and the 


**Question4.3**  
**Edit the script to make a reproducible simulation of Brownian motion. Commit the file and push it to your forked reproducible-research homework repo.**
To create a reproducible simulation of Brownian motion, an initial seed must be inputted into the code which determines the point from which the rest of the code is executed. This allows "randomness" to still be achieved between the plots of random walks, however also allows the same plot to be reproduced therefore increasing the reliability and replicability of the code. 
