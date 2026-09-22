<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
f(\tau)=\frac{\Delta(\tau)}{\Delta(3\tau)}.
$$

For

$$
\gamma=\begin{pmatrix}a&b\\3c&d\end{pmatrix}\in\Gamma_0(3),
$$

the matrix $\gamma'=\begin{pmatrix}a&3b\\c&d\end{pmatrix}$ lies in $SL_2(\mathbb Z)$ and satisfies $3\gamma\tau=\gamma'(3\tau)$. The weight-twelve transformation law for the [modular discriminant](../../../../../../modular-discriminant.md) gives the same factor $(3c\tau+d)^{12}$ in numerator and denominator. Hence $f(\gamma\tau)=f(\tau)$, so $f$ is a weight-zero modular function of level $\Gamma_0(3)$.

The discriminant has no zero in the upper half-plane, so $f$ has neither zeros nor poles there. At infinity,

$$
\Delta(\tau)=q+O(q^2),
\qquad
\Delta(3\tau)=q^3+O(q^6),
$$

and therefore $f=q^{-2}+O(q^{-1})$: it has a pole of order two. The transformation $\Delta(-1/\tau)=\tau^{12}\Delta(\tau)$ gives

$$
f\left(-\frac1{3\tau}\right)
=3^{12}\frac{\Delta(3\tau)}{\Delta(\tau)}
=\frac{3^{12}}{f(\tau)}.
$$

The [Fricke involution](../../../../../../fricke-involution.md) exchanges infinity and zero, so $f$ has a zero of order two at the cusp zero.

Thus the morphism $\phi_f:X_0(3)\to\widehat{\mathbb C}$ has degree two, equal to its total pole order. An isomorphism of compact Riemann surfaces has degree one. Although $X_0(3)$ has genus zero, this particular morphism is therefore not an isomorphism.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
