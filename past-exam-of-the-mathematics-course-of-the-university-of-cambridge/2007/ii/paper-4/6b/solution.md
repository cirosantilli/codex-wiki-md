<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The terms $u$ and $\alpha v$ represent intrinsic exponential population growth. The losses $-uv$ and $-\alpha uv$ describe competition between the species; $-\epsilon_1u^2$ and $-\alpha\epsilon_2v^2$ describe crowding within each species. The positive constant $\alpha$ sets the relative time scale of the second population.

The four [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) in the nonnegative quadrant are

$$
(0,0),\quad (1/\epsilon_1,0),\quad(0,1/\epsilon_2),\quad
(u_*,v_*)=\left(\frac{1-\epsilon_2}{1-\epsilon_1\epsilon_2},
\frac{1-\epsilon_1}{1-\epsilon_1\epsilon_2}\right).
$$

The last follows by solving $\epsilon_1u+v=1$ and $u+\epsilon_2v=1$ and is strictly positive under the assumptions. The [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J=\begin{pmatrix}1-v-2\epsilon_1u&-u\\-\alpha v&\alpha(1-u-2\epsilon_2v)\end{pmatrix}.
$$

At the origin its [eigenvalues](../../../../../eigenvalue.md) are $1,\alpha>0$, so it is unstable. At the first single-species equilibrium they are $-1$ and $\alpha(1-1/\epsilon_1)<0$; at the second they are $1-1/\epsilon_2<0$ and $-\alpha$. Both are asymptotically stable. At coexistence,

$$
J_* =\begin{pmatrix}-\epsilon_1u_*&-u_*\\-\alpha v_*&-\alpha\epsilon_2v_*\end{pmatrix},
\qquad \det J_* =\alpha u_*v_*(\epsilon_1\epsilon_2-1)<0.
$$

Thus **coexistence is a saddle; either species-only equilibrium is stable, and extinction is unstable**. The saddle's stable manifold separates the competing basins of attraction.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
