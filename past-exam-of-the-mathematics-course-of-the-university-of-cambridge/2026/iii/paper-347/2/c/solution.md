<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Insert the self-similar ansatz into the height-integrated equations. Mass conservation is already satisfied because $H\sim c_s/\Omega_K\propto R$ and $\rho RHu_R$ is constant. The angular-momentum and energy equations reduce to

$$
c_1=-\frac32\alpha c_3,
\qquad
c_2^2=\epsilon'c_3,
$$

while radial momentum gives

$$
1=\frac12c_1^2+c_2^2+\frac52c_3.
$$

Define

$$
g(\alpha,\epsilon')=
\sqrt{1+\frac{18\alpha^2}{(5+2\epsilon')^2}}-1.
$$

Solving the quadratic gives the exact [advection-dominated accretion flow](../../../../../../advection-dominated-accretion-flow.md) coefficients

$$
\boxed{c_1=-\frac{5+2\epsilon'}{3\alpha}g},
$$



$$
\boxed{c_2=
\left[\frac{2\epsilon'(5+2\epsilon')}{9\alpha^2}g\right]^{1/2}},
\qquad
\boxed{c_3=\frac{2(5+2\epsilon')}{9\alpha^2}g}.
$$

For $\alpha^2\ll1$,

$$
g=\frac{9\alpha^2}{(5+2\epsilon')^2}+O(\alpha^4),
$$

and therefore

$$
\boxed{c_1\simeq-\frac{3\alpha}{5+2\epsilon'},\quad
c_2^2\simeq\frac{2\epsilon'}{5+2\epsilon'},\quad
c_3\simeq\frac{2}{5+2\epsilon'}}.
$$

Efficient cooling means $f\to0$ and hence $\epsilon'=\epsilon/f\to\infty$ for fixed $\gamma<5/3$. Then

$$
u_R/v_K\to0,
\qquad
\Omega/\Omega_K\to1,
\qquad
c_s^2/v_K^2\to0,
\qquad
H/R\sim c_s/v_K\to0.
$$

The flow is therefore cold, nearly Keplerian, slowly accreting, and geometrically thin: the standard thin-disk limit.

For significant advection, $f=O(1)$ and all three deviations are explicit:

$$
u_R\simeq-\frac{3\alpha}{5+2\epsilon'}v_K,
\quad
\Omega\simeq\sqrt{\frac{2\epsilon'}{5+2\epsilon'}}\,\Omega_K,
\quad
c_s\simeq\sqrt{\frac{2}{5+2\epsilon'}}\,v_K.
$$

The gas is hot and thick, pressure supplies part of the radial support, rotation is sub-Keplerian, and dissipated entropy is carried inward. As $\gamma\to5/3$, $\epsilon'\to0$, so $\Omega\to0$, $c_s^2\to(2/5)v_K^2$, and $u_R\to-(3\alpha/5)v_K$: the self-similar rotating solution approaches a hot Bondi-like inflow. Sagittarius A\* is the standard supermassive example: its luminosity is tiny compared with its [Eddington luminosity](../../../../../../eddington-luminosity.md) despite an available gas supply, and its hot optically thin spectrum and low radiative efficiency are described by an ADAF or the broader radiatively inefficient accretion-flow family.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
