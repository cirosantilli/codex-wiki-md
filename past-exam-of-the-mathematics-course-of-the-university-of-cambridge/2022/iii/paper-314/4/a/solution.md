<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the material forms of the [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) and momentum equation:

$$
\frac{D\mathbf B}{Dt}
=(\mathbf B\mathbin\cdot\nabla)\mathbf u
-\mathbf B\nabla\mathbin\cdot\mathbf u,
$$



$$
\frac{D\mathbf u}{Dt}
=-\nabla(h+\Phi)+T\nabla s
+\frac{(\nabla\times\mathbf B)\times\mathbf B}{4\pi\rho}.
$$

The magnetic force is perpendicular to $\mathbf B$. For $h_c=\mathbf u\cdot\mathbf B$, the two equations therefore give

$$
\frac{Dh_c}{Dt}
=-\mathbf B\mathbin\cdot\nabla
\left(h+\Phi-\frac{u^2}{2}\right)
+T\mathbf B\mathbin\cdot\nabla s
-h_c\nabla\mathbin\cdot\mathbf u.
$$

Since $\nabla\cdot\mathbf B=0$, this is the [cross-helicity conservation law](../../../../../../cross-helicity-conservation-law.md)

$$
\boxed{
\frac{\partial h_c}{\partial t}+\nabla\mathbin\cdot\mathbf F_c=S_c},
$$

with

$$
\boxed{
\mathbf F_c=\mathbf u h_c
+\mathbf B\left(h+\Phi-\frac{u^2}{2}\right),
\qquad
S_c=T\mathbf B\mathbin\cdot\nabla s}.
$$

For a [homentropic flow](../../../../../../homentropic-flow.md), $\nabla s=0$, so the source vanishes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
