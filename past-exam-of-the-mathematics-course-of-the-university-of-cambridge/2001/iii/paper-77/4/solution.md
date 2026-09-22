<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\operatorname{Par}$ be the set of finite weakly decreasing sequences of positive integers, together with the empty sequence; equivalently pad them indefinitely with zeros. The size is $|\lambda|=\sum_i\lambda_i$, the length counts positive parts, and $\operatorname{Par}(n)$ consists of size-$n$ [integer partitions](../../../../../integer-partition.md). Their [Young diagrams](../../../../../young-diagram.md) have cells $(i,j)$ with $1\le j\le\lambda_i$.

Diagram containment is the [partial order](../../../../../partially-ordered-set.md) $\mu\subseteq\lambda$ defined by $\mu_i\le\lambda_i$ for every $i$. Componentwise minimum and maximum give its meet and join, so this is [Young's lattice](../../../../../young-s-lattice.md). Its covers add one cell. On $\operatorname{Par}(n)$ the [dominance order on partitions](../../../../../dominance-order-on-partitions.md) is

$$
\mu\le\lambda\iff
\sum_{i=1}^r\mu_i\le\sum_{i=1}^r\lambda_i
\quad\text{for every }r.
$$

It is not diagram containment: distinct equal-size diagrams cannot contain one another. For the [reverse lexicographic order on partitions](../../../../../reverse-lexicographic-order-on-partitions.md), use the descending-dictionary convention: $\lambda<_R\mu$ when the first unequal pair of parts has $\lambda_i>\mu_i$. Thus for size four its increasing list is $(4),(3,1),(2,2),(2,1,1),(1,1,1,1)$. This is a total order opposite to increasing [dictionary order on integer partitions](../../../../../dictionary-order-on-integer-partitions.md), not the last-differing-exponent order on [polynomial](../../../../../polynomial-split.md) [monomials](../../../../../monomial.md).

Define the [elementary symmetric functions](../../../../../elementary-symmetric-polynomial.md) and [complete homogeneous symmetric functions](../../../../../complete-homogeneous-symmetric-polynomial.md) by

$$
e_r=\sum_{i_1<\cdots<i_r}x_{i_1}\cdots x_{i_r},
\qquad
h_r=\sum_{i_1\le\cdots\le i_r}x_{i_1}\cdots x_{i_r},
\qquad e_0=h_0=1.
$$

For a partition, write $e_\lambda=\prod_i e_{\lambda_i}$ and $h_\lambda=\prod_i h_{\lambda_i}$. The [monomial symmetric function](../../../../../monomial-symmetric-function.md) $m_\lambda$ sums each [monomial](../../../../../monomial.md) with exponent multiset $\lambda$ once.

Here is a proof of the [Fundamental theorem of symmetric polynomials](../../../../../fundamental-theorem-of-symmetric-polynomials.md) sufficient for the stable algebra. In $N$ variables, the lexicographically largest [monomial](../../../../../monomial.md) of a symmetric homogeneous [polynomial](../../../../../polynomial-split.md) has exponents $\lambda_1\ge\cdots\ge\lambda_N\ge0$. Otherwise exchanging an inverted pair of variables produces a larger [monomial](../../../../../monomial.md) with the same coefficient. The [polynomial](../../../../../polynomial-split.md)

$$
e_1^{\lambda_1-\lambda_2}e_2^{\lambda_2-\lambda_3}
\cdots e_N^{\lambda_N}
$$

has that [monomial](../../../../../monomial.md) as its largest one, with coefficient one. Subtract a suitable multiple and continue; there are only finitely many [monomials](../../../../../monomial.md) of the fixed degree, so the procedure terminates and proves generation. Distinct products $e_1^{a_1}\cdots e_N^{a_N}$ have distinct largest exponents $(a_1+\cdots+a_N,a_2+\cdots+a_N,\ldots,a_N)$. The largest such [monomial](../../../../../monomial.md) in any nonzero [polynomial](../../../../../polynomial-split.md) relation cannot cancel, proving [algebraic independence](../../../../../algebraic-independence.md). Stabilizing in each degree, where only $e_r$ with $r$ no greater than that degree can occur, gives

$$
\boxed{\Lambda=\mathbb Q[e_1,e_2,\ldots]\quad\text{as a polynomial algebra}.}
$$

The two generating functions satisfy

$$
E(t)=\sum_{r\ge0}e_rt^r=\prod_i(1+x_it),\qquad
H(t)=\sum_{r\ge0}h_rt^r=\prod_i(1-x_it)^{-1},
\qquad E(-t)H(t)=1.
$$

Since the $e_r$ freely generate, there is a unique [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md) $\omega$ with $\omega(e_r)=h_r$. Apply it to the last identity:

$$
H(-t)\omega(H(t))=1,\qquad \omega(H(t))=E(t).
$$

It follows that $\omega(h_r)=e_r$ and $\omega^2(e_r)=e_r$. Hence the [symmetric-function involution](../../../../../symmetric-function-involution.md) is an involutory automorphism, and

$$
\boxed{\omega(e_\lambda)=h_\lambda,\qquad\omega(h_\lambda)=e_\lambda.}
$$

For the forgotten coefficients, it is useful to derive the required duality explicitly. Put $p_r=\sum_i x_i^r$. The logarithmic generating-function identities give

$$
H(t)=\exp\!\left(\sum_{r\ge1}\frac{p_rt^r}{r}\right),
\qquad E(t)=\exp\!\left(\sum_{r\ge1}\frac{(-1)^{r-1}p_rt^r}{r}\right),
\qquad \omega(p_r)=(-1)^{r-1}p_r.
$$

The transition $p_r=rh_r+$ a [polynomial](../../../../../polynomial-split.md) in lower-index $h$'s is triangular and invertible over $\mathbb Q$, so the $p_r$ are also free generators and $p_\lambda$ is a [basis](../../../../../basis.md). Define the [Hall inner product of symmetric functions](../../../../../hall-inner-product-of-symmetric-functions.md) by

$$
\langle p_\lambda,p_\mu\rangle=\delta_{\lambda\mu}z_\lambda,
\qquad
z_\lambda=\prod_{r\ge1}r^{m_r(\lambda)}m_r(\lambda)!.
$$

Expand the same formal kernel in two ways:

$$
K(x,y)=\prod_{i,j}(1-x_iy_j)^{-1}
=\sum_\lambda h_\lambda(x)m_\lambda(y)
=\exp\!\left(\sum_{r\ge1}\frac{p_r(x)p_r(y)}r\right)
=\sum_\lambda\frac{p_\lambda(x)p_\lambda(y)}{z_\lambda}.
$$

The last expansion is a reproducing kernel for this [inner product](../../../../../inner-product.md). Comparing it with the $h,m$ expansion gives $\langle h_\lambda,m_\mu\rangle=\delta_{\lambda\mu}$. One can see this without assuming any Schur orthogonality: pair either kernel with $h_\nu(y)$; the reproducing property gives $h_\nu(x)$, and uniqueness of its $h$ expansion proves the duality. The signs in $\omega(p_\lambda)$ show that $\omega$ is an isometry; together with $\omega^2=1$ this makes it self-adjoint.

If $n=|\lambda|$ and $\ell=\ell(\lambda)$, define the [forgotten symmetric function](../../../../../forgotten-symmetric-function.md) $f_\lambda=(-1)^{n-\ell}\omega(m_\lambda)$. Its [monomial](../../../../../monomial.md) coefficient is consequently

$$
a_{\lambda\mu}
=\langle f_\lambda,h_\mu\rangle
=(-1)^{n-\ell}\langle m_\lambda,e_\mu\rangle
=(-1)^{n-\ell}[h_\lambda]e_\mu.
$$

It remains to compute this coefficient rather than merely invoke duality. Expand the formal inverse $E(t)=H(-t)^{-1}$ as a [geometric series](../../../../../geometric-series.md) in $H(-t)-1$:

$$
e_r=\sum_{\substack{\beta=(\beta_1,\ldots,\beta_k)\\
\beta_i>0,\ |\beta|=r}}
(-1)^{r-k}h_{\beta_1}\cdots h_{\beta_k}.
$$

In $e_\mu=\prod_j e_{\mu_j}$, choose a positive composition of each $\mu_j$. A term is $h_\lambda$ precisely when the concatenated list is a distinct rearrangement $\alpha$ of the parts of $\lambda$. Its boundaries at the end of each chosen composition are exactly the prescribed prefix sums of $\mu$. Conversely such a rearrangement uniquely determines the compositions by cutting at those prefix sums. Every one of its signs is $(-1)^{\sum\mu_j-\ell}=(-1)^{n-\ell}$, canceled by the prefactor in $a_{\lambda\mu}$. Thus

$$
\boxed{a_{\lambda\mu}
=\#\left\{\text{distinct rearrangements }\alpha\text{ of }\lambda:
\{\mu_1+\cdots+\mu_j\}_j\subseteq
\{\alpha_1+\cdots+\alpha_i\}_i\right\}.}
$$

Identical parts are not artificially distinguished. For example $f_{(2,1)}=m_{(2,1)}+2m_{(3)}$: only the order $(2,1)$ refines $(2,1)$, while both orders refine the single block $(3)$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
