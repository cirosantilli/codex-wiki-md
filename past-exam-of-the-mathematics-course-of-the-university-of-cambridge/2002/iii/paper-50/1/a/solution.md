<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\langle q\rangle=|\Omega|^{-1}\int_\Omega q\,dx$, $E=\langle\varepsilon\rangle$ and $S=\langle\sigma\rangle$. Use the [infinitesimal strain tensor](../../../../../../infinitesimal-strain-tensor.md), symmetric [stress](../../../../../../stress.md), zero [body force](../../../../../../body-force.md), and the outward unit normal $n$. The [divergence theorem](../../../../../../divergence-theorem.md) applied separately to the two displacement derivatives gives

$$
\boxed{E_{ij}=\frac1{2|\Omega|}\int_{\partial\Omega}(u_i n_j+u_j n_i)\,dS.}
$$

For [static elastic equilibrium](../../../../../../static-elastic-equilibrium.md), $\sigma_{ik,k}=0$, and therefore $\partial_k(\sigma_{ik}x_j)=\sigma_{ij}$. With [traction](../../../../../../traction.md) $t_i=\sigma_{ik}n_k$, the [divergence theorem](../../../../../../divergence-theorem.md) now gives

$$
\boxed{S_{ij}=\frac1{|\Omega|}\int_{\partial\Omega}t_i x_j\,dS.}
$$

The right-hand side is automatically symmetric because the volume [stress tensor](../../../../../../cauchy-stress-tensor.md) is symmetric; it can also be written as the integral of $(t_i x_j+t_j x_i)/2$.

To prove the work identity, put $v=u-Ex$. The constant symmetric [tensor](../../../../../../tensor.md) $S$ is equilibrated, so [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\begin{aligned}
\int_{\partial\Omega}(\sigma-S)n\cdot v\,dS
&=\int_\Omega(\sigma-S):\operatorname{sym}\nabla v\,dx\\
&=\int_\Omega(\sigma-S):(\varepsilon-E)\,dx\\
&=\int_\Omega\sigma:\varepsilon\,dx-|\Omega|S:E.
\end{aligned}
$$

Here the two cross terms each equal $|\Omega|S:E$, and the last constant term restores one of them. Division by the volume proves the required identity. In particular, affine boundary [displacement](../../../../../../displacement.md) makes $v=0$ on the boundary and yields the [Hill-Mandel energy identity](../../../../../../hill-mandel-energy-identity.md). The zero-[body force](../../../../../../body-force.md) hypothesis matters: otherwise the first [integration by parts](../../../../../../integration-by-parts.md) has an additional volume-force term.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
