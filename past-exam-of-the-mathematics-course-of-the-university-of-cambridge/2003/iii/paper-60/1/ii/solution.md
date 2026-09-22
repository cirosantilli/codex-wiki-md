<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The third planform is fixed by a diagonal [reflection](../../../../../../reflection-mathematics.md) and changes sign under a quarter-turn. Extend the preceding [group representation](../../../../../../group-representation.md) by

$$
r(A,B,C)=(B,-A,-C),\qquad s(A,B,C)=(-A,B,C).
$$

The other diagonal [reflection](../../../../../../reflection-mathematics.md) changes only the sign of $B$. Consequently the first two components of an [equivariant dynamical system](../../../../../../equivariant-dynamical-system.md) have factors $A$ and $B$, whereas its third component is even in each of $A,B$. The quarter-turn exchanges $A^2$ and $B^2$ while negating $C$. Its admissible quadratic coupling is therefore $A^2-B^2$ in the third equation and opposite $AC,BC$ couplings in the first two. At cubic order the only new terms are $AC^2,BC^2,C^3,C(A^2+B^2)$. The linear action on the two-dimensional irreducible mode has one coefficient $\mu_1$, while the distinct scalar representation has its own coefficient $\mu_2$. A small splitting of the two marginal linear modes supplies these two unfolding parameters. With real coefficients the resulting [amplitude equations](../../../../../../amplitude-equation.md) are

$$
\begin{aligned}
A_T&=\mu_1A-\alpha_0A^3-\lambda AB^2-\alpha_1AC-\alpha_2AC^2,\\
B_T&=\mu_1B-\alpha_0B^3-\lambda A^2B+\alpha_1BC-\alpha_2BC^2,\\
C_T&=\mu_2C-\gamma_0C^3+\gamma_1(A^2-B^2)-\gamma_2C(A^2+B^2).
\end{aligned}
$$

These equations follow by listing all equivariant monomials through degree three; the displayed minus signs are coefficient conventions, not consequences of symmetry.

In the specified reduced system put $A=B=s$, $C=0$. A nonzero branch exists for $\mu_1>0$, with $q=s^2=\mu_1/(1+\lambda)$. Write perturbations as $u=(\delta A+\delta B)/2$, $v=(\delta A-\delta B)/2$, and $c=\delta C$. [Linearization](../../../../../../linearization.md) gives

$$
u_T=-2\mu_1u,\qquad
\begin{pmatrix}v\\c\end{pmatrix}_T=
\underbrace{\begin{pmatrix}p&-\alpha_1s\\4\gamma_1s&\mu_2\end{pmatrix}}_{M}
\begin{pmatrix}v\\c\end{pmatrix},\qquad p=2(\lambda-1)q>0.
$$

For the [square-pattern interaction with a sign-changing scalar mode](../../../../../../square-pattern-interaction-with-a-sign-changing-scalar-mode.md), the remaining [eigenvalues](../../../../../../eigenvalue.md) have sum $\tau=p+\mu_2$ and product $D=p\mu_2+4\alpha_1\gamma_1q=p(\mu_2+K)$, where $K=2\alpha_1\gamma_1/(\lambda-1)>0$. A real two-dimensional [stability matrix](../../../../../../stability-matrix.md) has both [eigenvalues](../../../../../../eigenvalue.md) in the left half-plane exactly when its [trace](../../../../../../matrix-trace.md) is negative and its [determinant](../../../../../../determinant.md) is positive. Therefore

$$
\boxed{-K<\mu_2<-p,\qquad 0<\mu_1<\frac{(1+\lambda)\alpha_1\gamma_1}{(\lambda-1)^2}.}
$$

If $\mu_2<-K$, the block has negative [determinant](../../../../../../determinant.md) and one growing direction, explaining the instability at sufficiently small $\mu_2$. At the lower endpoint $\mu_2=-K$, one [eigenvalue](../../../../../../eigenvalue.md) is zero and the other is $p-K<0$. The symmetry $(A,B,C)\mapsto(B,A,-C)$ fixes the diagonal state and negates its critical $(v,c)$ direction. Thus a generic nonlinear unfolding has a [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) to unequal-amplitude states with nonzero $C$.

At the upper endpoint $\mu_2=-p$, the [trace](../../../../../../matrix-trace.md) vanishes and

$$
\boxed{\omega_H^2=\det M=p(K-p)>0.}
$$

The symmetric [eigenvalue](../../../../../../eigenvalue.md) remains negative. The critical conjugate pair crosses the imaginary axis with [derivative](../../../../../../derivative.md) $d\operatorname{Re}\sigma/d\mu_2=1/2$. If its cubic [Hopf normal form](../../../../../../hopf-normal-form.md) coefficient is nonzero, this is a [Hopf bifurcation](../../../../../../hopf-bifurcation.md) and nearby periodic solutions exist on one side. Their stability and the side of existence depend on that coefficient; the linear calculation does not determine them. It does establish the generic possibility of oscillating square patterns. The equality $p=K$ is a double-zero degeneracy, outside this nondegenerate [Hopf bifurcation](../../../../../../hopf-bifurcation.md) argument.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
