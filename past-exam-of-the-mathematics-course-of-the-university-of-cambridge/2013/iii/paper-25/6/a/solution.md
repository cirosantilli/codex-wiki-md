<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $a(x)=\sigma(x)\sigma(x)^{\mathsf T}$. The multidimensional [Itô formula](../../../../../../ito-s-lemma.md) gives the second-order [diffusion generator](../../../../../../diffusion-generator.md)

$$
\boxed{\mathcal L f(x)=\sum_{i=1}^d b_i(x)\partial_i f(x)+\frac12\sum_{i,j=1}^d a_{ij}(x)\partial_i\partial_jf(x).}
$$

Indeed,

$$
f(X_t)-\int_0^t(\mathcal Lf)(X_s)\,ds=f(X_0)+\int_0^t\nabla f(X_s)^{\mathsf T}\sigma(X_s)\,dW_s.
$$

The integrand is locally bounded along the continuous path after stopping on compact sets, because the coefficients and derivatives are continuous. Thus the final [stochastic integral](../../../../../../stochastic-integral.md) is a [local martingale](../../../../../../local-martingale.md). No global growth or uniqueness assumption on this already-given [weak solution of a stochastic differential equation](../../../../../../weak-solution-of-a-stochastic-differential-equation.md) is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
