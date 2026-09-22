<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The volume flux carried with the particle skeleton is

$$
Q_0=2\pi\int_0^Rw_s(r)r\,dr
=\boxed{\frac{\pi G(R-a)^2(3R^2+2Ra+a^2)}{24\eta}}.
$$

By [Darcy law](../../../../../../../darcy-law.md), the fluid moves relative to the solids at $kG/\eta$. The total mixture-volume flux is therefore

$$
\boxed{Q_T=Q_0+
\frac{2\pi kG}{\eta}
\int_0^R[1-\phi(r)]r\,dr}.
$$

This is explicit because $\phi(r)$ is given above. For example, if

$$
c=\frac{G}{2p_s},
\qquad
T=\sqrt{c(R-a)},
$$

then

$$
\int_0^R\phi r\,dr
=\phi_m\left\{
\frac{a^2}{2}
+\frac{2a}{c}[T-\log(1+T)]
+\frac{2}{c^2}
\left[\frac{T^3}{3}-\frac{T^2}{2}+T-\log(1+T)\right]
\right\}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 352](../../../../paper-352-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
