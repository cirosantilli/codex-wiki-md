<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First take finite endpoints $\ell<r$ and a starting point $z\in(\ell,r)$. For the [Brownian exit time](../../../../../../brownian-exit-time.md) $H=\inf\{t:B_t\notin(\ell,r)\}$, the stopped path stays in $[\ell,r]$. The process $(B_t-z)^2-t$ is a [martingale](../../../../../../martingale-split.md). Bounded-time [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
\mathbb E(H\wedge t)
=\mathbb E(B_{H\wedge t}-z)^2
\leq\max\{(r-z)^2,(z-\ell)^2\}.
$$

By the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), $\mathbb E H<\infty$, so **exit from every bounded interval is almost sure**:

$$
\boxed{\mathbb P_z(H<\infty)=1.}
$$

For completeness, a proper unbounded interval also has almost sure exit. Applying [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to $B_{H\wedge t}$ and then [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md) gives the endpoint probabilities

$$
\mathbb P_z(B_H=r)=\frac{z-\ell}{r-\ell},
\qquad \mathbb P_z(B_H=\ell)=\frac{r-z}{r-\ell}.
$$

For a fixed lower level $\ell$, let $r\to\infty$. Hitting $\ell$ before $r$ is a subset of ever hitting $\ell$, and its probability tends to one. Similarly every fixed higher level is hit almost surely. After a level is reached, the same argument from that level shows that a level strictly outside a given proper interval is eventually reached. This proves exit even when endpoints are included. A starting point already outside needs no argument. The whole real line has no exit, so the phrase “every interval” is understood to exclude that trivial exception. Countably many rational levels make the exit conclusion simultaneous for all proper intervals. The bounded-interval assertion is the one used below.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
