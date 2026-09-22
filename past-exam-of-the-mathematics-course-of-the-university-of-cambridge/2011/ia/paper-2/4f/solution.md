<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

[Pairwise independent events](../../../../../pairwise-independent-events.md) satisfy $\mathbb P(A_i\cap A_j)=\mathbb P(A_i)\mathbb P(A_j)$ for every distinct pair. [Independent events](../../../../../independent-events.md) satisfy

$$
\mathbb P\!\left(\bigcap_{i\in I}A_i\right)=\prod_{i\in I}\mathbb P(A_i)
$$

for every nonempty subset $I$ of the indices. For three events this includes the triple intersection, not just the three pairwise intersections.

Write $A_i=B_i\cup C$. Disjointness gives $\mathbb P(A_i)=p+q$, while every intersection of two or three distinct $A_i$ is exactly $C$. Thus [pairwise independence](../../../../../pairwise-independent-events.md) is equivalent to $q=(p+q)^2$. Since $p+q\ge0$,

$$
\boxed{p=\sqrt q-q.}
$$

For $0\le q\le1/16$, this is an admissible nonnegative $p$: putting $u=\sqrt q\in[0,1/4]$ gives $3p+q=3u-2u^2\le5/8<1$. The four disjoint events can therefore have the stated probabilities, with the remaining probability assigned to their complement. This also covers $q=0$.

Full [independence](../../../../../independent-random-variables.md) would additionally require $q=(p+q)^3$. Together with $q=(p+q)^2$, this forces $p+q$ to be zero or one. The first case gives $p=q=0$; the second gives $q=1,p=0$. Neither allows positive $p,q$. **There are no such mutually independent events with $p>0$ and $q>0$.**

## ↑ Ancestors (11)

1. [4F](../4f.md)
2. [Section I](../section-i.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
