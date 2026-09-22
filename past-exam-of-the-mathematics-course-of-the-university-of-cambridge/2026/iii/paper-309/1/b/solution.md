<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\mathcal L_XY=[X,Y]$. Expanding the definition on $fZ$ gives terms proportional to derivatives of $f$ with coefficient

$$
X(Yf)-[X,Y]f-Y(Xf)=0.
$$

All remaining terms carry an overall factor $f$, so

$$
(\mathcal L_X\nabla)_Y(fZ)=f(\mathcal L_X\nabla)_YZ.
$$

The same argument gives linearity in $Y$, confirming that the [Lie derivative of an affine connection](../../../../../../lie-derivative-of-an-affine-connection.md) is tensorial.

Using the torsion-free identities $[X,Y]=\nabla_XY-\nabla_YX$ and $[X,Z]=\nabla_XZ-\nabla_ZX$, expand

$$
\begin{aligned}
(\mathcal L_X\nabla)_YZ
={}&[X,\nabla_YZ]-\nabla_{[X,Y]}Z-\nabla_Y[X,Z]\\
={}&R(X,Y)Z+\nabla_Y(\nabla_ZX)-\nabla_{\nabla_YZ}X.
\end{aligned}
$$

This is the required formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
