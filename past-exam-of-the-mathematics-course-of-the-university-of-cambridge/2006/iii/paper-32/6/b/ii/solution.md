<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First derive the [Laplace functional of a Poisson random measure](../../../../../../../laplace-functional-of-a-poisson-random-measure.md). For a simple nonnegative $g=\sum_jt_j\mathbf1_{A_j}$ on disjoint finite-intensity sets, independent [Poisson random variables](../../../../../../../poisson-distribution.md) give

$$
\mathbb E e^{-M(g)}=\prod_j\exp\bigl(\mu(A_j)(e^{-t_j}-1)\bigr)
=\exp\left(-\int(1-e^{-g})\,d\mu\right).
$$

Increasing simple approximations, [monotone convergence](../../../../../../../monotone-convergence-theorem.md) for the integrals, and [bounded convergence theorem](../../../../../../../bounded-convergence-theorem.md) for the random exponentials prove the same identity for every nonnegative measurable $g$.

Here the intensity is [Lebesgue measure](../../../../../../../lebesgue-measure.md). Put $A=B(0,r)$ and

$$
L=\exp\left(-\int_{\mathbb R^d}(1-e^{-f(x)})\,dx\right)=\mathbb E e^{-M(f)}.
$$

The integral is finite because $f$ has compact support. Apply the [Laplace functional of a Poisson random measure](../../../../../../../laplace-functional-of-a-poisson-random-measure.md) to $f+t\mathbf1_A$, $t\geq0$:

$$
\mathbb E e^{-M(f)-tN_r}
=L\exp\left(-(1-e^{-t})\int_Ae^{-f(x)}\,dx\right).
$$

Differentiate from the right at $t=0$. The difference quotient on the random side is dominated by $N_r$, which is integrable with mean $v_dr^d$; the intensity integral is over a finite-volume ball. We obtain the [count-weighted Laplace functional of a Poisson random measure](../../../../../../../count-weighted-laplace-functional-of-a-poisson-random-measure.md):

$$
\boxed{\mathbb E[N_re^{-M(f)}]
=\exp\left(-\int_{\mathbb R^d}(1-e^{-f(x)})\,dx\right)\int_{B(0,r)}e^{-f(x)}\,dx.}
$$

At $r=0$, the ball is empty and both sides are zero.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
