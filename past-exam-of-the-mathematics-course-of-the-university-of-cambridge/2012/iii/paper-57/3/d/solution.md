<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $G=\Phi_G$ and $f=f_{NL}^{\rm local}$. The [Gaussian random field](../../../../../../gaussian-random-field.md) [covariance](../../../../../../covariance.md) in Fourier space is

$$
\langle G(\mathbf k)G(\mathbf p)\rangle=(2\pi)^3\delta^3(\mathbf k+\mathbf p)P(k).
$$

The [Fourier transform](../../../../../../fourier-transform.md) of the centered quadratic term is

$$
Q(\mathbf k)=\int\frac{d^3q}{(2\pi)^3}G(\mathbf q)G(\mathbf k-\mathbf q)-(2\pi)^3\delta^3(\mathbf k)\langle G^2\rangle.
$$

The Gaussian three-point function vanishes. At first order in $f$, the only terms are $f\langle Q_1G_2G_3\rangle$ and its two cyclic placements. For the first, [Wick theorem](../../../../../../wick-s-theorem.md) pairs four Gaussian factors in three ways. Pairing the two factors inside $Q_1$ together is canceled by the mean subtraction. Pairing one of those factors with $G_2$ and the other with $G_3$ gives $P(k_2)P(k_3)$ and the overall momentum delta; exchanging the two factors gives the same contribution. Thus

$$
\langle Q_1G_2G_3\rangle=2(2\pi)^3\delta^3(\mathbf k_1+\mathbf k_2+\mathbf k_3)P(k_2)P(k_3).
$$

Adding the three placements gives

$$
\boxed{\langle\Phi_1\Phi_2\Phi_3\rangle_c=2f_{NL}^{\rm local}(2\pi)^3\delta^3(\mathbf k_1+\mathbf k_2+\mathbf k_3)[P(k_1)P(k_2)+P(k_2)P(k_3)+P(k_3)P(k_1)]+O(f^3).}
$$

There is no second-order term because it would contain five centered Gaussian factors. The two-point function receives its first correction at $f^2$, whereas the displayed [local-type primordial non-Gaussianity](../../../../../../local-type-primordial-non-gaussianity.md) gives a three-point correlation already at $f$. For $P\propto k^{-3}$ the squeezed limit is $B_\Phi(q,k,k)\simeq4fP(q)P(k)$; this explains the strong correlation between a long potential and short-scale power. A finite [variance](../../../../../../variance-split.md) or regulator is needed to define the subtracted $\langle G^2\rangle$, as noted in part (b).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
