<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $s=\tilde z$ and use full positive coefficients, $\tilde Q=A s^\theta$, $\tilde M=D s^\mu$, $\tilde B=C s^\psi$. Comparing exponents in the three plume equations gives

$$
\theta-1=\mu/2,\qquad \mu-1=\psi+\theta-\mu,\qquad
\psi-1=\theta+\beta.
$$

Solving these equations yields

$$
\boxed{\theta=3+\beta/2,\qquad\mu=4+\beta,\qquad\psi=4+3\beta/2.}
$$

The coefficient equations are $\theta A=\sqrt D$, $\mu D=CA/D$ and $\psi C=-\lambda^\beta A$. Thus

$$
\boxed{c_\theta=A=\frac{\lambda^{\beta/2}}{\theta^2\sqrt{-\mu\psi}},\quad
c_\mu=D=-\frac{\lambda^\beta}{\mu\psi\theta^2},\quad
c_\psi=C=-\frac{\lambda^\beta A}{\psi}=\mu\theta^4A^3.}
$$

For a rising plume with $Q,M,B>0$, the first equation requires $\theta>0$, the momentum equation $\mu>0$, and the decreasing-buoyancy equation $\psi<0$. Together these require

$$
\boxed{-4<\beta<-8/3.}
$$

They are the physical [plume similarity in power-law stratification](../../../../../../plume-similarity-in-power-law-stratification.md) branches, not positive-plume solutions for arbitrary powers. The endpoint coefficients are singular; the endpoints cannot be included by simply substituting into these formulas. At the prescribed positive source coordinate $s_s=1/\lambda$, the matched source buoyancy is

$$
\tilde B_s=C\lambda^{-\psi}
=\frac{\mu}{\theta^2(-\mu\psi)^{3/2}}\lambda^{-4},
$$

finite and positive for every finite $\lambda>0$ in the open range. In contrast, the same branch has divergent buoyancy at the mathematical origin $s=0$. A source at positive height makes the branch physically usable. Merely saying a power is finite at a nonzero coordinate would not itself determine this range; positivity and the plume balances are essential.

At large $s$, $Q$ and $M$ increase without bound, $B$ decreases to zero, radius $Q/\sqrt{\pi M}$ grows proportionally to height, and mean upward [velocity](../../../../../../velocity.md) $M/Q\propto s^{1+\beta/2}$ decreases but remains positive. The integrated buoyancy loss is finite because $\theta+\beta=\psi-1<-1$. The weakening ambient stratification never makes this matched plume negatively buoyant at a finite height; its upward momentum continues to grow even while its speed decreases through [entrainment](../../../../../../fluid-entrainment.md). Consequently its maximum rise height is infinite in this ideal model. This particular exact branch requires its three source fluxes to match the displayed coefficients; it is not a proof that every source in the same ambient escapes.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
