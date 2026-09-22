<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

Represent the [Riemann sphere](../../../../../riemann-sphere.md) by the complex [projective line](../../../../../projective-line.md), with finite $z$ represented by $[z:1]$ and infinity by $[1:0]$. An invertible [matrix](../../../../../matrix.md) $A=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$ acts by $[u:v]\mapsto[au+bv:cu+dv]$, giving the stated fractional map on finite points. Applying $B$ and then $A$ is exactly [matrix multiplication](../../../../../matrix-multiplication.md) $AB$, including at poles and infinity. Therefore

$$
\theta(AB)=\theta(A)\circ\theta(B),
$$

so $\theta$ is a [group homomorphism](../../../../../group-homomorphism.md) from the [special linear group](../../../../../special-linear-group.md) to the [Möbius group](../../../../../mobius-group.md).

Every [Möbius transformation](../../../../../mobius-transformation.md) has an invertible complex [matrix](../../../../../matrix.md) representative $A$. Choose $\rho\in\mathbb C$ with $\rho^2\det A=1$. Such a nonzero [square root](../../../../../square-root.md) exists in $\mathbb C$, and $\rho A$ has [determinant](../../../../../determinant.md) one while representing the same projective map. This proves surjectivity. If the map is the identity, fixing zero and infinity forces $b=c=0$, and fixing one forces $a=d$. The determinant-one condition gives $a^2=1$. Conversely both [scalar matrices](../../../../../scalar-matrix.md) $I$ and $-I$ act trivially. Hence

$$
\boxed{\ker\theta=\{I,-I\},\qquad
\mathcal M\cong SL_2(\mathbb C)/\{I,-I\}.}
$$

For the normal forms, use the fact that a complex $2\times2$ [matrix](../../../../../matrix.md) has a [Jordan normal form](../../../../../jordan-normal-form.md): either it is diagonalizable or it has one nontrivial [Jordan block](../../../../../jordan-block.md). For a determinant-one representative, distinct [eigenvalues](../../../../../eigenvalue.md) are $\lambda,\lambda^{-1}$. Diagonalizing gives $\operatorname{diag}(\lambda,\lambda^{-1})$, whose projective action is $z\mapsto\lambda^2z$. Distinctness means $\lambda^2\ne1$, so $\mu=\lambda^2$ is neither zero nor one.

If the [eigenvalue](../../../../../eigenvalue.md) is repeated, the [determinant](../../../../../determinant.md) condition gives $\lambda=\pm1$. A diagonalizable representative would be $\lambda I$ and would give the identity, excluded here. A nontrivial [Jordan block](../../../../../jordan-block.md) is similar to $\left(\begin{smallmatrix}\lambda&1\\0&\lambda\end{smallmatrix}\right)$, giving $z\mapsto z+1/\lambda=z\pm1$. Any invertible conjugating [matrix](../../../../../matrix.md) gives a [Möbius transformation](../../../../../mobius-transformation.md); rescaling it to [determinant](../../../../../determinant.md) one does not change that map. Thus these [matrix similarities](../../../../../matrix-similarity.md) are genuine conjugacies in the [Möbius group](../../../../../mobius-group.md), proving the requested [Möbius conjugacy normal forms](../../../../../mobius-conjugacy-normal-forms.md).

Conjugacy preserves [fixed points](../../../../../fixed-point.md) bijectively. A nonidentity scaling has exactly the two [fixed points](../../../../../fixed-point.md) zero and infinity, while either translation has exactly one, infinity. The identity fixes every point. This proves all three possibilities and excludes any further finite number of [fixed points](../../../../../fixed-point.md).

Finally, suppose $P\circ T\circ P^{-1}=S$, with $S(z)=z+\varepsilon$ and $\varepsilon=\pm1$. Then $S^n(z)=z+n\varepsilon\to\infty$ for every finite $z$ in the topology of the [Riemann sphere](../../../../../riemann-sphere.md); infinity remains infinity. Since $P^{-1}$ is continuous on that [sphere](../../../../../sphere.md),

$$
\boxed{T^n(z)=P^{-1}\bigl(S^n(P(z))\bigr)\longrightarrow
P^{-1}(\infty)=z_0\quad\text{for every }z.}
$$

This is [iteration of a one-fixed-point Möbius transformation](../../../../../iteration-of-a-one-fixed-point-mobius-transformation.md). The limiting statement includes the unique [fixed point](../../../../../fixed-point.md) itself and uses spherical convergence, which also handles intermediate iterates equal to infinity.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
