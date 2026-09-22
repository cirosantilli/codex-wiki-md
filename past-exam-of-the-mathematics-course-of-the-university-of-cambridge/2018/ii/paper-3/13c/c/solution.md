<h1 id="13c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume again that all boundary terms vanish. Multiplying the [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) by $x_k$ and integrating by parts gives

$$
\begin{aligned}
\frac d{dt}\langle x_k\rangle
&=-\int x_k\,\partial_i(A_iP)\,dV
+\frac12\int x_k\,\partial_i\partial_j(B_{ij}P)\,dV\\
&=\int\delta_{ik}A_iP\,dV
=\boxed{\langle A_k\rangle}.
\end{aligned}
$$

The diffusion term vanishes after the second integration by parts.

Similarly, $\partial_i(x_kx_l)=\delta_{ik}x_l+\delta_{il}x_k$ and

$$
\partial_i\partial_j(x_kx_l)
=\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}.
$$

Because $B$ is symmetric,

$$
\boxed{
\frac d{dt}\langle x_kx_l\rangle
=\langle x_lA_k+x_kA_l+B_{kl}\rangle.}
$$

These are the [First two moments of a multivariate Fokker-Planck equation](../../../../../../first-two-moments-of-a-multivariate-fokker-planck-equation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13C](../../13c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
