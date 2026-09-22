<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Every forced propagating mode must have the imposed zonal frequency

$$
\omega=kC.
$$

For $C>0$, only the [equatorial Kelvin wave](../../../../../../equatorial-kelvin-wave.md) has the correct sign. Upward group velocity in the fluid $z>0$ selects

$$
m_K=-\frac NC.
$$

With $K(y)=\exp[-\beta y^2/(2C)]$, its pressure field can be written

$$
\boxed{
\phi_K=\operatorname{Re}
\left\{
a_KK(y)e^{i[k(x-Ct)+m_Kz]}
\right\}}.
$$

Here $v_K=0$, $u_K=\phi_K/C$, and the complex vertical-velocity amplitude is

$$
\hat w_K=-\frac{kCm_K}{N^2}a_KK
=\frac kN a_KK.
$$

The lower boundary is matched only if

$$
\boxed{
W(y)=\frac kN a_K
\exp\left(-\frac{\beta y^2}{2C}\right)}
$$

after choosing the phase of $a_K$ to make the prescribed cosine amplitude real.

For $C<0$, the upward-radiating [equatorial Rossby waves](../../../../../../equatorial-rossby-wave.md) have

$$
\boxed{
m_n=-\frac{N}{(2n+1)C}>0},
\qquad n=1,2,\ldots.
$$

Choose each pair $(\hat v_n,\hat\phi_n)$ as in part c for this $m_n$. The propagating sum is

$$
\boxed{
v=\operatorname{Re}
\sum_{n=1}^{\infty}
a_n\hat v_n(y)
e^{i[k(x-Ct)+m_nz]}},
$$



$$
\boxed{
\phi=\operatorname{Re}
\sum_{n=1}^{\infty}
a_n\hat\phi_n(y)
e^{i[k(x-Ct)+m_nz]}}.
$$

The other fields follow mode by mode from part c and $\hat w_n=-kCm_n\hat\phi_n/N^2$. Thus the boundary matching condition is

$$
\boxed{
W(y)=
\sum_{n=1}^{\infty}
\frac{k\,a_n}{N(2n+1)}
\hat\phi_n(y)}.
$$

For $C>0$, the space of upward-radiating wave profiles is only the one-dimensional Gaussian Kelvin profile, so a generic $W(y)$ cannot be matched by propagating waves. Its Kelvin projection radiates upward; the remaining forcing produces a balanced, vertically evanescent response trapped near the lower boundary. This is the equatorial analogue of the fact that quasi-geostrophic [Rossby waves](../../../../../../rossby-wave.md) have westward rather than eastward phase propagation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
