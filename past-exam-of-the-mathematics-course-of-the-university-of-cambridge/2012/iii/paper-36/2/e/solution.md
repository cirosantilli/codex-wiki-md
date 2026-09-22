<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the [bounded density tilt](../../../../../../bounded-density-tilt.md) $f_t=f(1+tg)$, differentiate the polynomial in $t$:

$$
\left.\frac{d}{dt}\int_0^1 f_t(u)^4\,du\right|_{t=0}
=4\int_0^1 f(u)^4g(u)\,du=P_f(4f^3g).
$$

Since every [score function](../../../../../../informant-function.md) is centered, the centered representer is

$$
\boxed{\varphi_f(u)=4\left(f(u)^3-\int_0^1 f(v)^4\,dv\right).}
$$

A bounded baseline $f$ makes this a bounded [mean-zero function](../../../../../../mean-zero-function.md), hence an element of $L^2_0(P_f)$. Thus it is the [efficient influence function](../../../../../../canonical-gradient.md) for the [density fourth-power functional](../../../../../../density-fourth-power-functional.md) relative to the regular [bounded density tilts](../../../../../../bounded-density-tilt.md). Its squared [L2 norm](../../../../../../l2-norm.md) is $16\{\int f^7-(\int f^4)^2\}$.

**A bounded baseline alone does not make this functional differentiable along every quadratic-mean differentiable path.** The [derivative](../../../../../../derivative.md) above is the intended regular-path answer. To see the need for the qualification, let $f_0=1$ and put $b(s)=6s(1-s)$ on $[0,1]$, extended by zero outside. For $0<|t|<1$, define

$$
f_t(u)=1-t^4+t^{-2}b(u/t^6),\qquad 0\leq u\leq1.
$$

Each $f_t$ is a nonnegative continuous [probability density function](../../../../../../probability-density-function.md), because its narrow bump has mass $t^4$. Moreover,

$$
\int(\sqrt{f_t}-1)^2\,du\leq\int|f_t-1|\,du\leq2t^4=o(t^2).
$$

It is therefore a [differentiable-in-quadratic-mean path](../../../../../../differentiability-in-quadratic-mean.md) with zero [score function](../../../../../../informant-function.md). Yet

$$
\int f_t^4\,du\geq t^{-2}\int_0^1b(s)^4\,ds=\frac{72}{35t^2}\longrightarrow\infty.
$$

The [density fourth-power functional](../../../../../../density-fourth-power-functional.md) is not even continuous along this [statistical path](../../../../../../statistical-path.md), although every $f_t$ is individually bounded. Consequently no [efficient influence function](../../../../../../canonical-gradient.md) represents [derivatives](../../../../../../derivative.md) over the unrestricted class of all such paths.

One sufficient additional condition is a common bound $f_t,f\leq M$ for all small $t$. [Taylor expansion](../../../../../../taylor-expansion.md) then bounds the fourth-power remainder by $6M^2(f_t-f)^2$, while

$$
\|f_t-f\|_2\leq2\sqrt M\,\|\sqrt{f_t}-\sqrt f\|_2=O(|t|).
$$

Together with the [quadratic-mean to L1 density derivative](../../../../../../quadratic-mean-to-l1-density-derivative.md), this gives $\psi(P_{f_t})-\psi(P_f)=tP_f(\varphi_fg)+o(|t|)$. Under this local bound, or when the chosen [statistical paths](../../../../../../statistical-path.md) are the [bounded density tilts](../../../../../../bounded-density-tilt.md), the boxed [canonical gradient](../../../../../../canonical-gradient.md) is fully justified. The counterexample is a [spike obstruction to density-power differentiability](../../../../../../spike-obstruction-to-density-power-differentiability.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
