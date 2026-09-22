<h1 id="14d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The function $U(s)=V_0e^{-2s}$ is strictly [convex](../../../../../../convex-function.md). Subject to $\alpha+\beta+\gamma=2\pi$, the [Jensen inequality](../../../../../../jensen-s-inequality.md) gives

$$
U(\alpha)+U(\beta)+U(\gamma)
\geq3U\left(\frac{\alpha+\beta+\gamma}{3}\right),
$$

with equality only at

$$
\boxed{\alpha=\beta=\gamma=\frac{2\pi}{3}}.
$$

This is the minimum of the relative potential, so it is a [stable relative equilibrium](../../../../../../stable-equilibrium-in-lagrangian-mechanics.md).

Let $q_j=q_j^{(0)}+x_j$ near an equally spaced configuration, and put

$$
A=V_0e^{-4\pi/3}.
$$

The gap perturbations are

$$
\delta\alpha=x_2-x_1,\qquad
\delta\beta=x_3-x_2,\qquad
\delta\gamma=x_1-x_3,
$$

whose sum vanishes. A [Taylor expansion](../../../../../../taylor-series.md) gives the quadratic energies

$$
T_2=\frac{mr^2}{2}\sum_j\dot x_j^2,
\qquad
V_2=2A\left[
(x_2-x_1)^2+(x_3-x_2)^2+(x_1-x_3)^2
\right].
$$

Thus the linearized equations are

$$
mr^2\ddot x_i+4A(2x_i-x_j-x_k)=0,
\qquad \{i,j,k\}=\{1,2,3\}.
$$

The matrix in parentheses is the [Graph Laplacian](../../../../../../laplacian-matrix.md) of $K_3$. Its constant eigenvector has eigenvalue zero, while every vector whose components sum to zero has eigenvalue three. One orthonormal set of three [normal modes](../../../../../../normal-mode.md) and their [angular frequencies](../../../../../../angular-frequency.md) is therefore

$$
\begin{array}{c|c}
\text{mode}&\omega\\ \hline
\displaystyle \frac1{\sqrt3}(1,1,1)&0\\[2mm]
\displaystyle \frac1{\sqrt2}(1,-1,0)&
\displaystyle\sqrt{\frac{12V_0e^{-4\pi/3}}{mr^2}}\\[3mm]
\displaystyle \frac1{\sqrt6}(1,1,-2)&
\displaystyle\sqrt{\frac{12V_0e^{-4\pi/3}}{mr^2}}
\end{array}
$$

The zero mode is rigid rotation. The positive and equal squared frequencies on the two-dimensional relative subspace prove stability and agree with the general [normal modes of three equal masses with a symmetric gap potential](../../../../../../normal-modes-of-three-equal-masses-with-a-symmetric-gap-potential.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14D](../../14d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
