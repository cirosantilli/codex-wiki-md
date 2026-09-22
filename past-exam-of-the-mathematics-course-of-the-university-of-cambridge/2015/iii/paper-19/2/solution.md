<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We use the [James reduced product](../../../../../james-reduced-product.md) theorem and the [Bott–Samelson theorem](../../../../../bott-samelson-theorem.md): if $X$ is a connected based [CW complex](../../../../../cw-complex.md) with free integral [homology](../../../../../homology-split.md), then $JX\to\Omega\Sigma X$ is a weak equivalence, and its induced [Pontryagin ring](../../../../../pontryagin-ring.md) is

$$
H_*(\Omega\Sigma X;\mathbb Z)
\cong T_{\mathbb Z}\bigl(\widetilde H_*(X;\mathbb Z)\bigr).
$$

Here $\Sigma$ is the [reduced suspension](../../../../../reduced-suspension.md), $T$ is the [tensor algebra](../../../../../tensor-algebra.md), and the multiplication is induced by concatenating James words, hence by concatenating loops. Taking $X=S^{2n}$ supplies a single generator $x$ of degree $2n$, so

$$
H_*(\Omega S^{2n+1};\mathbb Z)=\mathbb Z\{1,x,x^2,\ldots\}
$$

is free, with one generator in every degree $2nk$ and zero in the other degrees.

The diagonal makes this a [homology](../../../../../homology-split.md) coalgebra. The generator $x$ is a [primitive homology class](../../../../../primitive-homology-class.md):

$$
\Delta x=x\otimes1+1\otimes x.
$$

There are no nontrivial lower positive degrees in which its reduced diagonal could land. Compatibility of the diagonal with loop multiplication gives

$$
\Delta(x^k)=(x\otimes1+1\otimes x)^k
=\sum_{i=0}^k\binom ki x^i\otimes x^{k-i}.
$$

The degree of $x$ is even, so the two tensor factors commute without a [Koszul sign rule](../../../../../koszul-sign-rule.md).

The [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) has no Ext terms here because [homology](../../../../../homology-split.md) is free. Let $a_k$ be the [cohomology](../../../../../cohomology-split.md) class dual to $x^k$, with $a_0=1$ and $|a_k|=2nk$. The [cup product](../../../../../cup-product.md) is dual to the diagonal, hence

$$
\boxed{a_i a_j=\binom{i+j}{i}a_{i+j}.}
$$

Therefore **the integral [cohomology](../../../../../cohomology-split.md) ring is the [divided power algebra](../../../../../divided-power-algebra.md)**

$$
\boxed{H^*(\Omega S^{2n+1};\mathbb Z)
\cong\Gamma_{\mathbb Z}(a),\qquad |a|=2n.}
$$

Explicitly $H^{2nk}=\mathbb Z a_k$ for $k\geq0$, and all other [cohomology](../../../../../cohomology-split.md) groups vanish. In particular $a_1^k=k!a_k$: over the integers this is not a [polynomial ring](../../../../../polynomial-ring.md) on $a_1$. This is the [integral cohomology of an odd-sphere loop space](../../../../../integral-cohomology-of-an-odd-sphere-loop-space.md).

For the requested [homology](../../../../../homology-split.md) multiplication, use the [homology cross product](../../../../../homology-cross-product.md) followed by concatenation:

$$
\boxed{\alpha*\beta=\mu_*(\alpha\times\beta).}
$$

The constant loop gives the degree-zero unit. Loop concatenation is associative up to [homotopy](../../../../../homotopy.md), which suffices for associativity on [homology](../../../../../homology-split.md); Moore loops can make the space-level operation strictly associative. The [Künneth theorem](../../../../../kunneth-theorem.md) identifies the tensor-product [homology](../../../../../homology-split.md) because its groups are [free abelian groups](../../../../../free-abelian-group.md). The [Bott–Samelson theorem](../../../../../bott-samelson-theorem.md) identifies this product with word multiplication, so $x^i*x^j=x^{i+j}$. **The [Pontryagin ring of an odd-sphere loop space](../../../../../pontryagin-ring-of-an-odd-sphere-loop-space.md) has presentation**

$$
\boxed{H_*(\Omega S^{2n+1};\mathbb Z),*
\cong T_{\mathbb Z}(x)\cong\mathbb Z[x],\qquad |x|=2n.}
$$

With only one generator the [tensor algebra](../../../../../tensor-algebra.md) has the indicated polynomial presentation. The [homology](../../../../../homology-split.md) product and the divided-power [cohomology](../../../../../cohomology-split.md) product are different operations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
