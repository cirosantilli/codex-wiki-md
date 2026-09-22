<h1 id="b/7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Explore the component of one vertex by processing discovered vertices in order. At each step, the number of newly discovered neighbours is a binomial variable with at most $n$ trials and success probability $1/(2n)$, on previously unexposed independent edges. Pad each step with independent dummy trials. This couples the exploration below independent offspring variables $\xi_i\sim\operatorname{Bin}(n,1/(2n))$, each of mean one half.

If the component has at least $k\ge2$ vertices, after $k-1$ vertices have been processed at least $k-1$ offspring must have been found. Hence

$$
P(|C(v)|\ge k)\le P\left(\sum_{i=1}^{k-1}\xi_i\ge k-1\right).
$$

The sum is binomial with mean $\mu=(k-1)/2$. The multiplicative Chernoff inequality $P(B\ge2\mu)\le(e/4)^\mu$ therefore gives

$$
P(|C(v)|\ge k)\le e^{-c(k-1)},\qquad c=\tfrac12(\log_e4-1)>0.
$$

A [union bound](../../../../../boole-s-inequality.md) over all vertices bounds the probability of any component of size at least $k$ by $ne^{-c(k-1)}$. Taking $k=\lceil\alpha\log_e n\rceil$ with any $\alpha>1/c$, for example ten, makes this tend to zero. Thus **the largest component is at most a constant times $\log n$ with high probability**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
