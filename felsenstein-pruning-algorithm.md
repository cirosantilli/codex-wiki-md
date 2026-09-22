# Felsenstein pruning algorithm

↑ **Parent:** [Phylogenetic tree](phylogenetic-tree.md)

The [Felsenstein pruning algorithm](felsenstein-pruning-algorithm.md) computes a site [likelihood function](likelihood-function.md) by [sum-product belief propagation](sum-product-belief-propagation.md) from leaves to root. For a finite-state [Markov kernel](markov-kernel.md) $K$, the subtree [likelihood function](likelihood-function.md) obeys $L_v(a)=\prod_{w\text{ child of }v}\sum_bK(a,b)L_w(b)$, with observed-state indicators at leaves. Summing against the root [probability distribution](probability-distribution.md) gives the site [likelihood function](likelihood-function.md). An outward pass gives edge [posterior probabilities](posterior-probability.md) and expected transition counts for the [expectation-maximization algorithm](expectation-maximization-algorithm.md).

## ↑ Ancestors (5)

1. [Phylogenetic tree](phylogenetic-tree.md)
2. [Phylogenetics](phylogenetics.md)
3. [Evolution](evolution.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Felsenstein pruning algorithm](felsenstein-pruning-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/2/solution.md)
