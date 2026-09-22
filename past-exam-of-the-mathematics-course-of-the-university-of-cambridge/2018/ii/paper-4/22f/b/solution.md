<h1 id="22f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fixed-point space $I=\ker(U-I)$ is closed. If $y\in I$ and $w=Ux-x\in W$, then [unitarity](../../../../../../unitary-operator.md) gives

$$
\langle y,w\rangle
=\langle y,Ux\rangle-\langle y,x\rangle
=\langle U^{-1}y,x\rangle-\langle y,x\rangle=0,
$$

so $I\perp W$.

Conversely, $z\in W^\perp$ exactly when

$$
0=\langle z,Ux-x\rangle
=\langle U^*z-z,x\rangle
$$

for every $x\in H$. Thus $U^*z=z$, equivalently $Uz=z$, and $z\in I$. Hence $W^\perp=I$, so the [double orthogonal complement](../../../../../../double-orthogonal-complement.md) identity gives

$$
\overline W=(W^\perp)^\perp=I^\perp.
$$

The [orthogonal decomposition by a closed subspace](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) now yields

$$
\boxed{H=I\oplus\overline W}.
$$

Define the [Cesaro average](../../../../../../cesaro-mean.md)

$$
A_n=\frac1n\sum_{i=0}^{n-1}U^i.
$$

For $y\in I$, $A_ny=y$. For a generator $w=Uz-z$ of $W$, the sum telescopes:

$$
A_nw=\frac{U^nz-z}{n},
\qquad
\|A_nw\|\leq\frac{2\|z\|}{n}\longrightarrow0.
$$

Moreover $\|A_n\|\leq1$, so approximation extends this convergence from $W$ to $\overline W$. Writing $x=Px+(I-P)x$ according to the orthogonal decomposition gives the [Von Neumann mean ergodic theorem](../../../../../../von-neumann-mean-ergodic-theorem.md)

$$
\boxed{\lim_{n\to\infty}\frac1n\sum_{i=0}^{n-1}U^ix=Px}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22F](../../22f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
