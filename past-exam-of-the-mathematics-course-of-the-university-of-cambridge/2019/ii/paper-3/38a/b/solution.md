<h1 id="38a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the axisymmetric streamfunction convention

$$
w=\frac1r\frac{\partial\psi}{\partial r},
\qquad
u=-\frac1r\frac{\partial\psi}{\partial z}.
$$

For the [similarity solution](../../../../../../similarity-solution.md) $\psi=\nu z g(\eta)$, $\eta=r/z$, regularity on the axis requires $g(0)=g'(0)=0$, while matching to still ambient fluid requires $g'(\eta)/\eta\to0$ as $\eta\to\infty$. The given equation has the first integral

$$
\eta g'-2g+\frac12g^2=C.
$$

The axis conditions give $C=0$, and separation yields

$$
\frac{dg}{g(4-g)}=\frac{d\eta}{2\eta},
\qquad
g(\eta)=\frac{4a\eta^2}{1+a\eta^2}
$$

for some $a>0$.

The axial velocity is

$$
w=\frac{\nu}{\eta z}g'(\eta)
=\frac{8\nu a}{z(1+a\eta^2)^2}.
$$

Normalizing by the conserved momentum flux gives

$$
M=\int_0^\infty rw^2\,dr
=64\nu^2a^2\int_0^\infty\frac{\eta\,d\eta}{(1+a\eta^2)^4}
=\frac{32}{3}\nu^2a,
$$

so $a=3M/(32\nu^2)$. The [similarity solution for a laminar round jet](../../../../../../similarity-solution-for-a-laminar-round-jet.md) is therefore

$$
\boxed{g(\eta)=\frac{12M\eta^2}{32\nu^2+3M\eta^2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38A](../../38a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
