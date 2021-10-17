# End-to-End Machine Learning Project
In this section, I am ganna give a intro in data visualization and fearture engineering. In addition, some important APIs of sklearn are also included. So, after fininshing reading this section, you will have a outline of how machine learning project is built and you can create your own machine learning project later. 

**IMPORTANT: ALL code are from the original book**

### Performance indicators
It gives an indication of how much error the system will usually produce in its predictions. Here I'm ganna introduce two indicators RMSE and MAE. Both of them are coming from the L-parametric mathematically. Let's see them first.

![avatar](/End-to-End_ML/RMSE.jpg)

![avatar](/End-to-End_ML/MAE.jpg)

Alright, so now, what we need to learn is to figure out when to use what and why, right? RMSE is usually the preferred performance metric for regression tasks, but if there are many outliers, we may consider using MAE. Why? The higher the number of paradigms, the more it focuses on large values and ignores small ones. For example, the l0 parametric number gives the number of non-zero elements in the vector, and the l infinity gives the maximum absolute value in the vector. Thus the higher the number of paradigms, the more it focuses on large values and ignores small values. This is the reason why RMSE is more sensitive to outliers than MAE. However, when outliers are rare in exponential form (e.g. bell curves), RMSE performs very well and is therefore usually preferred.

### Relevance analysis
As far as I am concerned, features are distint contributers of the final result. Let's imagine if two features are leading a same impact to the result, do we need both of them? The answer is **NO**, because thay have the same or similer overlapped contribution. So, to avoid or exclude overlapped features, here comes the relevance analysis.

By using `.corr()` function, we can check the relavent degree between each two features. But the correlation coefficient only measures linear correlation. So it has the potential to completely miss non-linear correlations. For example, the closer x tends to zero, the larger y is. Therefore, we need to apply some transformations to such features, which might make the results better. Alternatively, we can optimise this process by constructing new features.