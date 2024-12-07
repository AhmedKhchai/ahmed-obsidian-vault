## The Trade-Off Between Prediction Accuracy and Model Interpretability
 - Flexibility VS restrictiveness, ex: linear regression is a relatively inflexible approach 
 - Other methods, such as the **thin plate splines** shown in Figures
 - *why would we ever choose to use a more restrictive method instead of a very flexible approach?*
	 - If we are mainly interested in **inference**, then **restrictive models** are much more **interpretable**.
		 - Ex: when inference is the goal, the linear model may be a good choice since it will be quite easy to understand the relationship between Y and X1, X2, . . . , Xp.
- ![[Pasted image 20240309114459.png]]

## Choosing the best method for a given application:
- *cross-validation* and the *bootstrap* (CHAPTER 5)

TODO: Look for labs that cover the methods discussed in ISL implemented/documented in Python 