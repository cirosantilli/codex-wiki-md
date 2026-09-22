<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Undo the commutator gauge by putting $\psi_j=\mu_je^{-i\theta\sigma_3}$. Then $\psi_{j,x}=(-ik\sigma_3+Q)\psi_j$ and $\psi_{j,t}=(-2ik^2\sigma_3+V)\psi_j$, with $V=2kQ-iQ_x\sigma_3-i|q|^2\sigma_3$. The [trace](../../../../../../matrix-trace.md) of each coefficient matrix is zero, so all normalized fundamental matrices have determinant one. Their ratios $\psi_2^{-1}\psi_j$ are independent of both $x$ and $t$, because differentiation cancels the common left-hand coefficient.

Call these constant matrices $s$ for $j=3$ and $S$ for $j=1$. Returning to the commutator gauge gives

$$
\boxed{\mu_3=\mu_2e^{-i\theta\widehat\sigma_3}s,\qquad\mu_1=\mu_2e^{-i\theta\widehat\sigma_3}S.}
$$

Here $e^{\alpha\widehat\sigma_3}C=e^{\alpha\sigma_3}Ce^{-\alpha\sigma_3}$. Evaluation at $(0,0)$ gives $s=\mu_3(0,0,k)$, computed solely by the spatial [Volterra integral equation](../../../../../../volterra-integral-equation.md) for the initial potential. At $(0,T)$ the normalization of $\mu_1$ gives

$$
\boxed{S(k)=e^{2ik^2T\widehat\sigma_3}\mu_2(0,T,k)^{-1}.}
$$

Thus $S$ is computed by integrating the time [Lax pair](../../../../../../lax-pair.md) for $\mu_2(0,t,k)$ from zero to $T$. It uses both boundary traces $q(0,t)$ and $q_x(0,t)$ before their compatibility is enforced.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
