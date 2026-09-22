<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $f_n(q)=\mathbb P(G(n,q)\in P_n)$. This is increasing in $q$ by [monotone coupling of binomial random graphs](../../../../../../monotone-coupling-of-binomial-random-graphs.md), and $f_n(p)=1/10$ by hypothesis.

First let $q/p\to0$. Choose $k=\lfloor p/(2q)\rfloor$, so $k\to\infty$. The union of $k$ independent copies of $G(n,q)$ has distribution $G(n,q')$, where

$$
q'=1-(1-q)^k\leq kq\leq p.
$$

If any layer has $P_n$, their union has $P_n$, and hence

$$
\frac1{10}=f_n(p)\geq f_n(q')
\geq1-(1-f_n(q))^k.
$$

It follows that $f_n(q)\leq1-(9/10)^{1/k}\to0$.

Now let $q/p\to\infty$. Choose $k=\lfloor q/(2p)\rfloor$, again tending to infinity. The union of $k$ independent $G(n,p)$ graphs has parameter

$$
p'=1-(1-p)^k\leq kp\leq q.
$$

Monotonicity and independence give

$$
f_n(q)\geq f_n(p')
\geq1-(1-f_n(p))^k
=1-(9/10)^k\longrightarrow1.
$$

**Thus $p(n)$ is a threshold function.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
