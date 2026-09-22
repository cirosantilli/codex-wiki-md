<h1 id="31a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There is a literal inconsistency in the stated [Riemann-Hilbert problem](../../../../../../riemann-hilbert-problem.md): a jump [matrix](../../../../../../matrix.md) $S(k)$ tending to zero is incompatible with $\mu_\pm\to I$. Along the real axis the conjugating exponentials are unitary, so the right side of the jump tends to zero while the left side tends to $I$. **No normalized solution satisfies the printed decay condition.** The intended condition is $S(k)\to I$, or replacement of $S$ in the jump by $I+S$ when $S$ denotes its decaying part.

For this corrected problem assume a regular, invertible, pole-free solution, differentiable in $x,t$, with the required expansion uniformly at infinity. These conditions matter: arbitrary jump data need not be solvable, and [poles](../../../../../../pole.md) would contribute extra terms. Write $\sigma=\sigma_3$ and $\mu=I+\mu_1/k+\mu_2/k^2+\cdots$. Matching the nondecaying coefficients in the two differential expressions yields

$$
\boxed{Q=i[\sigma,\mu_1],\qquad A=2i[\sigma,\mu_1]=2Q,\qquad
B=2i[\sigma,\mu_2]-A\mu_1.}
$$

The first expression makes $Q$ off-diagonal.

These matches really establish the differential equations, rather than just formal identities. Let $G=e^{-i(kx+2k^2t)\sigma}S(k)e^{i(kx+2k^2t)\sigma}$. It satisfies $G_x=-ik[\sigma,G]$ and $G_t=-2ik^2[\sigma,G]$. Differentiating $\mu_+=\mu_-G$ consequently shows that

$$
R_x=(\mu_x+ik[\sigma,\mu]-Q\mu)\mu^{-1},\qquad
R_t=(\mu_t+2ik^2[\sigma,\mu]-(kA+B)\mu)\mu^{-1}
$$

have matching boundary values. They therefore extend holomorphically across the contour. The chosen coefficients make both residuals $O(k^{-1})$ at infinity. Their absence of [poles](../../../../../../pole.md) and [Liouville theorem](../../../../../../liouville-theorem.md) imply $R_x=R_t=0$, proving the required [Lax pair](../../../../../../lax-pair.md) under the corrected hypotheses. This is [matrix NLS reconstruction from a normalized Riemann-Hilbert problem](../../../../../../matrix-nls-reconstruction-from-a-normalized-riemann-hilbert-problem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31A](../../31a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
