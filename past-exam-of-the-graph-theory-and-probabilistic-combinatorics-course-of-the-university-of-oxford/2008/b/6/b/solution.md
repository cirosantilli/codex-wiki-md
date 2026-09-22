<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The event $K=k$ implies $S_k=0$. If $B_k$ counts the positive increments, then $B_k\sim\operatorname{Bin}(k,p)$ and $S_k=1+2B_k-k$. Let $\delta=|p-1/2|>0$.

For $p>1/2$, $S_k=0$ forces $B_k=(k-1)/2\le k/2$, so the lower-tail Hoeffding form of the [Chernoff bound](../../../../../chernoff-bound.md) gives

$$
\mathbb P(K=k)\le\mathbb P(B_k-kp\le-\delta k)\le e^{-2\delta^2k}.
$$

For $p<1/2$ and $k\ge1/\delta$, the required value is at least $kp+\delta k/2$. The upper-tail bound gives $\mathbb P(K=k)\le e^{-\delta^2k/2}$.

To include all smaller positive integers, note that each finite-time atom has probability strictly less than one: at $k=1$ its probability is $1-p<1$, while for $k>1$ immediate extinction already has positive probability and excludes $K=k$. Over the finitely many small $k$ with nonzero atom, take the minimum of $-k^{-1}\log\mathbb P(K=k)$ and the applicable tail constant. This minimum is positive, and zero atoms impose no restriction. Thus for both cases there is $c>0$ such that

$$
\boxed{\mathbb P(K=k)\le e^{-ck}\quad\text{for every positive integer }k}.
$$

In the supercritical case this bounds the finite atoms, not the positive probability of $K=\infty$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
