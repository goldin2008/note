## DS Interview

1. what is 95% CI ， 给了个例子how to get the population response rate from sample given the 95% ci.
2. 给了个例子，age~ height+weight 问了multicollinearity的问题，要求解释，完了问一般情况下怎么detect
3. 给了个 fund raising 例子，5000 alumni，1000 variables build a model to see the probability to make the donation, 这个case 还问了包括 variables selection and model vailidation的问题
4. missing value problem. 有些applicants 没有透露 income， 然后他们用average income做了填充，问这样好不好，或者你有别的什么办法吗

一些别处找来的面经，自己面试前用来准备的
what is p value, what is significance level, what is mean and variance
what is mean by strongly postitively related
how to select variables from thousands of them
一些case
1. 之前response rate 10% 现在变成18% 设计hypothesis test 来确定新的电话营销方案是真的提高而不是偶然发生的。
2. 怎样在不增加cost的情况下使得response rate 升高。
3. prsidential poll obama52% Romney49% margin error 3%， what is your conclusion.

被问到不同model为什么learning curve不同，multi-correlation怎么处理。主要是针对你用的model和feature提问。建议大家弄清自己为什么用某个方法以及用它的目的。

比方说hadoop和spark的区别和原理

问我map reduce的工作流程， spark跟map reduce的区别？

gradient descent 的pesudo

## DS
***Feature Selection*** is the process of selecting the attributes that can make the predicted variable more accurate or eliminating those attributes that are irrelevant and can decrease the model accuracy and quality.

***Data Correlation*** is a way to understand the relationship between multiple variables and attributes in your dataset. Using Correlation, you can get some insights such as:
- One or multiple attributes depend on another attribute or a cause for another attribute.
- One or multiple attributes are associated with other attributes.

So, why is correlation useful?
- Correlation can help in predicting one attribute from another (Great way to impute missing values).
- Correlation can (sometimes) indicate the presence of a causal relationship.
- Correlation is used as a basic quantity for many modelling techniques

***Multicollinearity*** happens when one predictor variable in a multiple regression model can be linearly predicted from the others with a high degree of accuracy. This can lead to skewed or misleading results. Luckily, decision trees and boosted trees algorithms are immune to multicollinearity by nature. When they decide to split, the tree will choose only one of the perfectly correlated features. However, other algorithms like Logistic Regression or Linear Regression are not immune to that problem and you should fix it before training the model.

How Can I Deal With This Problem?
There are multiple ways to deal with this problem. The easiest way is to delete or eliminate one of the perfectly correlated features. Another way is to use a dimension reduction algorithm such as Principle Component Analysis (PCA).

### References

#### Machine Learning Algorithms In Layman’s Terms
> https://towardsdatascience.com/machine-learning-algorithms-in-laymans-terms-part-1-d0368d769a7b

> https://towardsdatascience.com/machine-learning-algorithms-in-laymans-terms-part-2-a0a74df9a9ac

> https://www.kdnuggets.com/2020/03/linear-logistic-regression-explained.html

> https://communities.sas.com/t5/SAS-Communities-Library/Decision-Tree-in-Layman-s-Terms/ta-p/571690#

> https://www.experfy.com/blog/ai-ml/machine-learning-algorithms-in-laymans-terms-part-1/

> https://www.experfy.com/blog/ai-ml/machine-learning-algorithms-in-laymans-terms-part-2/

#### Statistics
> https://www.cnblogs.com/Belter/p/5923828.html


## Consulting Prep

> https://www.youtube.com/user/MConsultingPrep/videos

> https://www.myconsultingcoach.com/case-interview

> https://managementconsulted.com/case-interview-structure/

> https://www.craftingcases.com/case-interview-examples/