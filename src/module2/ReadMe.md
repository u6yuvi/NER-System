# Train Test-Split Strategies

Common Ways to Split Dataset
1. Random Split
2. Splitting by Maximizing Divergence
3. Splitting by heurisitic
4. Splitting by perturbation


## Splitting by Maximizing Divergence
A central assumption in machine learning is that the training and test sets are from the same distribution, i.e., [they are independent and identically distributed (i.i.d.) (Gilmer, 2020)](https://en.wikipedia.org/wiki/Independent_and_identically_distributed_random_variables). But let’s drop that for a moment. We know that the i.i.d. assumption can lead to grossly overestimated model performances, but what if we evaluate the model with the “worst” possible test set?

We can obtain the “worst” test set by ensuring that the train and test sets have different distributions, i.e., they’re wholly divergent. In literature, this mode of splitting is called adversarial splits. We can measure this value using a metric called the[ Wasserstein distance](https://en.wikipedia.org/wiki/Wasserstein_metric). However, finding the right combination of train and test examples that maximizes this metric is an NP-hard problem, so[ Sogaaard et al.](https://aclanthology.org/2021.eacl-main.156/) (2021) used an approximate approach involving k-nearest neighbors with a ball-tree algorithm.

For better intution on Wesserstein distance refer to this [video](https://www.youtube.com/watch?v=CDiol4LG2Ao)