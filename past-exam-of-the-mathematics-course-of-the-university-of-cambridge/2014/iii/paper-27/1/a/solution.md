<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $V_t=\langle X\rangle_t$ and $S_t=\sup_{s\leq t}|X_s|$. Suppose first that $|X|\leq K$. The [Itô formula](../../../../../../ito-s-lemma.md) for $|x|^p$, which is twice continuously differentiable for $p\geq2$, gives

$$
|X_t|^p=p\int_0^t|X_s|^{p-2}X_s\,dX_s+\frac{p(p-1)}2\int_0^t|X_s|^{p-2}\,dV_s.
$$

For $p=2$, the second derivative is interpreted as the constant $2$. The stochastic term has mean zero: its integrand is bounded, and $\mathbb EV_t<\infty$ makes it a square-integrable [martingale](../../../../../../martingale-split.md). Consequently

$$
\mathbb E|X_t|^p\leq\frac{p(p-1)}2\mathbb E(S_t^{p-2}V_t).
$$

This is the first required estimate.

A bounded [local martingale](../../../../../../local-martingale.md) is a true [martingale](../../../../../../martingale-split.md). Apply the allowed [Doob Lp maximal inequality](../../../../../../doob-lp-maximal-inequality.md), and then [Hölder's inequality](../../../../../../holder-s-inequality.md) with conjugate exponents $p/(p-2)$ and $p/2$ for $p>2$. With $D_p=(p/(p-1))^p$, this yields

$$
\mathbb ES_t^p\leq D_p\frac{p(p-1)}2(\mathbb ES_t^p)^{(p-2)/p}(\mathbb EV_t^{p/2})^{2/p}.
$$

If the left side is zero there is nothing to prove; otherwise divide by its indicated power and raise to $p/2$. For $p=2$, the same conclusion follows directly from $\mathbb EX_t^2=\mathbb EV_t$ and Doob's inequality. A usable constant is therefore

$$
\boxed{\mathbb ES_t^p\leq C_p\mathbb EV_t^{p/2},\qquad C_p=\left[\frac{p(p-1)}2\left(\frac p{p-1}\right)^p\right]^{p/2}.}
$$

In particular $C_2=4$. This is the [upper maximal moment bound for a continuous local martingale](../../../../../../upper-maximal-moment-bound-for-a-continuous-local-martingale.md).

For an unbounded [continuous local martingale](../../../../../../continuous-local-martingale.md), stop at $\tau_n=\inf\{s:|X_s|\geq n\}$. Its stopped path is bounded, and its bracket at $t$ is $V_{t\wedge\tau_n}\leq V_t$. The proved inequality gives a bound by $C_p\mathbb EV_t^{p/2}$, independent of $n$. Continuity makes $\tau_n\uparrow\infty$, and the stopped maxima increase to $S_t$. [Monotone convergence](../../../../../../monotone-convergence-theorem.md) proves **the same inequality for the original unbounded process**, with the same constant. This localization step also shows that the assumed bracket moments supply all the needed maximal moments.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
