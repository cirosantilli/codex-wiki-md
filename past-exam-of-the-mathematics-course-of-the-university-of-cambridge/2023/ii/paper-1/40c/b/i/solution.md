<h1 id="40c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [acoustic velocity potential](../../../../../../../acoustic-velocity-potential.md) convention

$$
\mathbf u=\nabla\phi,
\qquad
p'=-\rho_0\phi_t.
$$

For a spherically symmetric outgoing wave with time dependence $e^{i\omega t}$ and $k=\omega/c_0$, write

$$
\widehat\phi(r)=C\frac{e^{-ik(r-a)}}r.
$$

Linearizing the boundary condition at the mean surface $r=a$ gives

$$
\widehat\phi'(a)=i\omega\epsilon.
$$

Since

$$
\widehat\phi'(a)=-\frac{C}{a^2}(1+ika),
$$

we find

$$
C=-\frac{i\omega\epsilon a^2}{1+ika}.
$$

Thus the [outgoing acoustic field of a pulsating sphere](../../../../../../../outgoing-acoustic-field-of-a-pulsating-sphere.md) is

$$
\boxed{
\phi(r,t)
=\operatorname{Re}\left[
-\frac{i\omega\epsilon a^2}{1+i\omega a/c_0}
\frac{e^{i\omega t-i(\omega/c_0)(r-a)}}r
\right]
}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [40C](../../../40c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
