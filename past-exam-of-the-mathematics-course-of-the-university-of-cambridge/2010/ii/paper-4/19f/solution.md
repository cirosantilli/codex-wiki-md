<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

The [circle group](../../../../../circle-group.md) is $U(1)=\{z\in\mathbb C:|z|=1\}$ under multiplication. For continuous finite-dimensional complex representations, its irreducibles are the one-dimensional [characters](../../../../../character-of-a-representation.md)

$$
\boxed{\chi_m(z)=z^m,\qquad m\in\mathbb Z.}
$$

A [group representation](../../../../../group-representation.md) is a continuous homomorphism to the invertible linear maps; it is irreducible when it has no proper nonzero invariant subspace. [Compactness](../../../../../compact-space.md) permits an invariant Hermitian [inner product](../../../../../inner-product.md) by averaging. Since the resulting unitary operators commute for $U(1)$, simultaneous diagonalization reduces an irreducible to a [character](../../../../../character-of-a-representation.md), and the continuous [characters](../../../../../character-of-a-representation.md) of the circle have the stated integer winding number.

The group $SU(2)$ consists of unitary two-by-two complex matrices of [determinant](../../../../../determinant.md) one. Each has the unique form

$$
\begin{pmatrix}a&b\\-\overline b&\overline a\end{pmatrix},
\qquad |a|^2+|b|^2=1,
$$

identifying it homeomorphically with the unit 3-sphere in $\mathbb R^4$. This is the [Spin group](../../../../../spin-group.md) $\operatorname{Spin}(3)$. A [unitary matrix](../../../../../unitary-matrix.md) is conjugate to $\operatorname{diag}(e^{i\theta},e^{-i\theta})$, and its conjugacy class is determined by $0\le\theta\le\pi$, or equivalently its [trace](../../../../../matrix-trace.md) $2\cos\theta$.

The irreducible [representations of SU2](../../../../../representation-theory-of-su-2.md) are $V_n=\operatorname{Sym}^n(\mathbb C^2)$ for integers $n\ge0$, with dimension $n+1$. The symmetric power can be realized as homogeneous degree-$n$ [polynomials](../../../../../polynomial-split.md) in two variables, with the induced linear action. On the diagonal torus its [eigenvalues](../../../../../eigenvalue.md) are $e^{i(n-2j)\theta}$ for $j=0,\ldots,n$, so its [character](../../../../../character-of-a-representation.md), the [trace](../../../../../matrix-trace.md) of the representing operator, is

$$
\boxed{\chi_n(\theta)=\sum_{j=0}^ne^{i(n-2j)\theta}
=\frac{\sin((n+1)\theta)}{\sin\theta}.}
$$

At the endpoints use the continuous values $\chi_n(0)=n+1$ and $\chi_n(\pi)=(-1)^n(n+1)$. The highest-weight classification says this list is complete.

For the final action, multiplication of block matrices gives $(AB)_1=A_1B_1$, so conjugation is a linear [group representation](../../../../../group-representation.md). Decompose the underlying three-dimensional space as $V_1\oplus V_0$. Its endomorphism space is

$$
\operatorname{End}(V_1)\oplus\operatorname{Hom}(V_0,V_1)
\oplus\operatorname{Hom}(V_1,V_0)\oplus\operatorname{End}(V_0).
$$

The two off-diagonal blocks are each $V_1$, since the invariant alternating form identifies $V_1^*$ with $V_1$. The scalar part of $\operatorname{End}(V_1)$ is $V_0$ and its traceless part is $V_2$: the same alternating form identifies traceless endomorphisms with symmetric tensors of degree two. The lower scalar block is a second $V_0$. Thus

$$
\boxed{M_3(\mathbb C)\cong2V_0\oplus2V_1\oplus V_2.}
$$

The dimensions add to $2+4+3=9$, and its [character](../../../../../character-of-a-representation.md) is $2\chi_0+2\chi_1+\chi_2$.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
