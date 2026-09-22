<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The on-site potential of the [Phi-four lattice model](../../../../../../phi-four-lattice-model.md) is

$$
V(s)=\frac g4s^4+\frac\nu2s^2,
\qquad V''(s)=3gs^2+\nu\geq\nu>0.
$$

In the [random-walk representation of a lattice-field covariance](../../../../../../random-walk-representation-of-a-lattice-field-covariance.md), $\langle\phi_x\phi_y\rangle$ is a Green function for a nearest-neighbour walk with a nonnegative environment-dependent killing rate bounded below by a positive constant depending on $\nu$. Dropping the quartic contribution can only decrease that killing, so

$$
0\leq\langle\phi_x\phi_y\rangle
\leq(-\Delta+\nu)^{-1}(x,y).
$$

The massive lattice Green function has the killed-walk expansion

$$
(-\Delta+\nu)^{-1}(x,y)
=\sum_{k\geq0}\frac1{2d+\nu}
\left(\frac{2d}{2d+\nu}\right)^k
\mathbb P_x(S_k=y),
$$

with normalization adjusted to the chosen Laplacian. Reaching $y$ requires at least $|x-y|_1$ steps, while the geometric survival factor is strictly below one. Summing the tail gives constants $C,c>0$ such that

$$
\boxed{|\langle\phi_x\phi_y\rangle|\leq Ce^{-c|x-y|_1}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
