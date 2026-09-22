<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the two concentration differences $u=C_a-C_b$ and $v=C_b-C_d$. For zero emissions and $R_a=R_b=R$, their [ordinary differential equation](../../../../ordinary-differential-equation.md) is

$$
\frac d{dt}\begin{pmatrix}u\\v\end{pmatrix}
=\begin{pmatrix}-2r/R&s/R\\r/R&-s(1/R+1/R_d)\end{pmatrix}
\begin{pmatrix}u\\v\end{pmatrix}.
$$

Writing the positive decay rates as $\mu_i=1/\tau_i$, their characteristic equation is

$$
\mu^2-P\mu+Q=0,\qquad
P=\frac{2r+s}{R}+\frac s{R_d},\qquad
Q=\frac{rs(R_d+2R)}{R^2R_d}.
$$

Consequently

$$
\boxed{\tau_1=\frac2{P+\sqrt{P^2-4Q}},\qquad
\tau_2=\frac2{P-\sqrt{P^2-4Q}}.}
$$

For $r\gg s$, the first [normal mode](../../../../normal-mode.md) rapidly equalizes the fast reservoirs, giving $\mu_1\simeq2r/R$. The slower evolution treats them as a combined capacity $2R$ exchanging with $R_d$, giving $\mu_2\simeq s[1/(2R)+1/R_d]$. Therefore

$$
\boxed{\tau_1\simeq\frac R{2r},\qquad
\tau_2\simeq\frac{2RR_d}{s(R_d+2R)}\simeq\frac{2R}s\quad(R_d\gg R).}
$$

The timescale ratio is $\tau_2/\tau_1\simeq4r/s\gg1$ in the joint limit. Since the conserved [normal mode](../../../../normal-mode.md) has $\tau_3=\infty$, the hierarchy is $\tau_1\ll\tau_2\ll\tau_3$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
