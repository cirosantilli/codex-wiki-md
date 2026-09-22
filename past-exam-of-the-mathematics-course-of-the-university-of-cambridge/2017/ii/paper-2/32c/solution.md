<h1 id="32c/solution">Solution</h1>

↑ **Parent:** [32C](../32c.md)

Taking $\mathbf n$ along a coordinate axis gives $\sigma_i^2=I$. Taking $\mathbf n=(e_i+e_j)/\sqrt2$ for $i\ne j$ gives $\{\sigma_i,\sigma_j\}=0$. Combining this [anticommutator](../../../../../anticommutator.md) relation with the specified [commutator](../../../../../commutator.md) gives

$$
\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k,
$$

and contraction with $a_ib_j$ proves

$$
\boxed{(\mathbf a\cdot\boldsymbol\sigma)(\mathbf b\cdot\boldsymbol\sigma)
=(\mathbf a\cdot\mathbf b)I+i(\mathbf a\times\mathbf b)\cdot\boldsymbol\sigma.}
$$

The operators for [spin angular momentum](../../../../../spin.md), $S_i=\hbar\sigma_i/2$, satisfy $[S_i,S_j]=i\hbar\epsilon_{ijk}S_k$ and $S^2=3\hbar^2I/4$, identifying spin $1/2$. The usual irreducible spin space is two-dimensional; the assumptions also allow repeated copies of it if no Hilbert-space dimension is specified.

Since $\mathbf n\cdot\boldsymbol\sigma$ is Hermitian and squares to $I$, $P_\pm=(I\pm\mathbf n\cdot\boldsymbol\sigma)/2$ are Hermitian, $P_\pm^2=P_\pm$, $P_+P_-=0$ and $P_++P_-=I$. They are its [spectral projectors](../../../../../spectral-projector.md). Write

$$
|\chi\rangle=P_+|\chi\rangle+P_-|\chi\rangle.
$$

Each nonzero term is a scalar multiple of a normalized eigenstate with [eigenvalue](../../../../../eigenvalue.md) $\pm1$. The [Born rule](../../../../../born-rule.md) gives, for normalized $|\chi\rangle$,

$$
\boxed{\mathbb P(\pm1)=\|P_\pm\chi\|^2=\langle\chi|P_\pm|\chi\rangle=\frac12(1\pm\langle\mathbf n\cdot\boldsymbol\sigma\rangle).}
$$

If $(\mathbf m\cdot\boldsymbol\sigma)|\chi\rangle=|\chi\rangle$, [expectation](../../../../../expected-value.md) of $\{\mathbf m\cdot\boldsymbol\sigma,\mathbf a\cdot\boldsymbol\sigma\}=2\mathbf m\cdot\mathbf a$ gives $\langle\mathbf a\cdot\boldsymbol\sigma\rangle=\mathbf m\cdot\mathbf a$. Taking $\mathbf a=\mathbf n$ yields $\boxed{\mathbb P(\text{up along }\mathbf n)=\tfrac12(1+\mathbf n\cdot\mathbf m)}$.

## ↑ Ancestors (10)

1. [32C](../32c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
