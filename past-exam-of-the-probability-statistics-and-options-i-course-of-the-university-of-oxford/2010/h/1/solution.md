<h1 id="h/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For [small oscillations](../../../../small-oscillation.md) about equilibrium, put $M_{ij}=T_{ij}(0)$ and $K_{ij}=\partial_i\partial_jV(0)$. The potential has no linear term at equilibrium; to quadratic order the [Lagrangian](../../../../lagrangian.md) is $L_2=\dot x^{\mathsf T}M\dot x/2-x^{\mathsf T}Kx/2$. Its equations are $M\ddot x+Kx=0$. A [normal mode](../../../../normal-mode.md) $x=v e^{i\omega t}$ satisfies the generalized [eigenvalue problem](../../../../eigenvalue-problem.md) $(K-\omega^2M)v=0$. For a positive-definite mass [matrix](../../../../matrix.md), [diagonalization](../../../../diagonalization-of-a-matrix.md) $M^{-1/2}KM^{-1/2}$ gives the squared frequencies and independent normal coordinates. A strictly positive Hessian gives positive frequencies; zero [eigenvalues](../../../../eigenvalue.md) require separate higher-order stability analysis.

Here the spring extensions are $x_1$, $x_2-x_1$, and $-x_2$. Thus

$$
\boxed{T=\tfrac m2(\dot x_1^2+\dot x_2^2),\qquad
V=\tfrac k2[x_1^2+(x_2-x_1)^2+x_2^2].}
$$

The stiffness [matrix](../../../../matrix.md) is $k\left(\begin{smallmatrix}2&-1\\-1&2\end{smallmatrix}\right)$ and $M=mI$. Its eigenvectors $(1,1)$ and $(1,-1)$ have stiffness [eigenvalues](../../../../eigenvalue.md) $k$ and $3k$, giving

$$
\boxed{\omega_1=\sqrt{k/m},\quad v_1=(1,1);\qquad
\omega_2=\sqrt{3k/m},\quad v_2=(1,-1).}
$$

In the first mode the masses move together with equal displacements and the middle spring keeps its length. In the second they move oppositely with equal amplitudes, stretching and compressing the middle spring twice as much as either end spring.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [H](../../h.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
