<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $B_R(x_0)\subset B_1$, put $A_0=A(x_0)$, and let $v$ have the same boundary values as $u$ while solving $\operatorname{div}(A_0\nabla v)=0$. Then $w=u-v\in W_0^{1,2}(B_R)$ satisfies

$$
\operatorname{div}(A_0\nabla w)
=\operatorname{div}((A_0-A(x))\nabla u).
$$

Since $u\in C^1$ gives $|Du|\leq L$ locally, the supplied energy estimate and [Hölder continuity](../../../../../../holder-space.md) of $A$ yield

$$
\int_{B_R}|\nabla w|^2\leq C L^2[A]_{C^\alpha}^2R^{n+2\alpha}.
$$

The constant-coefficient decay estimate gives

$$
\int_{B_\rho}|\nabla v-(\nabla v)_{B_\rho}|^2
\leq C(\rho/R)^{n+2}
\int_{B_R}|\nabla v-(\nabla v)_{B_R}|^2.
$$

Thus, for $\Phi(r)=\int_{B_r}|\nabla u-(\nabla u)_{B_r}|^2$,

$$
\Phi(\rho)\leq C(\rho/R)^{n+2}\Phi(R)+CR^{n+2\alpha}.
$$

Because $n+2>n+2\alpha$, the [Campanato iteration lemma](../../../../../../campanato-iteration-lemma.md) gives $\Phi(\rho)\leq C\rho^{n+2\alpha}$ on balls in $B_{1/2}$. Hence $\nabla u\in\mathcal L^{2,n+2\alpha}=C^{0,\alpha}$ and $u\in C^{1,\alpha}(B_{1/2})$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
