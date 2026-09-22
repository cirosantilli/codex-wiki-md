<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Embed the two off-diagonal [Pauli matrices](../../../../pauli-matrices.md) in each of the $(u,d)$, $(u,s)$ and $(d,s)$ two-dimensional subspaces. Together with two independent embedded diagonal [Pauli matrices](../../../../pauli-matrices.md), this produces the [Gell-Mann matrices](../../../../gell-mann-matrices.md):

$$
\begin{aligned}
\lambda_1&=\begin{pmatrix}0&1&0\\1&0&0\\0&0&0\end{pmatrix},&
\lambda_2&=\begin{pmatrix}0&-i&0\\i&0&0\\0&0&0\end{pmatrix},&
\lambda_3&=\begin{pmatrix}1&0&0\\0&-1&0\\0&0&0\end{pmatrix},\\
\lambda_4&=\begin{pmatrix}0&0&1\\0&0&0\\1&0&0\end{pmatrix},&
\lambda_5&=\begin{pmatrix}0&0&-i\\0&0&0\\i&0&0\end{pmatrix},&
\lambda_6&=\begin{pmatrix}0&0&0\\0&0&1\\0&1&0\end{pmatrix},\\
\lambda_7&=\begin{pmatrix}0&0&0\\0&0&-i\\0&i&0\end{pmatrix},&
\lambda_8&=\frac1{\sqrt3}\begin{pmatrix}1&0&0\\0&1&0\\0&0&-2\end{pmatrix}.&&
\end{aligned}
$$

To construct the last matrix explicitly, the $(u,s)$ diagonal embedding is $D_{us}=\operatorname{diag}(1,0,-1)$ and the $(d,s)$ embedding is $D_{ds}=\operatorname{diag}(0,1,-1)$. Their difference is $\lambda_3$, and their sum divided by $\sqrt3$ is $\lambda_8$. There are only two independent diagonal generators.

Each matrix is [Hermitian](../../../../hermitian-operator.md) and traceless. Their inner products satisfy $\operatorname{tr}(\lambda_a\lambda_b)=2\delta_{ab}$, proving [linear independence](../../../../linear-independence.md). With $T_a=\lambda_a/2$, arbitrary transformations near the identity have $U=\exp(i\theta_aT_a)$. The eight matrices span the generators; they are not a vector-space basis of group elements themselves.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
