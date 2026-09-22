<h1 id="27i/solution">Solution</h1>

↑ **Parent:** [27I](../27i.md)

A [sufficient statistic](../../../../../sufficient-statistic.md) has a conditional law of $X$ given $T$ independent of the parameter. An ordinary [ancillary statistic](../../../../../ancillary-statistic.md) has a distribution independent of the whole parameter. A [partial ancillary statistic](../../../../../partial-ancillary-statistic.md) for $\psi$ has a law free of $\psi$, though it may depend on the [nuisance parameter](../../../../../nuisance-parameter.md) $\lambda$. The [conditionality principle](../../../../../conditionality-principle.md) uses the conditional experiment given the observed value of $S$; removing $\lambda$ additionally requires the conditional law of $C$ given $S$ to be free of it.

The factorization requested in the PDF expresses this stronger [ancillary conditioning that eliminates a nuisance parameter](../../../../../ancillary-conditioning-that-eliminates-a-nuisance-parameter.md). There is also a normalization typo: the conditional factor must satisfy $\sum_c\phi_C(c,s;\psi)=1$ **for each fixed $s$**, rather than the printed double sum over $s$ and $c$.

Under that nuisance-eliminating interpretation, take $\phi_0(x)$ to be the parameter-free conditional probability of $X=x$ given $(C,S)$, $\phi_C(c,s;\psi)$ to be the conditional probability of $C=c$ given $S=s$, and $\phi_S(s;\lambda)$ the marginal probability of $S=s$. The conditional probability rule gives $f=\phi_0\phi_C\phi_S$, with the three separate normalizations. Conversely summing over the fibers first gives the joint law $\phi_C\phi_S$, then summing over $c$ gives $\phi_S$ and dividing gives the required conditional law $\phi_C$. The factorization also proves sufficiency of $(C,S)$.

This equivalence is not valid for ordinary ancillarity alone: a constant $S$ is always ancillary, and $T=X$ is sufficient, but conditioning on a constant generally leaves the nuisance parameter present. Thus the distinction matters to the conclusion.

For the independent [gamma distributed](../../../../../gamma-distribution.md) sample, the joint [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell(a,b)=na\log b-n\log\Gamma(a)+(a-1)\sum_j\log x_j-b\sum_jx_j.
$$

The proposed factorization would write this as a data-only term plus a function of $a$ and data plus a function of $b$ and data. It would therefore force its mixed derivative to vanish. In fact

$$
\boxed{\frac{\partial^2\ell}{\partial a\,\partial b}=\frac nb\ne0.}
$$

The [mixed log-likelihood derivative obstruction to parameter separation](../../../../../mixed-log-likelihood-derivative-obstruction-to-parameter-separation.md) rules out this exact nuisance-eliminating factorization. It does not rule out ordinary ancillary statistics: a constant statistic still qualifies, and $(\sum\log X_j,\sum X_j)$ is sufficient for the full two-parameter family.

## ↑ Ancestors (10)

1. [27I](../27i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
