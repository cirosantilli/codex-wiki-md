<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write

$$
D=1+\psi_r^2+\psi_z^2.
$$

Differentiating the prescribed identity $u(\psi(r,z),r,z)=0$ in its two [tangential directions](../../../../../../tangent-vector.md) gives

$$
u_r=-\psi_ru_t,
\qquad
u_z=-\psi_zu_t.
$$

The [unit normal](../../../../../../unit-normal.md) is $(1,-\psi_r,-\psi_z)/\sqrt D$, so the second item of [Cauchy data](../../../../../../cauchy-data.md) becomes

$$
g=\partial_Nu
=\frac{u_t-\psi_ru_r-\psi_zu_z}{\sqrt D}
=\sqrt D\,u_t.
$$

Consequently

$$
u_t=\frac g{\sqrt D},
\qquad
u_r=-\frac{\psi_rg}{\sqrt D},
\qquad
u_z=-\frac{\psi_zg}{\sqrt D}.
$$

Substitution into the [principal symbol](../../../../../../principal-symbol-of-a-partial-differential-equation.md) from part a shows that the graph is [non-characteristic](../../../../../../non-characteristic-hypersurface.md) exactly where

$$
\boxed{1-(1-\frac{\psi_zg}{\sqrt{1+\psi_r^2+\psi_z^2}})^2
(\psi_r^2+\psi_z^2)\ne0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
