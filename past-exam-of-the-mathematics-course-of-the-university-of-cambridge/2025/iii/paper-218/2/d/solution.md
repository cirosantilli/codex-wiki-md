<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $z=\widehat\beta_{\mathrm{OLS}}$ and $G=X^TX/n=\begin{pmatrix}1&\rho\\\rho&1\end{pmatrix}$. While both lasso coordinates are positive, the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) give

$$
G(\widehat\beta-z)+\lambda\binom11=0,
\qquad
\widehat\beta=z-\frac{\lambda}{1+\rho}\binom11.
$$

Hence

$$
\lambda^\dagger=(1+\rho)\min(z_1,z_2).
$$

Assume without loss of generality that $z_1\leq z_2$. After the first coordinate vanishes, the second remains active until $lambda=z_2+\rho z_1$. The zero vector satisfies the KKT conditions exactly when $lambda\geq\lVert Gz\rVert_\infty$; for $z_1\leq z_2$ and $-1<\rho<1$, this norm is $z_2+\rho z_1$. Therefore

$$
\lambda^\ddagger=\max(z_1,z_2)+\rho\min(z_1,z_2),
$$

and

$$
\lambda^\ddagger-\lambda^\dagger
=\max(z_1,z_2)-\min(z_1,z_2)=|z_1-z_2|,
$$

which is independent of $\rho$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
