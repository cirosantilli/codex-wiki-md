<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use [left Grassmann derivatives](../../../../../../left-grassmann-derivative.md) and place the odd constant transformation parameters on the left. A [scalar superfield transformation](../../../../../../scalar-superfield-transformation.md) can be written

$$
\delta S=(\epsilon^\alpha Q_\alpha+\bar\epsilon^{\dot\alpha}\bar Q_{\dot\alpha})S,
\qquad
Q_\alpha=\partial_\alpha-i\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_\mu,
\qquad
\bar Q_{\dot\alpha}=\bar\partial_{\dot\alpha}-i\theta^\beta\sigma^\mu_{\beta\dot\alpha}\partial_\mu.
$$

Equivalently, pull back the scalar function under the infinitesimal [superspace](../../../../../../superspace.md) translation

$$
\delta\theta=\epsilon,\qquad\delta\bar\theta=\bar\epsilon,
\qquad\delta x^\mu=i\theta\sigma^\mu\bar\epsilon-i\epsilon\sigma^\mu\bar\theta.
$$

The term involving $\bar\epsilon$ has the displayed sign because interchanging it with $\theta$ reverses the sign in the [Grassmann algebra](../../../../../../grassmann-algebra.md). Overall factors of $i$ in the definition of the [supercharges](../../../../../../supersymmetry-generator.md) can be changed together without changing this coordinate transformation.

For two even scalar [superfields](../../../../../../superfield.md) $S,T$, the odd generators obey the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md), while the full parameter-weighted variation $\delta$ is even. Thus

$$
\delta(ST)=(\delta S)T+S(\delta T).
$$

This is precisely the transformation of a [product of scalar superfields](../../../../../../product-of-scalar-superfields.md). The finite version is even clearer: if $S'(z)=S(z')$ and $T'(z)=T(z')$ for the same transformed [superspace](../../../../../../superspace.md) point, then $(ST)'(z)=S(z')T(z')=(ST)(z')$. No new representation law is required.

The expression $S(x,\theta,\bar\theta)=\phi(x)$ needs a distinction between a configuration and a closed field content. As a function on [superspace](../../../../../../superspace.md), it is a valid special configuration of an unconstrained [superfield](../../../../../../superfield.md). But its variation is

$$
\delta S=(i\theta\sigma^\mu\bar\epsilon-i\epsilon\sigma^\mu\bar\theta)\partial_\mu\phi.
$$

For nonconstant $\phi$, this generates nonzero components depending on [Grassmann variables](../../../../../../grassmann-variable.md). Therefore **the pure-scalar truncation is not a supersymmetric multiplet**: an isolated spacetime [scalar field](../../../../../../scalar-field.md) with all its partners permanently set to zero is not closed under [supersymmetry](../../../../../../supersymmetry-split.md). This is the [pure-scalar truncation of a superfield](../../../../../../pure-scalar-truncation-of-a-superfield.md). A constant gauge-singlet $\phi$ is the trivial invariant exception. Calling $\phi(x)$ a special [superfield](../../../../../../superfield.md) configuration is consistent; claiming that its restricted field content remains a [superfield](../../../../../../superfield.md) representation is not.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 307](../../../paper-307-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
