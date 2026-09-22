<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Substituting both profiles into the shear [traction](../../../../traction.md) condition gives

$$
2b_1A_1+\frac{b_2^2+k^2}{b_2}A_2=0.
$$

For the normal [traction](../../../../traction.md), use $Mb_1^2=Mk^2-\rho k^2c^2$ and $b_2^2+k^2=k^2(2-c^2/c_T^2)$. Removing the common nonzero factors yields the second equation. Thus

$$
\boxed{\begin{pmatrix}
2b_1&(b_2^2+k^2)/b_2\\
(b_2^2+k^2)/k&2k
\end{pmatrix}\binom{A_1}{A_2}=0.}
$$

A nonzero [displacement field](../../../../displacement-field-mechanics.md) requires the [determinant](../../../../determinant.md) to vanish:

$$
\boxed{(b_2^2+k^2)^2=4k^2b_1b_2.}
$$

Let $s=c^2/c_T^2$ and $\eta=c_T^2/c_L^2$. Cancelling $k^4$ gives the [Rayleigh secular equation](../../../../rayleigh-secular-equation.md)

$$
\boxed{(2-s)^2=4\sqrt{1-s}\sqrt{1-\eta s},\qquad0<s<1.}
$$

Squaring and excluding the zero root gives $s^3-8s^2+(24-16\eta)s-16(1-\eta)=0$; any candidate must still satisfy the unsquared equation and the decay inequalities. For stable isotropic elasticity $0<\eta<3/4$, this cubic has one root in $(0,1)$: its values at zero and one have opposite signs, and its strictly negative second [derivative](../../../../derivative.md) on this interval prevents a second crossing back to a positive final value. Both sides of the unsquared equation are positive there, so this root is valid.

The root $s=0$ of the squared equation is not a propagating surface [wave](../../../../wave-split.md): at $c=0$, the two roots coincide, and the null combination $A_2=-A_1$ in this representation produces zero [displacement field](../../../../displacement-field-mechanics.md). As a numerical example, $\lambda=\mu$ gives $\eta=1/3$ and $c\simeq0.9194c_T$. The surface-wave speed is independent of $k$ in this homogeneous half-space model.

## ↑ Ancestors (12)

1. [H](../h.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
