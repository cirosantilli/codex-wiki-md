<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Model [alpha decay](../../../../alpha-decay.md) as a preformed [alpha particle](../../../../alpha-particle.md) making repeated escape attempts from a short-range nuclear potential well, then undergoing [quantum tunnelling](../../../../quantum-tunnelling.md) through the external [Coulomb potential](../../../../coulomb-potential-energy.md). Write the daughter [atomic number](../../../../atomic-number.md) as $Z_D$, the nuclear radius as $R$, and the relative [reduced mass](../../../../reduced-mass.md) as $\mu$. For zero [orbital angular momentum](../../../../orbital-angular-momentum.md), the [WKB approximation](../../../../wkb-approximation.md) gives

$$
P_{\mathrm{tun}}\simeq e^{-G},\qquad
G=\frac2\hbar\int_R^{r_2}\sqrt{2\mu(V(r)-Q)}\,dr,
\qquad V(r)=\frac{k}{r},\quad
k=\frac{2Z_De^2}{4\pi\epsilon_0},\quad r_2=\frac{k}{Q}.
$$

Set $v=\sqrt{2Q/\mu}$ and $r=r_2\sin^2\theta$. Then

$$
G=\frac{2\sqrt{2\mu Q}\,r_2}{\hbar}
\left[\arccos\sqrt{\frac R{r_2}}-
\sqrt{\frac R{r_2}\left(1-\frac R{r_2}\right)}\right].
$$

When $R/r_2\ll1$, the leading term is

$$
G\simeq\frac{2\pi k}{\hbar v}
=\frac{Z_De^2}{\epsilon_0\hbar v},\qquad
\boxed{\tau\simeq(P_\alpha\nu_{\mathrm{attempt}})^{-1}
\exp\left(\frac{Z_De^2}{\epsilon_0\hbar v}\right).}
$$

Here $P_\alpha$ is the [alpha preformation probability](../../../../alpha-preformation-probability.md) and $\nu_{\mathrm{attempt}}$ the attempt frequency. The stated proportionality retains only the dominant barrier exponent. It assumes a thick classically forbidden barrier, nonrelativistic relative motion, a spherical unscreened external [Coulomb potential](../../../../coulomb-potential-energy.md), and slowly varying prefactors. Finite $R$, changes in [alpha preformation probability](../../../../alpha-preformation-probability.md), and a [centrifugal barrier](../../../../centrifugal-barrier.md) for nonzero [orbital angular momentum](../../../../orbital-angular-momentum.md) produce significant corrections. The precise charge in the barrier is $Z_D=Z_P-2$; using the parent charge is an approximation for large $Z_P$. The measured [alpha particle](../../../../alpha-particle.md) speed approximates $v$ only when daughter recoil is negligible.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the nuclear and particle physics course of the University of Oxford](../../../split.md)
5. [Nuclear and particle physics course of the University of Oxford](../../../../nuclear-and-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
