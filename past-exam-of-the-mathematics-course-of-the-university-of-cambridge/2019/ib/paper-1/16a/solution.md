<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

Use $\mathbf E=-\nabla\phi$ and [Gauss's law](../../../../../gauss-s-law.md) $\nabla\cdot\mathbf E=\rho/\epsilon_0$. The [divergence theorem](../../../../../divergence-theorem.md) and the decay at infinity give

$$
\int\rho\phi\,dV
=\epsilon_0\int\phi\nabla\cdot\mathbf E\,dV
=\epsilon_0\int\nabla\cdot(\phi\mathbf E)\,dV
-\epsilon_0\int\mathbf E\cdot\nabla\phi\,dV
=\epsilon_0\int|\mathbf E|^2\,dV.
$$

Multiplying by $1/2$ proves that the two expressions for the [electrostatic energy](../../../../../electrostatic-energy.md) agree.

The uniform volume charge density in the thick shell is

$$
\rho_0=\frac{3Q}{4\pi(b^3-a^3)}.
$$

Spherical symmetry and the integral form of Gauss's law give

$$
\boxed{
\mathbf E(r)=
\begin{cases}
0,&0\leq r<a,\\[2mm]
\displaystyle\frac{Q}{4\pi\epsilon_0}
\frac{r^3-a^3}{(b^3-a^3)r^2}\,\widehat{\mathbf r},&a\leq r\leq b,\\[3mm]
\displaystyle\frac{Q}{4\pi\epsilon_0r^2}\,\widehat{\mathbf r},&r>b.
\end{cases}}
$$

Thus $|\mathbf E|$ is zero inside, rises continuously through the charged region, reaches $Q/(4\pi\epsilon_0b^2)$ at $b$, and then decays as $r^{-2}$. Taking $\phi(\infty)=0$ and integrating $E=-d\phi/dr$ gives

$$
\phi(r)=
\begin{cases}
\phi(a),&r<a,\\[1mm]
\displaystyle\frac{Q}{4\pi\epsilon_0}\left[\frac1b+
\frac{(b^2-r^2)/2+a^3(1/b-1/r)}{b^3-a^3}\right],&a\leq r\leq b,\\[3mm]
\displaystyle\frac{Q}{4\pi\epsilon_0r},&r>b.
\end{cases}
$$

The [electric potential](../../../../../electric-potential.md) is continuous, constant inside, decreases smoothly across the charge, and continues as $1/r$ outside.

As $b\to a$, the charge becomes a surface shell. Then

$$
\mathbf E=\begin{cases}0,&r<a,\\ Q\widehat{\mathbf r}/(4\pi\epsilon_0r^2),&r>a,
\end{cases}
\qquad
\phi=\begin{cases}Q/(4\pi\epsilon_0a),&r\leq a,\\ Q/(4\pi\epsilon_0r),&r\geq a.
\end{cases}
$$

The potential remains continuous, but the normal electric field jumps by $Q/(4\pi\epsilon_0a^2)$ across the [surface charge density](../../../../../surface-charge-density.md).

The field-energy expression gives

$$
U=\frac{\epsilon_0}{2}\int_a^\infty
\left(\frac{Q}{4\pi\epsilon_0r^2}\right)^2,4\pi r^2\,dr
=\frac{Q^2}{8\pi\epsilon_0a}
=\frac12Q\phi(a).
$$

The charge-potential expression gives the same result directly because the entire charge lies where the potential equals $\phi(a)$:

$$
U=\frac12\int\rho\phi\,dV=\frac12Q\phi(a).
$$

This is the [electrostatic energy of a uniformly charged spherical shell](../../../../../electrostatic-energy-of-a-uniformly-charged-spherical-shell.md).

Since $\phi(a)=Q/(4\pi\epsilon_0a)$ is proportional to $Q$,

$$
\delta U=\delta\left(\frac{Q^2}{8\pi\epsilon_0a}\right)
=\boxed{\phi(a)\,\delta Q}
$$

to first order. This is the [work](../../../../../work.md) required to bring the additional charge $\delta Q$ from infinity to the potential created by the charge already present.

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
