# Regular variation

↑ **Parent:** [Real analysis](real-analysis-split.md)

A [power law](power-law.md) $q(t)=t^\rho$ responds to every fixed rescaling $t\mapsto ut$ by the same factor $u^\rho$. [Regular variation](regular-variation.md) keeps this scaling behaviour in the [limit](limit-of-a-function.md) $t\to\infty$, while allowing departures from an exact [power law](power-law.md). It is useful when the scaling exponent is stable but a smaller correction continues changing. The correction can even grow without bound.

An eventually positive [measurable function](measurable-function.md) $q$ has [regular variation](regular-variation.md) at infinity with index $\rho\in\mathbb R$ if

$$
\lim_{t\to\infty}\frac{q(ut)}{q(t)}=u^\rho
\qquad\text{for every fixed }u>0.
$$

The argument $ut$ is in the [domain of a function](domain-of-a-function.md) for sufficiently large $t$. Each $u$ is held fixed as the [limit](limit-of-a-function.md) is taken; allowing $u$ to change with $t$ is a different assertion. This is the scalar definition recalled by [Filip Lindskog, Sidney I. Resnick and Joyjit Roy, Regularly varying measures on metric spaces: hidden regular variation and hidden jumps, §3.2, p. 12](https://people.orie.cornell.edu/sid/NewForLinking/papers/RegVarMeasFinal2.pdf). The index is unique: taking $u=2$ determines $2^\rho$.

For example, on $t>1$ the [function](function-split.md) $q(t)=t^2\log t$ has

$$
\frac{q(ut)}{q(t)}
=u^2\left(1+\frac{\log u}{\log t}\right)
\longrightarrow u^2.
$$

Thus $q$ has [regular variation](regular-variation.md) of index two. Yet $q(t)/t^2=\log t\to\infty$: [regular variation](regular-variation.md) does not require [asymptotic equivalence](asymptotic-equivalence.md) to a constant times a [power law](power-law.md). Doubling $t$ gives $q(2t)/q(t)=4(1+\log2/\log t)$. At $t=100,10^4,10^6$ this is approximately $4.60206,4.30103,4.20069$, respectively. The ratio approaches four slowly, even though the exponent is exactly two in the limiting scaling law.

<a id="image-an-exact-power-law-has-a-fixed-doubling-ratio-a-logarithmic-correction-approaches-the-same-ratio-without-approaching-a-constant-multiple-of-that-power"></a>
![](regular-variation-rescaling-ratios.png)

**[Figure 10](#image-an-exact-power-law-has-a-fixed-doubling-ratio-a-logarithmic-correction-approaches-the-same-ratio-without-approaching-a-constant-multiple-of-that-power). An exact power law has a fixed doubling ratio; a logarithmic correction approaches the same ratio without approaching a constant multiple of that power**.

The [slowly varying function](slowly-varying-function.md) isolates this correction. Set $\ell(t)=q(t)/t^\rho$. Then

$$
\frac{\ell(ut)}{\ell(t)}
=u^{-\rho}\frac{q(ut)}{q(t)}\longrightarrow1.
$$

Conversely, multiplying a [slowly varying function](slowly-varying-function.md) by $t^\rho$ gives [regular variation](regular-variation.md) of index $\rho$. Hence the decomposition $q(t)=t^\rho\ell(t)$ is exact on its eventual [domain of a function](domain-of-a-function.md); it is the scaling relation, rather than the decomposition itself, that is asymptotic.

A [Pareto distribution](pareto-distribution.md) gives a decreasing example with a direct interpretation. For $x\geq1$, take the [tail probability](tail-probability.md) $\mathbb P(X>x)=x^{-2}$. Its [regular variation](regular-variation.md) index is $-2$. Doubling a threshold divides its [tail probability](tail-probability.md) by four, and

$$
\mathbb P(X>2t\mid X>t)
=\frac{\mathbb P(X>2t)}{\mathbb P(X>t)}
=\frac14
\qquad(t\geq1).
$$

For a [tail probability](tail-probability.md) with [regular variation](regular-variation.md) of index $-\alpha$, the same [conditional probability](conditional-probability.md) tends to $2^{-\alpha}$. An [exponential distribution](exponential-distribution.md) behaves differently: its corresponding conditional probability is $e^{-\lambda t}\to0$. This comparison explains why scaling limits are useful in [extreme value theory](extreme-value-theory-split.md); it does not establish that an observed dataset follows a particular tail model. The role of [regular variation](regular-variation.md) in [heavy-tailed distributions](heavy-tailed-distribution.md) is discussed in [Lindskog, Resnick and Roy, introduction, p. 1](https://people.orie.cornell.edu/sid/NewForLinking/papers/RegVarMeasFinal2.pdf).

An [exponential function](exponential-function.md) $q(t)=e^t$ is not [regularly varying](regular-variation.md) with any finite index: at $u=2$, $q(2t)/q(t)=e^t\to\infty$, rather than $2^\rho$. Boundedness alone is also insufficient, as the oscillating counterexample in [slowly varying function](slowly-varying-function.md) shows. Checking a few rescaling ratios at finite arguments can illustrate a proposed law, but cannot prove its limiting definition.

Jovan Karamata developed this theory in his 1930 paper and returned to its fundamental results in 1933. The opening of his 1933 paper identifies the earlier work; pp. 57–58 connect the rescaling limit with a [power law](power-law.md) and a slowly varying factor. See [J. Karamata, Sur un mode de croissance régulière. Théorèmes fondamentaux, Bulletin de la Société Mathématique de France 61 (1933), 55–62](https://www.numdam.org/article/BSMF_1933__61__55_0.pdf). This gives a precise language for “almost a power” without discarding corrections that remain large.

**Table of contents**

- [Slowly varying function](slowly-varying-function.md)

## ↑ Ancestors (5)

1. [Real analysis](real-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Fréchet distribution](frechet-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/3/solution.md)
- [Power law](power-law.md)
- [Regular variation](regular-variation.md)
- [Slowly varying function](slowly-varying-function.md)
