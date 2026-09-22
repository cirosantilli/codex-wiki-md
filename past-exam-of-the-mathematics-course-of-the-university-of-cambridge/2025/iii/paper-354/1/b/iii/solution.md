<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

When $J(x)$ varies, the radial wave equation recursively generates local derivative terms before the normalizable response. Substituting

$$
\phi=J+z^2\phi_{(2)}+z^4\phi_{(4)}+z^5A+\cdots
$$

into

$$
z^2\phi_{zz}-4z\phi_z+z^2\Box_5\phi=0
$$

gives

$$
\phi_{(2)}=\frac16\Box_5J,
\qquad
\phi_{(4)}=\frac1{24}\Box_5^2J.
$$

Because the boundary dimension is odd, no logarithmic term is required. [Holographic renormalization](../../../../../../../holographic-renormalization.md) subtracts these source-dependent pieces, leaving

$$
\boxed{
\mathcal O(x)=
\lim_{z\to0}z^{-5}
\left[
\phi(z,x)-J(x)
-\frac{z^2}{6}\Box_5J(x)
-\frac{z^4}{24}\Box_5^2J(x)
\right]}
$$

in the normalization $\mathcal O=A$. Equivalently,

$$
\boxed{
\mathcal O(x)=\frac15\lim_{z\to0}z^{-4}
\left[
\partial_z\phi
-\frac z3\Box_5J
-\frac{z^3}{6}\Box_5^2J
\right]}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 354](../../../../paper-354-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
