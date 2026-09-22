<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We use a [closed manifold](../../../../../../closed-manifold.md) of positive [dimension](../../../../../../dimension-vector-space.md) $n$. The nonnegative [positive Laplace-Beltrami operator](../../../../../../positive-laplace-beltrami-operator.md) on functions is

$$
\boxed{\Delta=d^*d=-\rho^{-1}\partial_i(\rho g^{ij}\partial_j),\qquad\rho=\sqrt{\det(g_{ij})}.}
$$

It satisfies $\langle\Delta f,f\rangle=\int_M|df|_g^2\,d\mathrm{vol}_g$. Its domain as a [self-adjoint operator](../../../../../../self-adjoint-operator.md) on $L^2(M)$ is $H^2(M)$. The analytic argument in Question 4(d), with $q=0$, gives a smooth [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) and ordered [eigenvalues](../../../../../../eigenvalue.md) $0=\lambda_0\leq\lambda_1\leq\cdots\to\infty$.

We prove a quantitative counting bound from local [Fourier series](../../../../../../fourier-series-split.md), rather than assume a spectral asymptotic formula. Choose a finite coordinate cover and smooth functions $\chi_\alpha$ compactly supported in its charts with $\sum_\alpha\chi_\alpha^2=1$. This can be obtained by normalizing an ordinary nonnegative [partition of unity](../../../../../../partition-of-unity.md) by the square root of the sum of its squares. Embed each chart support in a fixed coordinate [torus](../../../../../../torus.md), and extend $v_\alpha=\chi_\alpha f$ by zero there. Uniform comparison of the coordinate and metric norms, and differentiation of the cutoffs, give constants independent of $f$ such that

$$
c\|f\|_2^2\leq\sum_\alpha\|v_\alpha\|_{L^2(\mathbb T^n)}^2,
\qquad
\sum_\alpha\|v_\alpha\|_{H^1(\mathbb T^n)}^2
\leq C\bigl(\|df\|_2^2+\|f\|_2^2\bigr).
$$

Let $P_R$ retain the [Fourier modes](../../../../../../fourier-mode.md) $|k|\leq R$. [Parseval identity](../../../../../../parseval-identity.md) gives

$$
\|(I-P_R)v\|_2^2\leq R^{-2}\|v\|_{H^1}^2\qquad(R\geq1).
$$

The map $f\mapsto(P_Rv_\alpha)_\alpha$ has target [dimension](../../../../../../dimension-vector-space.md) at most $C_0R^n$, since there are at most $C_nR^n$ lattice points in each cutoff ball.

Let $E_\Lambda$ span all [eigenfunctions](../../../../../../eigenfunction.md) with [eigenvalues](../../../../../../eigenvalue.md) at most $\Lambda$. For $f\in E_\Lambda$, $\|df\|_2^2\leq\Lambda\|f\|_2^2$. If every retained local coefficient vanishes, the preceding estimates imply

$$
c\|f\|_2^2\leq C R^{-2}(1+\Lambda)\|f\|_2^2.
$$

Choose $R=b\sqrt{1+\Lambda}$ with fixed $b$ sufficiently large. Then this is impossible unless $f=0$, so the finite-dimensional coefficient map is injective on $E_\Lambda$. Therefore the [eigenvalue counting function](../../../../../../eigenvalue-counting-function.md) satisfies

$$
N(\Lambda):=\dim E_\Lambda\leq C_1(1+\Lambda)^{n/2}.
$$

Taking $\Lambda=\lambda_k$ gives $k+1\leq C_1(1+\lambda_k)^{n/2}$, so $\lambda_k\geq c_1(k+1)^{2/n}-1$. For all sufficiently large $k$, this implies $\lambda_k\geq A_0k^{2/n}$.

If $M$ is connected, the zero [eigenvalue](../../../../../../eigenvalue.md) is simple: $\Delta f=0$ implies $df=0$, hence $f$ is constant. Thus every $\lambda_k$ for $k\geq1$ is positive. Taking the minimum of $A_0$ and the finitely many positive ratios $\lambda_k/k^{2/n}$ below the large-$k$ threshold proves

$$
\boxed{\lambda_k\geq Ak^{2/n}\quad(k\geq0),\qquad A>0.}
$$

Connectedness is implicit in the printed claim. If $M$ has $b>1$ connected components, zero has multiplicity $b$, and the claim fails already at $k=1$. The same proof gives $\lambda_k\geq A\max\{k-b+1,0\}^{2/n}$ for all $k$, as well as the universal counting bound above. These finite initial zero modes do not affect part (d).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
