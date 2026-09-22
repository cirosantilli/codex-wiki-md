<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Multiply the [Beta distribution](../../../../../../beta-distribution.md) density of $p_M$, the conditional [binomial distribution](../../../../../../binomial-distribution.md) mass of $X$, and the conditional [Beta distribution](../../../../../../beta-distribution.md) density of $p_T$. With $B(a,b)$ the [beta function](../../../../../../beta-function.md), the full joint density, relative to counting measure in $x$ and Lebesgue measure in the two probabilities, is

$$
\boxed{f(p_T,x,p_M)=\frac{\binom nx}{B(\alpha,\beta)B(\alpha+x,\beta+n-x)}
(p_Tp_M)^{\alpha+x-1}[(1-p_T)(1-p_M)]^{\beta+n-x-1}.}
$$

Here $x=0,\ldots,n$ and both probabilities lie in $(0,1)$. **The printed joint expression omits the factor $1/B(\alpha+x,\beta+n-x)$.** It is a constant when $x$ is fixed and only the two probabilities vary, but is not a constant for the full [joint probability distribution](../../../../../../joint-probability-distribution.md). Keeping it is essential when summing over the [latent variable](../../../../../../latent-variable.md).

## ↑ Ancestors (11)

1. [H](../h.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
