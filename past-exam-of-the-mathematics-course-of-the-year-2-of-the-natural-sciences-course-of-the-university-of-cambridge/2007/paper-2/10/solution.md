<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

A real two-dimensional [group representation](../../../../group-representation.md) is a [group homomorphism](../../../../group-homomorphism.md) $D:G\to GL(2,\mathbb R)$, so $D(AB)=D(A)D(B)$ and $D(I)=I$.

Substitute $\tilde x=\alpha x+\beta y$ and $\tilde y=\gamma x+\delta y$ into the quadratic expression. Its coefficients of $x^2$ and $y^2$ are $\alpha^2\hat a+\gamma^2\hat b$ and $\beta^2\hat a+\delta^2\hat b$. The cross term is zero for every matrix in this particular [cyclic group](../../../../cyclic-group.md), because each has one nonzero entry per row. Thus

$$
\boxed{M(A)=\begin{pmatrix}\alpha^2&\gamma^2\\\beta^2&\delta^2\end{pmatrix}.}
$$

Let $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ generate the group. For $A=\pm I$, $M=I$; for $A=\pm J$, $M=S:=\begin{pmatrix}0&1\\1&0\end{pmatrix}$. Since $S^2=I$, each $M$ is its own inverse and $D(J^k)=S^k$. The group law is respected: $S^{k+l}=S^kS^l$, and $S^4=I$ makes it independent of the representative modulo four. This proves that $D=M^{-1}$ is a [group representation](../../../../group-representation.md).

This [quarter-turn action on diagonal quadratic forms](../../../../quarter-turn-action-on-diagonal-quadratic-forms.md) has

$$
\boxed{\ker D=\{I,-I\},}
$$

so it is **not faithful**. Quadratic forms cannot distinguish a simultaneous sign reversal of both coordinates. The invariant coefficient directions $(1,1)$ and $(1,-1)$ correspond to the fixed form $x^2+y^2$ and the form $x^2-y^2$ whose sign changes under a quarter-turn.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2007](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
