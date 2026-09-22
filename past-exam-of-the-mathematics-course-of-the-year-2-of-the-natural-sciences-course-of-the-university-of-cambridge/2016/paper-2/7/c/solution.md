<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the constraint from part (b). For equal masses and spring constants, the [generalized eigenvalue problem for small oscillations](../../../../../generalized-eigenvalue-problem-for-small-oscillations.md) reduces to

$$
\frac km\begin{pmatrix}2&0&0\\0&2&-1\\0&-1&1\end{pmatrix}v=\omega^2v.
$$

The horizontal coordinate decouples, giving

$$
\boxed{\omega_x=\sqrt{\frac{2k}{m}},\qquad v_x=(1,0,0)^T.}
$$

In this [normal mode](../../../../../normal-mode.md), mass 1 oscillates horizontally, mass 2 has its horizontal coordinate fixed, and neither mass has a vertical displacement.

For the vertical block, write $\lambda=m\omega^2/k$. Its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $(2-\lambda)(1-\lambda)-1=\lambda^2-3\lambda+1$. Thus $\lambda_\pm=(3\pm\sqrt5)/2$, and the first vertical equation gives $y_2/y_1=2-\lambda_\pm$. If $\varphi=(1+\sqrt5)/2$ is the [golden ratio](../../../../../golden-ratio.md), the two vertical modes are

$$
\boxed{\begin{aligned}
\omega_-&=\sqrt{\frac{k}{m}\frac{3-\sqrt5}{2}}=\frac1\varphi\sqrt{\frac km},&v_-&=(0,1,\varphi)^T,\\
\omega_+&=\sqrt{\frac{k}{m}\frac{3+\sqrt5}{2}}=\varphi\sqrt{\frac km},&v_+&=(0,1,-1/\varphi)^T.
\end{aligned}}
$$

In the lower-frequency mode, the masses move vertically in phase, with the lower mass having the larger amplitude. In the higher-frequency mode they move oppositely, with lower-to-upper amplitude ratio $1/\varphi$. Their [Euclidean inner product](../../../../../dot-product.md) is zero because $1+\varphi(-1/\varphi)=0$; since $M=mI$, this is also [mass-matrix orthogonality of normal modes](../../../../../mass-matrix-orthogonality-of-normal-modes.md).

The three frequencies satisfy $\omega_-<\omega_x<\omega_+$. Each mode has a scalar coordinate $A\cos\omega t+B\sin\omega t$, and their superposition gives the general constrained motion. No zero-frequency mode remains because the first spring anchors the system. Gravity fixes the equilibrium extensions but drops out of these frequencies for zero-natural-length springs.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
