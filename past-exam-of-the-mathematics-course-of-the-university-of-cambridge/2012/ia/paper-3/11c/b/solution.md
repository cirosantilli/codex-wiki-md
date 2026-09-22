<h1 id="11c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the continuously differentiable [irrotational vector field](../../../../../../irrotational-vector-field.md) is defined on all of $\mathbb R^3$, as in this [vector calculus](../../../../../../vector-calculus.md) setting. A constructive [vector-field potential](../../../../../../potential-of-a-conservative-vector-field.md) with the requested negative-gradient convention is

$$
\phi(x)=-\int_0^1 x_jE_j(tx)\,dt.
$$

Since zero [curl](../../../../../../curl.md) means $\partial_iE_j=\partial_jE_i$, differentiation under the integral gives

$$
\begin{aligned}
\partial_i\phi
&=-\int_0^1\left[E_i(tx)+t x_j\partial_iE_j(tx)\right]dt\\
&=-\int_0^1\frac d{dt}\left[tE_i(tx)\right]dt=-E_i(x).
\end{aligned}
$$

Thus $E=-\nabla\phi$. This is the [Poincaré lemma](../../../../../../poincare-lemma.md) in its straight-line form, and works on any [star-shaped set](../../../../../../star-shaped-set.md) about the integration base point. Zero [curl](../../../../../../curl.md) on a domain with holes would not by itself guarantee a global [vector-field potential](../../../../../../potential-of-a-conservative-vector-field.md); the full-space hypothesis matters.

For the given field, the second component requires $\phi_y=ye^{-x^2z}$. Integration in $y$ gives $\phi=\tfrac12y^2e^{-x^2z}+C(x,z)$. Its $x$ derivative is $-xy^2ze^{-x^2z}+C_x$, and its $z$ derivative is $-\tfrac12x^2y^2e^{-x^2z}+C_z$. Comparison with the other two components forces $C_x=C_z=0$. Hence

$$
\boxed{\phi(x,y,z)=\frac12y^2e^{-x^2z}+C.}
$$

Its negative [gradient](../../../../../../gradient.md) is exactly the given field. Because this [vector-field potential](../../../../../../potential-of-a-conservative-vector-field.md) is smooth everywhere, commutation of mixed [partial derivatives](../../../../../../partial-derivative.md) gives $\nabla\times E=-\nabla\times\nabla\phi=0$, verifying irrotationality. All such [vector-field potentials](../../../../../../potential-of-a-conservative-vector-field.md) differ by a constant on the connected domain.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
