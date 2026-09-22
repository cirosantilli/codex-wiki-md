<h1 id="14c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At an interior [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md), $x^2=1-y^2=\mu-y$, so

$$
y^2-y+\mu-1=0,\qquad \boxed{y_\pm=\frac{1\pm\sqrt{5-4\mu}}2,\quad x_\pm=\sqrt{1-y_\pm^2}.}
$$

For $1<\mu<5/4$ both values satisfy $0<y<1$, giving two physical equilibria. At such an equilibrium,

$$
J=\begin{pmatrix}-2x^2&-2xy\\-2xy&-y\end{pmatrix},\quad \operatorname{tr}J=-2x^2-y<0,\quad \det J=2x^2y(1-2y).
$$

The branch $y_-<1/2$ is [asymptotically stable](../../../../../../asymptotic-stability.md) by the [trace-determinant stability criterion](../../../../../../trace-determinant-stability-criterion.md); $y_+>1/2$ is a [saddle equilibrium](../../../../../../saddle-equilibrium.md). In fact $J$ is symmetric, so the stable branch has two negative real eigenvalues.

At $\mu=5/4$ the equilibria merge at $(x,y)=(\sqrt3/2,1/2)$. Writing $y=1/2+s$, the equilibrium condition is $s^2+\mu-5/4=0$, the characteristic branch geometry of a [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md). The stable node and saddle annihilate as $\mu$ increases through $5/4$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
