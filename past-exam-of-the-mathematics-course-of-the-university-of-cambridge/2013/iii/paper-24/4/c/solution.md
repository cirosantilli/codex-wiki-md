<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Relative to a [filtration](../../../../../../filtration-probability-theory.md) $(\mathcal F_t)$, [progressive measurability](../../../../../../progressive-measurability.md) means that, for every $T<\infty$, the map

$$
[0,T]\times\Omega\longrightarrow\mathbb R,\qquad (t,\omega)\longmapsto X_t(\omega)
$$

is measurable for the [product sigma-algebra](../../../../../../product-sigma-algebra.md) $\mathcal B([0,T])\otimes\mathcal F_T$ and the [Borel sigma-algebra](../../../../../../borel-sigma-algebra.md) on $\mathbb R$.

Fix $T>0$ and divide $[0,T]$ into $2^m$ equal subintervals with mesh $h_m=T/2^m$. Define

$$
X^{(m)}_t=
\sum_{k=1}^{2^m}X_{kh_m}\mathbf1_{[(k-1)h_m,kh_m)}(t)
+X_T\mathbf1_{\{T\}}(t).
$$

Since $X$ is [adapted](../../../../../../adapted-process.md), every [random variable](../../../../../../random-variable-split.md) $X_{kh_m}$ is $\mathcal F_{kh_m}$-measurable, hence $\mathcal F_T$-measurable. Each approximation is consequently $\mathcal B([0,T])\otimes\mathcal F_T$-measurable. For $t<T$, its sampling time lies strictly to the right of $t$, tends to $t$, and never exceeds $T$. [Right continuity](../../../../../../right-continuous-function.md) implies $X^{(m)}_t\to X_t$; at $T$ equality is exact. Thus $X$ is the pointwise limit of measurable functions on this product space. As $T$ was arbitrary, **$X$ is [progressively measurable](../../../../../../progressive-measurability.md)**. This is the theorem that [right-continuous adapted processes are progressively measurable](../../../../../../right-continuous-adapted-processes-are-progressively-measurable.md).

The right-endpoint approximations need not themselves be adapted at their intermediate times. What the proof requires is their joint measurability with respect to the single terminal sigma-algebra $\mathcal F_T$. The proof uses the pathwise [càdlàg](../../../../../../cadlag.md) convention. If path regularity is assumed only [almost surely](../../../../../../almost-sure-convergence.md), under a completed filtration setting the [stochastic process](../../../../../../stochastic-process-split.md) to zero on its common exceptional null event gives an [indistinguishable](../../../../../../indistinguishability-of-stochastic-processes.md) [progressively measurable](../../../../../../progressive-measurability.md) version. Arbitrary values on that null event need not make the original [stochastic process](../../../../../../stochastic-process-split.md) [progressively measurable](../../../../../../progressive-measurability.md): even with a complete filtration, a null sample point may be assigned a non-Borel time function. This is why [almost sure path regularity does not ensure progressive measurability](../../../../../../almost-sure-path-regularity-does-not-ensure-progressive-measurability.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
