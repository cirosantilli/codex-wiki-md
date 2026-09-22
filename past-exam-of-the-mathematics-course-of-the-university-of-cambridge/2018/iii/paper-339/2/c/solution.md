<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $u_i=(V\Lambda^{1/2})^Ta_i$. SDP feasibility implies

$$
\|u_i\|_2^2=a_i^TV\Lambda V^Ta_i=a_i^TX^*a_i\le1,\qquad
u_i^T\xi=a_i^T\widehat x(\xi).
$$

Choose $\alpha=\sqrt{2\log(2m)}$. For the uniform sign vector, whose coordinates are independent [Rademacher random variables](../../../../../../rademacher-distribution.md), the supplied bound for the [maximum of finitely many Rademacher linear forms](../../../../../../maximum-of-finitely-many-rademacher-linear-forms.md) gives

$$
\Pr\{M(\xi)\le\sqrt{2\log(2m)}\}>1-2m e^{-\log(2m)}=0.
$$

A positive-probability event in this finite space contains at least one sign vector. Thus

$$
\boxed{M(\xi)^2\le2\log(2m)\quad\text{for some }\xi\in\{-1,1\}^n.}
$$

The strict inequality in the supplied probability estimate matters: at the chosen threshold its right-hand side is zero.

For that sign vector, part (b) gives a feasible original point satisfying $\|x(\xi)\|_2^2\ge p_{\rm SDP}^*/[2\log(2m)]$. Taking the best original objective proves the unheaded concluding request as well:

$$
\boxed{\frac{p_{\rm SDP}^*}{2\log(2m)}\le v^*\le p_{\rm SDP}^*.}
$$

This is the [logarithmic approximation bound for slab-constrained quadratic maximization](../../../../../../logarithmic-approximation-bound-for-slab-constrained-quadratic-maximization.md), obtained by the [probabilistic method](../../../../../../probabilistic-method.md). It is a finite-value rounding guarantee under the spanning/attainment conditions explained above.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
