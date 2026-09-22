<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A rotation by $\pi$ about the vertical symmetry axis maps a horizontal angular velocity $\boldsymbol\Omega'$ to $-\boldsymbol\Omega'$ but leaves a possible vertical force unchanged. Linearity and uniqueness of [Stokes flow](../../../../../../stokes-flow-split.md) therefore require that vertical force to equal its own negative, so it vanishes. A horizontal force and a horizontal couple are allowed by the same symmetry.

Write $\lambda=1-\epsilon$ and examine the lower pole, where $\theta\ll1$. Since $\cos\theta=1-\theta^2/2+O(\theta^4)$,

$$
h=\Delta\left[\epsilon+\frac{\theta^2}{2}
+O(\epsilon\theta^2+\theta^4)\right].
$$

Thus $h=O(\epsilon\Delta)$ for $\theta=O(\epsilon^{1/2})$, a circular patch of radius

$$
\boxed{\ell=O(a\epsilon^{1/2})}.
$$

In the broad region, the surface speed is $O(\Omega'a)$, the shear is $O(\mu\Omega'a/\Delta)$, the area is $O(a^2)$, and the moment arm is $O(a)$. Hence

$$
G'_{\rm broad}=O\left(\frac{\mu\Omega'a^4}{\Delta}\right).
$$

In the narrow patch, the shear rises to $O(\mu\Omega'a/(\epsilon\Delta))$, while its area falls to $O(\epsilon a^2)$; the moment arm remains $O(a)$. Therefore

$$
\boxed{G'_{\rm patch}=G'_{\rm broad}
=O\left(\frac{\mu\Omega'a^4}{\Delta}\right)}.
$$

Dropping the moment arm gives the shear-force scale. Pressure produces the same horizontal order after multiplication by the small surface slope. Both regions consequently contribute

$$
\boxed{F'_{\rm patch}=F'_{\rm broad}
=O\left(\frac{\mu\Omega'a^3}{\Delta}\right)}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
