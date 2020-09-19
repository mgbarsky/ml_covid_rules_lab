# Classification rules for the COVID-19 dataset

In this lab you are asked to implement the *PRISM* algorithm to extract the classification rules with the highest accuracy and coverage from the hospital patients [dataset](https://docs.google.com/spreadsheets/d/1EPewR1KdT8mszXJMuqELRTHAVIFHEJw9VwLsb9whKPI/edit?usp=sharing) described in the [class demo notebook](https://github.com/mgbarsky/ml_decision_tree_demo.git).

Your algorithm should extract the rules ranked by the accuracy (from highest to lowest), and the ties are broken by choosing the rule with higher coverage. If both accuracy and coverage are the same - the condition is selected arbitrarily.

Your algorithm should have two additional optinal parameters: 
* the accuracy threshold - the number from 0 to 1 which specifies when you need to stop refining the rule. I.e. if you reached this accuracy threshold, you do not need to add more conditions to the rule's antedescent.
* the coverage threshold - the absolute number of records covered by the rule. If the more precise rule covers less records than this threshold, the algorithm should stop refining this rule.

The output of the algorithm should be a decision list, where all the rules are presented ranked as above, including the rule itself, its accuracy, and its coverage.

We want to apply the algorithm to the COVID-19 dataset to learn reliable rules which determine which symptoms/preexisting conditions and their combination lead to the deadly outcomes of the COVID-19 infection. 

In your report (a separate markdown cell), summarize which rules did you learn from this dataset, and whether you were surpised by any of your discoveries.

