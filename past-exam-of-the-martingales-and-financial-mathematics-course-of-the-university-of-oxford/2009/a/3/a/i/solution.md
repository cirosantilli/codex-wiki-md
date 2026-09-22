<h1 id="a/3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) are independent as in question 1, and all have the same probability distribution. Their [tail sigma-algebra](../../../../../../tail-sigma-algebra.md) is

$$
\mathcal T=\bigcap_{m\geq1}\sigma(X_m,X_{m+1},\ldots).
$$

An event is a tail event when it belongs to every sigma-algebra in this intersection. The [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md) says $\mathbb P(E)\in\{0,1\}$ for every $E\in\mathcal T$.

Use the intended [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) $S_n=\sum_{j=1}^nX_j$ with $S_0=0$; the printed lower summation index zero refers to an undefined $X_0$. For each $m$, removing the finite initial sum changes all later positions by one finite constant. This cannot change whether the lower limit is $-\infty$ or the upper limit is $+\infty$. Thus $B_-$ and $B_+$ belong to $\mathcal T$, and

$$
\boxed{\mathbb P(B_-),\mathbb P(B_+)\in\{0,1\}.}
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
