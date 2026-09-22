# Permanent as probability of distinct independent choices

↑ **Parent:** [Permanent (mathematics)](permanent-mathematics.md)

Let $X_1,\ldots,X_n$ be [independent random variables](independent-random-variables.md), each choosing a label from $\{1,\ldots,n\}$. Put their [probabilities](probability.md) in the [matrix](matrix.md) $P=(p_{ij})$, where $p_{ij}=\mathbb P(X_i=j)$. Each row sums to one. All choices are distinct precisely when their ordered list is one of the [permutations](permutation.md) of the $n$ labels. These are mutually exclusive [events](event.md), and [independence](independent-random-variables.md) makes the [probability](probability.md) of one list $\sigma$ equal to $\prod_i p_{i,\sigma(i)}$. Adding the list probabilities gives the [permanent of a matrix](permanent-mathematics.md):

$$
\mathbb P(X_1,\ldots,X_n\text{ all distinct})=\operatorname{perm}P.
$$

In particular, this permanent lies between zero and one.

For a two-person example,

$$
P=\begin{pmatrix}3/4&1/4\\1/5&4/5\end{pmatrix}.
$$

The distinct outcomes $(1,2)$ and $(2,1)$ have [probabilities](probability.md) $3/5$ and $1/20$. Therefore

$$
\operatorname{perm}P=\frac35+\frac1{20}=\frac{13}{20}=0.65.
$$

The colliding outcomes $(1,1)$ and $(2,2)$ have [probabilities](probability.md) $3/20$ and $1/5$, totaling $0.35$. All four outcomes are shown below; their [probabilities](probability.md) sum to one.

<a id="image-the-permanent-adds-the-probabilities-of-distinct-choices-two-successful-outcomes-have-total-probability-0-65"></a>
![](permanent-independent-choice-probability.png)

**[Figure 20](#image-the-permanent-adds-the-probabilities-of-distinct-choices-two-successful-outcomes-have-total-probability-0-65). The permanent adds the probabilities of distinct choices: two successful outcomes have total probability 0.65**.

If every choice has the [uniform distribution on a finite set](discrete-uniform-distribution.md) of $n$ labels, then $p_{ij}=1/n$ and the distinct-choice [probability](probability.md) is $n!/n^n$. For three choices and three labels it is $6/27=2/9$. This counts a subset of all $n^n$ ordered outcomes, not independent pairwise collision events. [Independence](independent-random-variables.md) of the original choices is essential: without it, the individual rows of $P$ do not determine the joint [probabilities](probability.md).

## ↑ Ancestors (6)

1. [Permanent (mathematics)](permanent-mathematics.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Permanent (mathematics)](permanent-mathematics.md)
