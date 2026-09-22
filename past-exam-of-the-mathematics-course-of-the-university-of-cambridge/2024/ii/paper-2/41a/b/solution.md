<h1 id="41a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write

$$
w'=\sum_l i\pi l\,\widehat w_l e^{i\pi lx},
\qquad
u_x=\sum_m i\pi m\,\widehat u_m e^{i\pi mx}.
$$

Projecting the equation onto modes $|n|\leq D$ gives the [Fourier-Galerkin matrix for a drift-diffusion equation](../../../../../../fourier-galerkin-matrix-for-a-drift-diffusion-equation.md)

$$
\boxed{\dot{\widehat u}_n
=\sum_{|m|\leq D}B_{nm}\widehat u_m,\qquad
B_{nm}=-\pi^2n^2\delta_{nm}
+\pi^2(n-m)m\,\widehat w_{n-m},}
$$

where $\widehat w_l=0$ for $|l|>d$.

For $w=\cos\pi x$, only  
$\widehat w_{\pm1}=1/2$ are nonzero. Hence

$$
B_{nm}=-\pi^2n^2\delta_{nm}
+\frac{\pi^2}{2}(n-m)m\,\mathbf1_{\{|n-m|=1\}}.
$$

The column belonging to the constant mode $m=0$ is zero, so

$$
\boxed{B\text{ is not invertible}}.
$$

Remove that zero mode. In every remaining row $n$, the sum of the magnitudes of the off-diagonal entries is at most $\pi^2|n|$; for $|n|=1$, the would-be coupling to the removed zero mode vanishes. The diagonal entry is $-\pi^2n^2$. Gershgorin's theorem therefore places every [eigenvalue](../../../../../../eigenvalue.md) of the nonconstant block in

$$
\operatorname{Re}z\leq-\pi^2(n^2-|n|)\leq0.
$$

Together with the zero [eigenvalue](../../../../../../eigenvalue.md), all [eigenvalues](../../../../../../eigenvalue.md) of $B$ have nonpositive real part.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [41A](../../41a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
