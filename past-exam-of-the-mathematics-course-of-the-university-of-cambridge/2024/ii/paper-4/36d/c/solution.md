<h1 id="36d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since there are no currents, $\nabla\times B=0$ in each constant-permeability region, while $\nabla\cdot B=0$ gives $\nabla^2\psi=0$. The displayed dipole forms are therefore harmonic. Regularity at the origin and the field at infinity give

$$
b_1=0,\qquad a_3=B_0.
$$

For $\psi=(ar+b/r^2)\cos\theta$,

$$
B_r=(a-2b/r^3)\cos\theta,
\qquad
B_\theta=-(a+b/r^3)\sin\theta.
$$

The [magnetic spherical-shell matching](../../../../../../magnetic-spherical-shell-matching.md) conditions, continuity of $B_r$ and $H_\theta$, give the remaining four equations

$$
a_1-\frac{2b_1}{R_1^3}=a_2-\frac{2b_2}{R_1^3},
\qquad
\frac{a_1+b_1/R_1^3}{\mu_0}
=\frac{a_2+b_2/R_1^3}{\mu},
$$



$$
a_2-\frac{2b_2}{R_2^3}=a_3-\frac{2b_3}{R_2^3},
\qquad
\frac{a_2+b_2/R_2^3}{\mu}
=\frac{a_3+b_3/R_2^3}{\mu_0}.
$$

The two $R_1$ equations yield

$$
a_2=\frac{\mu_0+2\mu}{3\mu_0}a_1,
\qquad
b_2=\frac{\mu-\mu_0}{3\mu_0}R_1^3a_1.
$$

Together with $b_1=0$ and $a_3=B_0$, these are the requested expressions. Substituting them into the two $R_2$ equations gives a two-by-two linear system for $a_1$ and $b_3$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [36D](../../36d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
