<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Use [suffix notation](../../../../../einstein-notation.md), with repeated indices summed from one to three. The [cross product](../../../../../cross-product.md), [divergence](../../../../../divergence.md), and [curl](../../../../../curl.md) have components $(\mathbf A\times\mathbf B)_i=\epsilon_{ijk}A_jB_k$, $\nabla\cdot\mathbf A=\partial_iA_i$, and $(\nabla\times\mathbf A)_i=\epsilon_{ijk}\partial_jA_k$. Here $\epsilon$ is the [Levi-Civita symbol](../../../../../levi-civita-symbol.md).

The [product rule](../../../../../product-rule.md) gives

$$
\partial_i(\epsilon_{ijk}A_jB_k)=\epsilon_{ijk}(\partial_iA_j)B_k+\epsilon_{ijk}A_j\partial_iB_k.
$$

Using the cyclic identity $\epsilon_{ijk}=\epsilon_{kij}$ in the first term and $\epsilon_{ijk}=-\epsilon_{jik}$ in the second identifies these terms as $B_k(\nabla\times\mathbf A)_k$ and $-A_j(\nabla\times\mathbf B)_j$. Therefore

$$
\boxed{\nabla\cdot(\mathbf A\times\mathbf B)=\mathbf B\cdot(\nabla\times\mathbf A)-\mathbf A\cdot(\nabla\times\mathbf B).}
$$

For the second identity, contract two [Levi-Civita symbols](../../../../../levi-civita-symbol.md), using $\epsilon_{ijk}\epsilon_{klm}=\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl}$:

$$
\begin{aligned}
[\nabla\times(\mathbf A\times\mathbf B)]_i
&=\epsilon_{ijk}\epsilon_{klm}\partial_j(A_lB_m)\\
&=\partial_j(A_iB_j-A_jB_i)\\
&=B_j\partial_jA_i+A_i\partial_jB_j-A_j\partial_jB_i-B_i\partial_jA_j.
\end{aligned}
$$

The four component expressions translate into

$$
\boxed{\nabla\times(\mathbf A\times\mathbf B)=(\mathbf B\cdot\nabla)\mathbf A-\mathbf B(\nabla\cdot\mathbf A)-(\mathbf A\cdot\nabla)\mathbf B+\mathbf A(\nabla\cdot\mathbf B).}
$$

Both derivations require only continuously differentiable [vector fields](../../../../../vector-field.md); no additional divergence-free assumptions are used.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
