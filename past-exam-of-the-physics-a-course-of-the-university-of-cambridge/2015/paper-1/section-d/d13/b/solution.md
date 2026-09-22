<h1 id="section-d/d13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Bayes' theorem](../../../../../../bayes-theorem.md) updates a hypothesis using observed data. For mutually exclusive exhaustive hypotheses $H_j$ and data $D$ of nonzero [probability](../../../../../../probability.md),

$$
\boxed{P(H_j\mid D)=
\frac{P(D\mid H_j)P(H_j)}
{\sum_kP(D\mid H_k)P(H_k)}}.
$$

The prior $P(H_j)$ describes information before these data; the [likelihood](../../../../../../likelihood-function.md) $P(D\mid H_j)$ describes the sampling model; the denominator is the evidence; and the posterior is the updated [probability](../../../../../../probability.md). [likelihood](../../../../../../likelihood-function.md) and posterior are different conditional quantities. For a continuous parameter, sums become integrals and the posterior is a [probability density](../../../../../../probability-density.md).

Consider a counter registering independent events at unknown constant rate $\lambda$, observed for known exposure $T$ with negligible background and dead time. The observed count has a [Poisson distribution](../../../../../../poisson-distribution.md):

$$
P(n\mid\lambda,T)=\frac{(\lambda T)^n e^{-\lambda T}}{n!}.
$$

Take a proper gamma prior in shape-rate convention,

$$
\pi(\lambda)=\frac{\beta^\alpha}{\Gamma(\alpha)}
\lambda^{\alpha-1}e^{-\beta\lambda},\qquad
\alpha,\beta>0.
$$

Multiplying by the [likelihood](../../../../../../likelihood-function.md) adds the count to the shape and the exposure to the rate. Normalization therefore gives

$$
\boxed{\lambda\mid n,T\sim\operatorname{Gamma}(\alpha+n,\beta+T)},\qquad
\mathbb E(\lambda\mid n,T)=\frac{\alpha+n}{\beta+T},
\quad
\operatorname{Var}(\lambda\mid n,T)=\frac{\alpha+n}{(\beta+T)^2}.
$$

Here $\beta$ has exposure units. This is [Poisson-gamma conjugacy](../../../../../../poisson-gamma-conjugacy.md). Successive independent counting runs update the same posterior by adding their counts and exposures, so the result agrees with analysing all the data together.

A [credible interval](../../../../../../credible-interval.md) contains a specified [posterior probability](../../../../../../posterior-probability.md) for $\lambda$, conditional on the chosen prior and model. For low counts, the posterior can be asymmetric and sensitive to the prior, and a symmetric Gaussian error bar can be misleading. For large $n$ and an exposure dominating prior information, the mean approaches $n/T$ and its standard deviation approaches $\sqrt n/T$. Background, missed events or time-dependent rates require a richer [likelihood](../../../../../../likelihood-function.md); [Bayes' theorem](../../../../../../bayes-theorem.md) cannot compensate for an incorrect physical counting model. The prior must be specified independently of the same data being used in the [likelihood](../../../../../../likelihood-function.md), unless its estimation is explicitly included in a larger model.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
