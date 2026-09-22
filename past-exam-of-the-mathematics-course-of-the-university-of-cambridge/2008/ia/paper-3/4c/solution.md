<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

For a constant orthogonal Cartesian coordinate change $x'_i=R_{ij}x_j$, a [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md) has components satisfying

$$
\boxed{T'_{ij}(x')=R_{ik}R_{jl}T_{kl}(x).}
$$

Both indices transform by the coordinate-change [matrix](../../../../../matrix.md); summation over repeated indices is understood by the [Einstein summation convention](../../../../../einstein-notation.md). A [vector](../../../../../vector.md) would have the one-index rule $U'_i=R_{ik}U_k$.

Define $U_i=\partial T_{ij}/\partial x_j$. Since $x_m=R_{jm}x'_j$, the [chain rule](../../../../../chain-rule.md) gives $\partial/\partial x'_j=R_{jm}\partial/\partial x_m$. The [rotation](../../../../../rotation-mathematics.md) coefficients are constant, so

$$
\begin{aligned}
U'_i&=\frac{\partial T'_{ij}}{\partial x'_j}
=R_{jm}R_{ik}R_{jl}\frac{\partial T_{kl}}{\partial x_m}\\
&=R_{ik}\delta_{ml}\frac{\partial T_{kl}}{\partial x_m}
=R_{ik}\frac{\partial T_{kl}}{\partial x_l}=R_{ik}U_k.
\end{aligned}
$$

The identity $R_{jm}R_{jl}=\delta_{ml}$ follows from orthogonality. Hence **the contracted derivative transforms as a [vector](../../../../../vector.md)**. This proves the [divergence of a Cartesian second-rank tensor](../../../../../divergence-of-a-cartesian-second-rank-tensor.md) rule for global Cartesian [rotations](../../../../../rotation-mathematics.md). In curvilinear coordinates the corresponding construction uses a [covariant derivative](../../../../../covariant-derivative.md); ordinary partial derivatives alone would not have the stated tensorial transformation law.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
