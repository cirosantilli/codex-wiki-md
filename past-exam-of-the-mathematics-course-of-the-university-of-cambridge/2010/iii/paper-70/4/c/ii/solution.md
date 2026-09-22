<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\alpha>0$, minimize $J_\alpha(x)=\|Ax-y\|^2+\alpha\|x\|^2$. Its first variation in every direction gives

$$
(A^*A+\alpha I)x_\alpha=A^*y.
$$

The [self-adjoint operator](../../../../../../../self-adjoint-operator.md) on the left has lower bound $\alpha I$, so it is invertible and the minimizer is unique. The regularized solution has the singular expansion

$$
\boxed{x_\alpha=\sum_j\frac{\sigma_j}{\sigma_j^2+\alpha}(y,v_j)u_j.}
$$

Since $\sigma^2+\alpha\ge2\sigma\sqrt\alpha$, its gain is at most $1/(2\sqrt\alpha)$. Consequently

$$
\boxed{\|x_\alpha(y^\delta)-x_\alpha(y)\|\le\frac{\|y^\delta-y\|}{2\sqrt\alpha}.}
$$

This proves existence, uniqueness and continuous data dependence at fixed positive parameter. For the particular perturbation from part (i), the error is $\delta\sigma_j/(\sigma_j^2+\alpha)$ instead of $\delta/\sigma_j$. To recover a minimum-norm exact solution as noise tends to zero, choose $\alpha\to0$ while $\delta/\sqrt\alpha\to0$; [dominated convergence](../../../../../../../dominated-convergence-theorem.md) of the exact-data singular coefficients removes the bias.

To connect this with the provided inverse expansion, put $B=AA^*$ and $C=A^*A$. The exact intertwining identity is

$$
(A^*A+\alpha I)^{-1}A^*=A^*(\alpha I+AA^*)^{-1}.
$$

It follows by multiplying $(C+\alpha I)A^*=A^*(B+\alpha I)$ on either side by the appropriate [resolvent](../../../../../../../resolvent-of-an-operator.md). A useful exact inverse identity is

$$
(\alpha I+B)^{-1}=\alpha^{-1}I-\alpha^{-2}A(I+\alpha^{-1}C)^{-1}A^*.
$$

Expanding $(I+\alpha^{-1}C)^{-1}$ to two terms gives the printed approximation, namely

$$
R_{\alpha,2}=\alpha^{-1}I-\alpha^{-2}B+\alpha^{-3}B^2.
$$

This is the [truncated Tikhonov resolvent](../../../../../../../truncated-tikhonov-resolvent.md). Multiplication gives $(\alpha I+B)R_{\alpha,2}=I+\alpha^{-3}B^3$, so the expression is not an exact inverse. For example $A=1$ and $\alpha=1$ give the approximate value $1$ instead of the exact $1/2$. Its exact remainder is

$$
R_{\alpha,2}-(\alpha I+B)^{-1}=\alpha^{-3}B^3(\alpha I+B)^{-1},\qquad
\|R_{\alpha,2}-(\alpha I+B)^{-1}\|\le\frac{\|B\|^3}{\alpha^4}.
$$

In the regime $\|C\|/\alpha<1$ it is a controlled Neumann expansion. Using it to reconstruct gives

$$
x_{\alpha,2}=\left(\alpha^{-1}I-\alpha^{-2}C+\alpha^{-3}C^2\right)A^*y.
$$

For each fixed $\alpha>0$ this is a bounded [polynomial](../../../../../../../polynomial-split.md) in bounded operators, with

$$
\|x_{\alpha,2}(y^\delta)-x_{\alpha,2}(y)\|
\le\left(\frac{\|A\|}{\alpha}+\frac{\|A\|^3}{\alpha^2}+\frac{\|A\|^5}{\alpha^3}\right)\|y^\delta-y\|.
$$

Thus the supplied approximation also has continuous data dependence in its domain of use. It must not be extrapolated to $\alpha\downarrow0$ with $A$ fixed: its gain on any nonzero singular mode diverges, so it would not define a convergent regularization family there. **The exact Tikhonov filter supplies the well-posed regularized problem; the truncated formula is only a controlled computational approximation.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 70](../../../../paper-70-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
