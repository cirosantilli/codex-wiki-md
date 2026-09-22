<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [affine algebraic group](../../../../../linear-algebraic-group.md) is a [linearly reductive algebraic group](../../../../../linearly-reductive-algebraic-group.md) if every finite-dimensional [rational representation](../../../../../rational-representation.md) is completely reducible; equivalently the functor of invariants is exact. It is a [geometrically reductive algebraic group](../../../../../geometrically-reductive-algebraic-group.md) if, whenever $0\ne v\in V^G$, there is a homogeneous invariant polynomial $F\in k[V]^G$ of positive degree with $F(v)\ne0$. Linear reductivity permits degree one; geometric reductivity allows higher degree.

Over the [algebraically closed field](../../../../../algebraically-closed-field.md), an [algebraic torus](../../../../../algebraic-torus.md) is $T\cong(\mathbb G_m)^r$. Its [coordinate ring](../../../../../coordinate-ring.md) is the Laurent [polynomial ring](../../../../../polynomial-ring.md). A rational action writes the coaction of a vector as a finite sum $\delta(v)=\sum_\chi v_\chi\otimes t^\chi$. The coaction identity and linear independence of Laurent monomials give $\delta(v_\chi)=v_\chi\otimes t^\chi$ and $v=\sum_\chi v_\chi$. Thus

$$
\boxed{V=\bigoplus_{\chi\in\mathbb Z^r}V_\chi.}
$$

Each [weight space](../../../../../weight-space.md) has scalar action, so any vector-space complement within each [weight space](../../../../../weight-space.md) is invariant. This proves complete reducibility, and hence **tori are linearly reductive in every characteristic**. The argument uses characters themselves, not their [Lie algebra](../../../../../lie-algebra-split.md) differentials, which could coincide modulo $p$.

We now prove geometric reductivity of $G=SL_2(k)$ by [determinant separation for positive-characteristic SL2](../../../../../determinant-separation-for-positive-characteristic-sl2.md). Fix a rational $G$-module $V$ and a nonzero fixed vector $v$. For the diagonal torus, choose a weight-zero functional $l\in V^*$ with $l(v)=1$, using the torus decomposition just proved. Define matrix coefficients

$$
\Phi(w)(g)=l(g^{-1}w).
$$

These are [regular functions](../../../../../regular-function.md) on $G$, and $\Phi(hw)(g)=\Phi(w)(h^{-1}g)$ makes $\Phi$ equivariant for left translations. Moreover $\Phi(w)(gt)=\Phi(w)(g)$ because $l$ is torus-invariant. Thus $\Phi$ maps into $k[G]^T$ for the right torus action, and $\Phi(v)=1$.

Write a matrix's two columns as $a=(a_0,a_1)$ and $b=(b_0,b_1)$, with $\Delta=a_0b_1-a_1b_0=1$. Right torus multiplication scales these columns by $t$ and $t^{-1}$. Every right-torus-invariant [regular function](../../../../../regular-function.md) has a weight-zero polynomial lift, hence a sum of polynomials of bidegrees $(j,j)$ in $(a,b)$. To see that a weight-zero lift exists, take any lift and retain its zero-weight component; the ideal $(\Delta-1)$ is torus-stable and the quotient map preserves weights. Multiply each piece by $\Delta^{n-j}$ to put the entire sum in bidegree $(n,n)$ without changing its restriction to $G$.

Let $P_n$ be the space of degree-$n$ polynomials in one column. Restriction gives an injective equivariant map $P_n\otimes P_n\to k[G]^T$. Indeed if a bidegree-$(n,n)$ polynomial vanishes on [determinant](../../../../../determinant.md)-one matrices, scale the first column of any invertible matrix to make its [determinant](../../../../../determinant.md) one. Homogeneity then makes the polynomial vanish on every invertible matrix, a dense open subset, so it is zero. Denote the image by $R_n$. These spaces increase because multiplication by $\Delta$ realizes $R_{n-1}\subset R_n$, and their union is $k[G]^T$. The finite-dimensional image $\Phi(V)$ therefore lies in one $R_n$, and in any sufficiently larger filtration piece.

Choose $q=p^s$ with $q-1$ at least that bound, and set $n=q-1$. The identity $(1+z)^q=1+z^q$ in characteristic $p$ gives

$$
\binom{q-1}{j}=(-1)^j\ne0\quad\text{in }k,\qquad0\le j\le q-1.
$$

The [invariant tensor](../../../../../invariant-tensor.md)

$$
D=\Delta^n=\sum_{j=0}^n(-1)^j\binom nj\,a_0^{n-j}a_1^j b_0^j b_1^{n-j}\in P_n\otimes P_n
$$

therefore defines an invertible equivariant [linear map](../../../../../linear-map.md) $D:P_n^*\to P_n$: its matrix is anti-diagonal with all entries nonzero. Interpret any tensor $B\in P_n\otimes P_n$ as a map $P_n^*\to P_n$ and send it to $BD^{-1}\in\operatorname{End}(P_n)$. Equivariance of $D$ makes this identification intertwine the diagonal tensor action with conjugation on endomorphisms. Crucially, $D$ restricts to the constant function $1$ on $G$, and is sent to the identity endomorphism.

Under the resulting equivariant [linear map](../../../../../linear-map.md) $V\to\operatorname{End}(P_n)$, the vector $v$ is sent to $I$. Since $\dim P_n=n+1=q$, the endomorphism [determinant](../../../../../determinant.md) is a [homogeneous polynomial](../../../../../homogeneous-polynomial.md) of positive degree $q$, invariant under conjugation. Pull it back to $V$. The resulting polynomial satisfies

$$
\boxed{F\in k[V]^{SL_2(k)},\qquad\deg F=q=p^s>0,\qquad F(v)=\det I=1.}
$$

This constructs the required invariant for every fixed nonzero vector and proves **$SL_2(k)$ is geometrically reductive**, including [characteristic two](../../../../../characteristic-two.md). No averaging by a group order or division by $q$ is used; those operations would fail in the field's characteristic.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
