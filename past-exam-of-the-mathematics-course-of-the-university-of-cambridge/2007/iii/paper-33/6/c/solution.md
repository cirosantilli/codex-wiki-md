<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For finitely many disjoint bounded intervals $J_1,\ldots,J_r$, all dyadic cells used in their level-$n$ sums are disjoint. The independent occupied indicators proved in part (a) form independent groups, so $M_n(J_1),\ldots,M_n(J_r)$ are independent. Their almost-sure limits are also independent: for $0\leq z_j\leq1$, bounded convergence gives

$$
\mathbb E\prod_j z_j^{M(J_j)}
=\lim_n\prod_j\mathbb E z_j^{M_n(J_j)}
=\prod_j\exp(\lambda(J_j)(z_j-1)).
$$

This joint [probability generating function](../../../../../../probability-generating-function.md) determines the joint law as that of independent Poisson counts. If an interval is unbounded, truncate all intervals by $[0,R)$ and let $R\uparrow\infty$ in the joint Laplace transforms. An unbounded interval has infinite count almost surely, since its Poisson means tend to infinity; this extends the [independence](../../../../../../independent-random-variables.md) assertion to such intervals as well.

For an interval-step function $s=\sum_j a_j\mathbf1_{J_j}$ with $a_j\geq0$ and disjoint bounded intervals, independent [Poisson distributions](../../../../../../poisson-distribution.md) yield

$$
\mathbb E e^{-M(s)}=\prod_j\exp\left(\lambda(J_j)(e^{-a_j}-1)\right)
=\exp\left(-\int_0^\infty(1-e^{-s(x)})\,dx\right).
$$

We now extend this to arbitrary nonnegative Borel functions, rather than stopping at interval-step functions. The mean [measure](../../../../../../measure.md) $m(A)=\mathbb E M(A)$ is countably additive by [Tonelli theorem](../../../../../../tonelli-theorem.md), is finite on bounded intervals, and agrees with $\lambda$ on intervals by the preceding Poisson count calculation. Uniqueness of finite [measures](../../../../../../measure.md) on each bounded Borel space, then exhaustion by bounded spaces, gives $m=\lambda$ on every Borel set. Simple-function approximation therefore gives

$$
\mathbb E M(g)=\int g\,d\lambda\qquad(g\geq0\text{ Borel}).
$$

For bounded $f$ supported in a bounded interval, choose nonnegative interval-step functions $s_k$ with $\int|s_k-f|\,d\lambda\to0$. Their existence follows by approximating measurable level sets in finite [Lebesgue measure](../../../../../../lebesgue-measure.md) by finite unions of intervals, then approximating $f$ by simple functions. The mean-measure identity implies

$$
\mathbb E|M(s_k)-M(f)|\leq\int|s_k-f|\,d\lambda\longrightarrow0.
$$

The function $e^{-u}$ is one-Lipschitz on $[0,\infty)$, so the [expectations](../../../../../../expected-value.md) of the exponentials converge. The deterministic integrals of $1-e^{-s_k}$ converge by the same Lipschitz bound. Hence the Laplace formula holds for this bounded Borel $f$.

For general $f\geq0$, put $f_k=(f\wedge k)\mathbf1_{[0,k)}$. These functions increase to $f$, giving $M(f_k)\uparrow M(f)$ and $\int(1-e^{-f_k})\,d\lambda\uparrow\int(1-e^{-f})\,d\lambda$. Bounded convergence for the exponentials and [monotone convergence](../../../../../../monotone-convergence-theorem.md) for the integrals prove the [Laplace functional of a Poisson random measure](../../../../../../laplace-functional-of-a-poisson-random-measure.md):

$$
\boxed{\mathbb E[e^{-M(f)}]=\exp\left(-\int_0^\infty(1-e^{-f(x)})\,dx\right),}
$$

with $e^{-\infty}=0$.

Finally take $f=\sum_j u_j\mathbf1_{A_j}$ for disjoint Borel sets of finite [Lebesgue measure](../../../../../../lebesgue-measure.md). The formula gives the product joint Laplace transform of independent Poisson counts with means $\lambda(A_j)$. Uniqueness of that transform proves the required count laws on all Borel sets. For infinite-measure sets the formula gives $\mathbb E e^{-uM(A)}=0$ for $u>0$, so their counts are infinite almost surely. Together with the given local finiteness, these facts show that **$M$ is a Poisson random [measure](../../../../../../measure.md) with intensity $\lambda$**. This completes the [exponential void probabilities characterize a Poisson random measure](../../../../../../exponential-void-probabilities-characterize-a-poisson-random-measure.md) argument; simplicity was used to recover counts from fine-cell occupancy.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
