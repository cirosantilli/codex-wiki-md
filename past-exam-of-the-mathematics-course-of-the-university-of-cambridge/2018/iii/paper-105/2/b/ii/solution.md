<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $T:H^1(U)\to L^2(\partial U)$ be the trace map from the [Sobolev trace theorem](../../../../../../../sobolev-trace-theorem.md). The [weak Robin problem for a uniformly elliptic operator](../../../../../../../weak-robin-problem-for-a-uniformly-elliptic-operator.md) uses all of $H^1(U)$ as the test space, since a [Robin boundary condition](../../../../../../../robin-boundary-condition.md) does not require a zero trace. Define

$$
\begin{aligned}
B_\lambda[u,v]={}&\int_U\left(\sum_{i,j}a^{ij}u_{x_i}v_{x_j}
+\sum_i b^iu_{x_i}v+(c+\lambda)uv\right)dx\\
&+\int_{\partial U}\beta\,Tu\,Tv\,dS.
\end{aligned}
$$

The [weak formulation](../../../../../../../weak-formulation.md) is

$$
\boxed{u\in H^1(U),\qquad B_\lambda[u,v]=\int_Ufv\,dx
\quad\text{for every }v\in H^1(U).}
$$

For a [classical solution](../../../../../../../classical-solution.md), [integration by parts](../../../../../../../integration-by-parts.md) produces the boundary term $-\int_{\partial U}(\sum a^{ij}u_{x_i}\nu_j)v$. Substituting the [Robin boundary condition](../../../../../../../robin-boundary-condition.md) replaces it by $\int_{\partial U}\beta uv$, giving the displayed identity.

Conversely, if $u\in C^2(\overline U)$ satisfies the identity, tests $v\in C_c^\infty(U)$ first show $(L+\lambda)u=f$ in the sense of [distributions](../../../../../../../distribution-mathematical-analysis.md). Subtracting this interior equality after [integration by parts](../../../../../../../integration-by-parts.md) gives

$$
\int_{\partial U}\left(\sum_{i,j}a^{ij}u_{x_i}\nu_j+\beta u\right)Tv\,dS=0.
$$

Every smooth boundary function is the trace of a smooth function on $\overline U$. The boundary residual is continuous, so this proves the boundary equation pointwise. Thus the formulations agree for $C^2$ solutions. If $f$ is continuous the interior equation holds pointwise; for merely $f\in L^2$, equality with that given representative of $f$ is understood [almost everywhere](../../../../../../../almost-everywhere.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
