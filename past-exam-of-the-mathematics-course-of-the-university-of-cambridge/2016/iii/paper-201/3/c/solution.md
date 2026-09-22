<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $b=\operatorname{ess\,sup}X_1$. The hypothesis $\mathbb P(X_1>a)>0$ implies $a<b$ and rules out a constant random variable. In particular $I(a)<\infty$. The [cumulant-generating function](../../../../../../cumulant-generating-function.md) is strictly convex, since its second derivative is the positive [variance](../../../../../../variance-split.md) under [exponential tilting](../../../../../../exponential-tilting.md), and $\psi'(0)=\mu$, $\psi'(\theta)\to b$ as $\theta\to\infty$.

If $a>\mu$, there is a unique $\theta_a>0$ with $\psi'(\theta_a)=a$, and the [Legendre transform](../../../../../../convex-conjugate.md) gives $I(a)=\theta_a a-\psi(\theta_a)$. Thus

$$
\theta_a(a+\varepsilon)-\psi(\theta_a)=I(a)+\theta_a\varepsilon>I(a).
$$

If $a=\mu$, use differentiability at zero: $\psi(\theta)=\mu\theta+o(\theta)$, so for some sufficiently small $\theta>0$,

$$
\theta(a+\varepsilon)-\psi(\theta)>0=I(a).
$$

In either case choose a parameter $\theta\geq0$ with $J=\theta(a+\varepsilon)-\psi(\theta)>I(a)$, and choose $0<\eta<J-I(a)$. The [Cramér theorem](../../../../../../cramer-s-theorem.md) gives, for all sufficiently large $n$,

$$
\mathbb P(S_n/n\geq a)\geq e^{-n(I(a)+\eta)}.
$$

The [Chernoff bound](../../../../../../chernoff-bound.md) at the chosen parameter gives $\mathbb P(S_n/n\geq a+\varepsilon)\leq e^{-nJ}$. The conditioning event has positive probability for every $n$, since all summands can simultaneously exceed $a$. Therefore

$$
\frac{\mathbb P(S_n/n\geq a+\varepsilon)}{\mathbb P(S_n/n\geq a)}
\leq e^{-n(J-I(a)-\eta)}\longrightarrow0.
$$

Taking the complement within the conditioning event proves the [conditional concentration at a large-deviation threshold](../../../../../../conditional-concentration-at-a-large-deviation-threshold.md):

$$
\boxed{\mathbb P\left(S_n/n\in[a,a+\varepsilon)\mid S_n/n\geq a\right)\longrightarrow1.}
$$

**The farther tail has a strictly larger exponential cost.** The argument also works when $a+\varepsilon$ reaches or exceeds the upper support endpoint, without requiring an interior maximizer there.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
