<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $\xi_i\in[t_i,t_{i+k}]$ and choose a knot interval $I=(t_\ell,t_{\ell+1})$ adjacent to it on which $N_i$ is active. Exactly $k$ B-splines are nonzero on $I$, and their polynomial restrictions form a basis of $\mathcal P_{k-1}$. Applying the expansion from part (a) to the polynomial piece $N_j|_I$ gives

$$
N_j(t)=\sum_r\lambda_r(N_j,\xi_i)N_r(t),
\qquad t\in I.
$$

Uniqueness of coordinates in this local basis forces

$$
\lambda_i(N_j,\xi_i)=\delta_{ij}
$$

when $N_j$ is active. If $N_j$ vanishes on $I$, all of its local polynomial derivatives vanish and the same equality holds with value zero. At a knot, use either adjacent polynomial piece; the $x$-independence proved in part (a) gives the same coefficient. Hence

$$
\boxed{\lambda_i(N_j,\xi_i)=\delta_{ij},
\qquad \xi_i\in[t_i,t_{i+k}]},
$$

so the $\lambda_i$ form the [dual basis](../../../../../../dual-basis.md) to the B-spline basis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
