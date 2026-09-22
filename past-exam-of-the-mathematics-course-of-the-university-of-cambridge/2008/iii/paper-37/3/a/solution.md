<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $N_t=\int_0^tZ_s^{-1}\,dZ_s$, the [stochastic logarithm](../../../../../../stochastic-logarithm.md) of $Z$. On each finite horizon, a strictly positive continuous path has its reciprocal bounded; stopping at levels of $Z$, $Z^{-1}$ and $[Z]$ rigorously localizes this [stochastic integral](../../../../../../stochastic-integral.md). Thus $N$ is a zero-start [continuous local martingale](../../../../../../continuous-local-martingale.md), with

$$
[N]_t=\int_0^tZ_s^{-2}\,d[Z]_s.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) for the ordinary logarithm gives

$$
\log Z_t=\log Z_0+N_t-\frac12[N]_t.
$$

Accordingly, with the exponential convention printed in this question,

$$
\boxed{M_t=\log Z_0+\int_0^t\frac{dZ_s}{Z_s},\qquad Z_t=\exp\!\left(M_t-\frac12[M]_t\right).}
$$

The initial constant in $M$ contributes no [quadratic variation](../../../../../../quadratic-variation.md). Under the standard normalized [Doléans-Dade exponential](../../../../../../doleans-dade-exponential.md) convention, which subtracts the driver's initial value in the exponent, the same formula is written $Z=Z_0\mathcal E(N)$.

For uniqueness, suppose another continuous driver $L$ gives the printed exponential. Evaluating at zero forces $L_0=\log Z_0$. Applying the [Itô formula](../../../../../../ito-s-lemma.md) to its exponential gives $dZ_t=Z_t\,dL_t$. Since $Z_t>0$, [associativity of stochastic integration](../../../../../../associativity-of-stochastic-integration.md) yields $dL_t=Z_t^{-1}dZ_t$. Thus $L_t=L_0+N_t=M_t$, up to [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md).

There is an initial-integrability qualification if “[local martingale](../../../../../../local-martingale.md)” is used with the usual integrable-initial-value definition. The displayed $M$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md) when $\log Z_0\in L^1$, in particular when $Z_0$ is a positive deterministic number. An arbitrary positive integrable $Z_0$ does not ensure this. For example, take an $\mathcal F_0$-measurable positive integer $W$ with $\mathbb P(W=n)=6/(\pi^2n^2)$ and put $Z_t=e^{-W}$ for all $t$. This is a bounded strictly positive [martingale](../../../../../../martingale-split.md), but any representing driver must have $M_0=-W$, which is not integrable. Thus the unqualified claim is false under that definition. For general $Z_0$, the always-valid local-[martingale](../../../../../../martingale-split.md) statement is the zero-start representation **$Z=Z_0\mathcal E(N)$**; the printed representation additionally requires the stated integrability or the convention that allows arbitrary finite initial constants.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
