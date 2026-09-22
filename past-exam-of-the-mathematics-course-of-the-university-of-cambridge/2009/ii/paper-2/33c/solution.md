<h1 id="33c/solution">Solution</h1>

↑ **Parent:** [33C](../33c.md)

Putting the [unit](../../../../../unit-in-a-ring.md) vector along a coordinate axis gives $\sigma_i^2=I$. Putting it along $(e_i+e_j)/\sqrt2$ gives $\sigma_i\sigma_j+\sigma_j\sigma_i=0$ for $i\ne j$. Combining the resulting anticommutators with the given [commutators](../../../../../commutator.md) yields $\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k$, and hence

$$
\boxed{(\mathbf a\cdot\boldsymbol\sigma)(\mathbf b\cdot\boldsymbol\sigma)
=(\mathbf a\cdot\mathbf b)I+i(\mathbf a\times\mathbf b)\cdot\boldsymbol\sigma.}
$$

The operators $S_i=(\hbar/2)\sigma_i$ obey angular-momentum [commutators](../../../../../commutator.md) and $\mathbf S^2=3\hbar^2I/4$, the spin-one-half value. In a spin-half irreducible sector they are the intrinsic [spin](../../../../../spin.md) operators; the algebra also permits direct sums of such sectors.

Since $Q=\mathbf n\cdot\boldsymbol\sigma$ is Hermitian with $Q^2=I$, its operators $P_\pm=(I\pm Q)/2$ are Hermitian and satisfy $P_\pm^2=P_\pm$, $P_+P_-=0$ and $P_++P_-=I$. Moreover $QP_\pm=\pm P_\pm$. Thus $|\chi\rangle=P_+|\chi\rangle+P_-|\chi\rangle$ is its [orthogonal](../../../../../orthogonal-vectors.md) [eigenstate](../../../../../eigenstate.md) decomposition, omitting any zero component. The Born probabilities for a normalized state are

$$
\boxed{\|P_\pm|\chi\rangle\|^2=\langle\chi|P_\pm|\chi\rangle=\tfrac12(1\pm\langle\chi|Q|\chi\rangle).}
$$

For [spin](../../../../../spin.md) up along $\mathbf m$, the anticommutator $\{\mathbf m\cdot\boldsymbol\sigma,\sigma_j\}=2m_jI$ gives $\langle\sigma_j\rangle=m_j$. Therefore **the probability of [spin](../../../../../spin.md) up along $\mathbf n$ is $(1+\mathbf n\cdot\mathbf m)/2$**.

## ↑ Ancestors (10)

1. [33C](../33c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
