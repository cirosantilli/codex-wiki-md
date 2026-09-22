<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The rotation introduces [angular frequency](../../../../../../angular-frequency.md) $\Omega$ and, after combining the two blades, harmonics such as $2\Omega$. The [acoustic compact-source approximation](../../../../../../acoustic-compact-source-approximation.md) requires the propagation time $a/c_0$ to be small compared with $\Omega^{-1}$. Thus

$$
\boxed{\mu=\Omega a/c_0\ll1.}
$$

It also bounds every blade element's [Mach number](../../../../../../mach-number.md) by $\mu$. Consequently $|1-M_r|=1+O(\mu)$, and its leading value is one. The separate [acoustic far field](../../../../../../acoustic-far-field.md) condition is $\Omega R/c_0\gg1$.

Choose the positive rotation sense so that a first blade at phase $\alpha$ has radial and tangential unit vectors

$$
e_r(\alpha)=\cos\alpha\,e_y+\sin\alpha\,e_z,\qquad
e_\phi(\alpha)=-\sin\alpha\,e_y+\cos\alpha\,e_z.
$$

Integrating the given line [force](../../../../../../force.md) from $r=0$ to $a$ yields $\mathcal F_1=F e_\phi(\Omega\tau)+D e_x$. Its axial component is constant, while $\dot{\mathcal F}_1=-F\Omega e_r$. Since $n=\cos\theta e_x+\sin\theta e_y$, the compact [acoustic dipole](../../../../../../acoustic-dipole.md) sound from this blade is

$$
\boxed{\rho'_1=-\frac{F\Omega\sin\theta}{4\pi c_0^3R}\cos\big(\Omega(t-R/c_0)\big).}
$$

The other blade has phase $\alpha+\pi$ and contributes the opposite rotating [force](../../../../../../force.md). At a common compact [retarded time](../../../../../../retarded-time.md), their total [force](../../../../../../force.md) is $2D e_x$, so

$$
\boxed{\rho'_{\text{two blades}}=0\quad\text{at leading compact dipole order}.}
$$

This cancellation calls for the next source-delay correction; it does not mean that the complete moving-source field vanishes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
