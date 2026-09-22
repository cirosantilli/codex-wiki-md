<h1 id="14c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [steady-state bifurcation](../../../../../../steady-state-bifurcation.md) is a change in the local equilibrium branches or their stability as a parameter varies. At such a bifurcation the [Jacobian matrix](../../../../../../jacobian-matrix.md) at the equilibrium has a zero [eigenvalue](../../../../../../eigenvalue.md), so the implicit function argument for a unique persistent local equilibrium fails.

For this system,

$$
J=\begin{pmatrix}1-y^2-3x^2&-2xy\\-2xy&\mu-2y-x^2\end{pmatrix}.
$$

At $(0,\mu)$ its eigenvalues are $1-\mu^2,-\mu$; at $(1,0)$ they are $-2,\mu-1$. Both have one simple zero eigenvalue at $\mu=1$, with the other eigenvalue negative. Interior equilibrium branches, obtained below, meet these boundary equilibria there, establishing the actual bifurcations rather than merely a necessary eigenvalue test.

$$
\boxed{\mu=1:\quad\sigma(J_{(0,1)})=\{0,-1\},\quad\sigma(J_{(1,0)})=\{-2,0\}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [14C](../../14c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
