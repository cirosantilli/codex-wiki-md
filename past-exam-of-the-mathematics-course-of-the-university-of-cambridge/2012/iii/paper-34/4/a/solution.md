<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [stochastic exponential](../../../../../../doleans-dade-exponential.md) of $M$ is

$$
\boxed{\mathcal E(M)_t=\exp(M_t-\tfrac12[M]_t).}
$$

Itô's formula gives $d\mathcal E(M)_t=\mathcal E(M)_t\,dM_t$, so it is a positive continuous local [martingale](../../../../../../martingale-split.md) starting from one. For $p>1$,

$$
\mathcal E(M)_t^p=\mathcal E(pM)_t\exp\left(\tfrac12p(p-1)[M]_t\right).
$$

Every nonnegative local [martingale](../../../../../../martingale-split.md) is a supermartingale. Hence, under $[M]_\infty\leq C$,

$$
\boxed{\sup_t\mathbb E\mathcal E(M)_t^p\leq e^{p(p-1)C/2}.}
$$

The bound applies also to stopped versions. Localize the exponential to true [martingales](../../../../../../martingale-split.md). Their uniform $L^p$ bound permits $L^1$ passage to the limit, proving that the unstopped exponential is a true [martingale](../../../../../../martingale-split.md) of mean one. The same bound makes its entire time-indexed family [uniformly integrable](../../../../../../uniform-integrability.md). This proves the [bounded-bracket criterion for a stochastic exponential](../../../../../../bounded-bracket-criterion-for-a-stochastic-exponential.md), without needing an additional exponential-moment assumption.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
