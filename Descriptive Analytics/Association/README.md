# Association Rules

For this exercise, we found the association of different transactions in a dataset and used the Apriori Algorithm to streamline the calculations.
We start by using x->y as the definition of a transaction. The antecedent (x) is associated with the consequent (y). 
X can imply Y, but that doesn't mean that Y implies X.

We measure the association of different items by using the support, confidence, and lift. 
The support measures the count of a given transaction in the dataset.
The confidence is the measurement of an association rule as a % of the antecedent present (support(x->y)/support(x)).
The lift is the confidence of an association rule over the support of the consequent.

We think about these rules as follows. 
How many times does a rule occur? (Support)
How many times does a rule occur as a % of the antecedent present? (Confidence)
Given a multiple, how much more likely is the consequent (Y) going to occur when the antecedent (X) is present? As opposed to the variables being independent. (Lift)

This is powerful for finding patterns, say, for example, consumer behavior, but it is a costly calculation. This is why we use the Apriori Algorithm.

The Apriori Algorithm uses a minimum support threshold and filters all transactions to find the most relevant ones. 
Then, it sets a minimum confidence level and finds the ones that meet the requirement. 
Then, it finds the lift and the best transactions in the dataset.

![Image Alt](https://github.com/aarern/descriptive-predictive-analytics/blob/67568aa572f898a83716c37119c1d45e84ee3cd2/Descriptive%20Analytics/Association/images/asc1.jpg)
