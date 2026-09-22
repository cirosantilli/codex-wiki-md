<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Divide the supplied scheme by $\omega$ and take

$$
M=\frac D\omega+L,\qquad N=\left(\frac1\omega-1\right)D-U.
$$

Then $A=M-N$, and $M$ is invertible because it is lower triangular with positive diagonal $D/\omega$. Symmetry gives $U=L^T$, so

$$
\boxed{W=M+M^T-A=\left(\frac2\omega-1\right)D>0\quad(0<\omega<2).}
$$

The [Householder-John theorem](../../../../../../householder-john-theorem.md) therefore gives convergence.

For a direct spectral proof, let $B=M^{-1}N=I-M^{-1}A$. Expansion verifies $A-B^*AB=(I-B)^*W(I-B)$. If $Bv=\lambda v$ with $v\ne0$, then

$$
(1-|\lambda|^2)v^*Av=|1-\lambda|^2v^*Wv.
$$

The value $\lambda=1$ is impossible since $(I-B)v=M^{-1}Av$ and $A$ is invertible. Both quadratic forms are positive, hence $|\lambda|<1$. The error obeys $e^{(k+1)}=Be^{(k)}$ and tends to zero, proving **convergence to the unique solution $A^{-1}b$ for every initial iterate**. This is the successive-over-relaxation iteration, with no assertion of convergence at the excluded endpoints.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
