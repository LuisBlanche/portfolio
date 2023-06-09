
## Laboratory Experiment plan assistant for recipe building 


### Context 
Dataswati develops [PowerOP](https://www.dataswati.com/en/powerop) as a service intended for the food processing industry. It centralises the data from the production line (sensors, settings, ingredients, recipes, etc. ) and leverages data visualisation and machine learning to help saving resources and improve quality. 

This experiment plan assistant proof of concept was built with a customer to demonstrate the ability to accelerate and reduce the cost of a laboratory phase looking for a recipe for a new product. The idea is then to implement it as a feature of [PowerOP](https://www.dataswati.com/en/powerop) to allow for experimenting with new ingredients and new processes on existing production lines.

### Methodology 

When building an experiment plan, the laboratory comes up with a finite set of tests to explore the possibilities and rate the results to sort them and then be able to make an informed choice with the data created. The size of this set of test is constrained by the ressources limitations of the lab (time, costs, machines, people, etc.). Hence they are only able to try out a small subset of the parameter space that are chosen mostly using domain knowledge of the experts.

This project's goal was to leverage data and Bayesian Optimisation (while still relying on domain knowledge using constraints) to define the set of tests iteratively and to prove that this methodology converges faster to a satisfying result (eg: less tests for same result).

The most important part of this project was to frame it and to define the parameter space, the objective function, and the constraints. 

Then the [Meta Ax platform] (https://ax.dev/docs/bayesopt.html)  was used to create an optimization loop. The advantage of Ax is that it implements state of the art Bayesian Optimisation algorithms that allow large dimension as well as reprogramming of the parameter space, objective function or constraints at each step. That allows for human in the loop intervention to bring in that domain knowledge which is how we get the best of both worlds!

![bayesian optimisation](../assets/img/Dataswati/bayesian_optimisation.png)


We were able to show running it on historical test data that using this methodology would have allowed finding the best existing recipe much faster. We then started applying in in real time with the lab through an excel sheet that was updated by the optimization loop. Unfortunately we were not able to reach the convergence phase of the loop before the project was stopped by the customer because of lack of resources and failure of framing the correct problem on their side.


### Tools
- Microsoft Excel
- Python : ax, pandas, scikit-optimise 
- Docker for packaging 
- VSCode for development

### My involvment 

I took this project over from an intern to make it viable to use it and experiment with it with a customer. I was developing as well as exchanging with the customer.

### Results and achievements

- successfuly apply state of the art bayesian optimisation algorithms to real world data
- demonstrate the feasibility of using it to optimize the experiment plans and access better results faster 


### References
[1] J. Snoek, H. Larochelle, R. P. Adams, Practical Bayesian Optimization of Machine Learning Algorithms. Advances in Neural Information Processing Systems 26, 2012.
[2] D. Eriksson, M. Jankowiak. High-Dimensional Bayesian Optimization with Sparse Axis-Aligned Subspaces. Proceedings of the Thirty-Seventh Conference on Uncertainty in Artificial Intelligence, 2021.
[3] S. Daulton, M. Balandat, E. Bakshy. Parallel Bayesian Optimization of Multiple Noisy Objectives with Expected Hypervolume Improvement. Arxiv, 2021.
[4] D. Eriksson, P. Chuang, S. Daulton, P. Xia, A. Shrivastava, A. Babu, S. Zhao, A. Aly, G. Venkatesh, M. Balandat. Latency-Aware Neural Architecture Search with Multi-Objective Bayesian Optimization. ICML AutoML Workshop, 2021.
