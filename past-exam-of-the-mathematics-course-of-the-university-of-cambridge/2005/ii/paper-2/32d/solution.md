<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

Taking $n=e_i$ gives $\sigma_i^2=I$. Taking $n=(e_i+e_j)/\sqrt2$ for $i\ne j$ and expanding the square gives $\sigma_i\sigma_j+\sigma_j\sigma_i=0$. Thus the [anticommutator](../../../../../anticommutator.md) and [commutator](../../../../../commutator.md) together imply

$$
\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k,
\qquad\boxed{(a\cdot\sigma)(b\cdot\sigma)=(a\cdot b)I+i(a\times b)\cdot\sigma.}
$$

Since $n\cdot\sigma$ is [Hermitian](../../../../../hermitian-operator.md) and $\theta$ is real, the exponent is [anti-Hermitian](../../../../../skew-hermitian-matrix.md). Its exponential has inverse equal to its adjoint and is therefore [unitary](../../../../../unitary-connection.md). Splitting the [exponential series](../../../../../exponential-series.md) into even and odd powers, using $(n\cdot\sigma)^2=I$, gives

$$
\boxed{U=I\cos(\theta/2)-i(n\cdot\sigma)\sin(\theta/2).}
$$

Put $N=n\cdot\sigma,M=m\cdot\sigma$ with $m\perp n$. Then $NM=i(n\times m)\cdot\sigma$, $MN=-NM$, and $NMN=-M$. Expanding $(c-iNs)M(c+iNs)$ gives $(c^2-s^2)M-2icsNM$. Consequently

$$
\boxed{UMU^{-1}=(m\cdot\sigma)\cos\theta+((n\times m)\cdot\sigma)\sin\theta.}
$$

The spin-half [angular momentum](../../../../../angular-momentum.md) is $S_i=\hbar\sigma_i/2$. The commutators then become $[S_i,S_j]=i\hbar\epsilon_{ijk}S_k$, and $(n\cdot S)^2=\hbar^2I/4$ expresses the two possible directional [spin](../../../../../spin.md) values $\pm\hbar/2$. Also $S^2=3\hbar^2I/4$, appropriate to [spin](../../../../../spin.md) one half. The exponential represents a spatial rotation on [spin](../../../../../spin.md) states.

Choose $n=(0,1,0)$ and initially $\sigma_3|\chi\rangle=|\chi\rangle$. The conjugation formula sends $\sigma_3$ to $\sigma_3\cos\theta+\sigma_1\sin\theta$. Therefore

$$
(\sigma_1\sin\theta+\sigma_3\cos\theta)U|\chi\rangle
=U\sigma_3|\chi\rangle=U|\chi\rangle.
$$

Thus **$U|\chi\rangle$ is [spin](../../../../../spin.md) up along $(\sin\theta,0,\cos\theta)$**, as required.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
