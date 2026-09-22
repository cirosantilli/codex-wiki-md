<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Remove the commutator gauge by setting $\Psi_j=\mu_je^{i\theta\sigma_3}$. These matrices all satisfy the ordinary first-order systems

$$
\Psi_x=(ik\sigma_3+Q)\Psi,\qquad
\Psi_t=(-4ik^3\sigma_3+\widetilde Q)\Psi.
$$

Both coefficient matrices are traceless, so the normalization implies $\det\Psi_j=\det\mu_j=1$. For any two solutions, differentiating $\Psi_2^{-1}\Psi_j$ shows that it is independent of both $x$ and $t$. Calling these constant matrices $s$ and $S$ gives

$$
\boxed{\mu_3=\mu_2e^{i\theta\widehat\sigma_3}s,\qquad
\mu_1=\mu_2e^{i\theta\widehat\sigma_3}S.}
$$

At $(0,0)$, $\mu_2=I$, so $s=\mu_3(0,0,k)$. More generally,

$$
s=e^{-ikx\widehat\sigma_3}[\mu_2(x,0,k)^{-1}\mu_3(x,0,k)].
$$

At $(0,T)$ the other normalization is $\mu_1=I$, so

$$
\boxed{S=e^{4ik^3T\widehat\sigma_3}\mu_2(0,T,k)^{-1}.}
$$

Thus $s$ is determined by the initial spatial [Volterra integral equation](../../../../../../volterra-integral-equation.md), while $S$ is determined by the boundary time equation evaluated at $T$. The latter uses all boundary values occurring in $\widetilde Q$, including the initially unknown second-derivative trace. It is the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md), rather than a claim of independence of those traces, that supplies their constraint.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
