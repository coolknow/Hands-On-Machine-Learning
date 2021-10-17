# End-to-End Machine Learning Project
In this section, I am ganna give a intro in data visualization and fearture engineering. In addition, some important APIs of sklearn are also included. So, after fininshing reading this section, you will have a outline of how machine learning project is built and you can create your own machine learning project later. 

**IMPORTANT: ALL code are from the original book**

### Performance indicators
It gives an indication of how much error the system will usually produce in its predictions. Here I'm ganna introduce two indicators RMSE and MAE. Both of them are coming from the L-parametric mathematically. Let's see them first.

![avatar](/End-to-End_ML/RMSE.jpg)

![avatar](/End-to-End_ML/MAE.jpg)

Alright, so now, what we need to learn is to figure out when to use what and why, right? RMSE is usually the preferred performance metric for regression tasks, but if there are many outliers, we may consider using MAE. Why? The higher the number of paradigms, the more it focuses on large values and ignores small ones. For example, the l0 parametric number gives the number of non-zero elements in the vector, and the l infinity gives the maximum absolute value in the vector. Thus the higher the number of paradigms, the more it focuses on large values and ignores small values. This is the reason why RMSE is more sensitive to outliers than MAE. However, when outliers are rare in exponential form (e.g. bell curves), RMSE performs very well and is therefore usually preferred.