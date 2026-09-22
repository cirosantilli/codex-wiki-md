<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

An [isotropic tensor](../../../../../isotropic-tensor.md) has unchanged components under every rotation: for rank four, $A_{ijkl}=R_{ia}R_{jb}R_{kc}R_{ld}A_{abcd}$. Orthogonality gives $R_{ia}R_{ja}=\delta_{ij}$, so each product of paired [Kronecker deltas](../../../../../kronecker-delta.md) is invariant. Every linear combination of $\delta_{ij}\delta_{kl}$, $\delta_{ik}\delta_{jl}$ and $\delta_{il}\delta_{jk}$ is therefore isotropic, for arbitrary coefficients.

For the integral, differentiation away from the origin gives

$$
\partial_k\partial_l\frac1r=\frac{3x_kx_l}{r^5}-\frac{\delta_{kl}}{r^3}.
$$

After multiplication by $x_ix_j$, this behaves as $O(r^{-1})$ and is locally integrable in three dimensions. Interpret the integral as the limit with a small central ball removed. A rotation preserves the integration ball and the radial kernel, so the resulting $B$ is an [isotropic tensor integral](../../../../../isotropic-tensor-integral.md). The symmetries $i\leftrightarrow j$ and $k\leftrightarrow l$ force the two cross-pair coefficients equal:

$$
B_{ijkl}=A\delta_{ij}\delta_{kl}+B(\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).
$$

Taking the trace in $k,l$ uses $\nabla^2(r^{-1})=0$ off the origin and gives $3A+2B=0$. For the other contraction, the displayed Hessian gives $\sum_{ij}x_ix_j\partial_i\partial_j(r^{-1})=2/r$. Thus

$$
3A+12B=\int_{r<a}\frac2r\,dV=8\pi\int_0^a r\,dr=4\pi a^2.
$$

Solving gives $B=2\pi a^2/5$ and $A=-4\pi a^2/15$. Therefore **the requested tensor is**

$$
\boxed{B_{ijkl}=\frac{2\pi a^2}{15}\left(-2\delta_{ij}\delta_{kl}+3\delta_{ik}\delta_{jl}+3\delta_{il}\delta_{jk}\right).}
$$

This is the [quadratically weighted inverse-radius Hessian integral](../../../../../quadratically-weighted-inverse-radius-hessian-integral.md). The origin creates no extra contribution to this weighted integral; even the distributional point term in the unweighted Hessian is annihilated by $x_ix_j$.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
