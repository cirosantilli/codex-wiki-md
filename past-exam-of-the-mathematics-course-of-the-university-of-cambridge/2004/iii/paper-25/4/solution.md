<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [central simple algebra](../../../../../central-simple-algebra.md) over $K$ is a finite-dimensional associative unital $K$-algebra $A$ with no nonzero proper two-sided [ideals](../../../../../ideal.md) and center exactly $K$. Its dimension is a square, $\dim_KA=n^2$. The [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) writes it as $M_r(D)$ for a uniquely determined [central division algebra](../../../../../central-division-algebra.md) $D$ up to isomorphism. One obtains this structure by taking a minimal left [ideal](../../../../../ideal.md) and its commuting division endomorphism ring; the simple algebra acts as all endomorphisms over that ring. Over a suitable finite [splitting field](../../../../../splitting-field.md) it becomes a full [matrix algebra](../../../../../matrix-algebra.md).

The [Brauer group](../../../../../brauer-group.md) identifies two [central simple algebras](../../../../../central-simple-algebra.md) if their division-algebra parts agree, equivalently if tensoring each with suitable [matrix algebras](../../../../../matrix-algebra.md) makes them isomorphic. The product is [tensor product](../../../../../tensor-product.md), the identity is the class of $K$, and the inverse of $[A]$ is $[A^{\rm op}]$. Indeed

$$
A\otimes_KA^{\rm op}\longrightarrow\operatorname{End}_K(A),\qquad
(a\otimes b)(x)=axb
$$

is an isomorphism for a [central simple algebra](../../../../../central-simple-algebra.md), so the product class is split. This also explains why matrix size is irrelevant to the [Brauer class](../../../../../brauer-class.md). The order of the class is its period, while the degree of its division-algebra representative is its index; these are different notions in general.

For the [cyclic algebra](../../../../../cyclic-algebra.md) construction, take a cyclic extension $L/K$ of degree $m$, a generator $\sigma$ and $a\in K^*$. Set

$$
A=(L/K,\sigma,a)=\bigoplus_{i=0}^{m-1}Lu^i,
\qquad u\ell=\sigma(\ell)u,\qquad u^m=a.
$$

The multiplication is obtained by moving coefficients past $u$ and replacing every $u^m$ by $a$. It is associative: reducing a product of three monomials gives the same total exponent, the same power of $a$ and the same iterated automorphisms in either order. The scalar $a$ is fixed by $\sigma$ and $\sigma^m=1$, so reduction is consistent.

An element commuting with every $\ell\in L$ has only its $u^0$ coefficient nonzero, because $\sigma^i\ne1$ for $0<i<m$. Commuting with $u$ then forces that coefficient into $K$, proving that the center is $K$. To prove simplicity, choose a nonzero element of a nonzero [ideal](../../../../../ideal.md) with the fewest nonzero monomial coefficients. Since $u$ is invertible and each nonzero coefficient in $L$ is invertible, normalize one term to be the constant one. If another term remains, its automorphism differs from the identity; commuting with a suitable element of $L$ eliminates the constant term but not that other term. This gives a shorter nonzero element, a contradiction. The minimal element is therefore a unit, and the [ideal](../../../../../ideal.md) is all of $A$. Thus $A$ is central simple of dimension $m^2$.

It splits over $L$. For example, over $L$ represent $\ell$ by the diagonal matrix with entries $\ell,\sigma(\ell),\ldots,\sigma^{m-1}(\ell)$, and let $u$ shift the standard basis down one place, sending the first vector to $a$ times the last. These matrices satisfy the defining relations. A primitive element of the separable extension $L/K$ has distinct conjugates; the Vandermonde matrix of their powers is invertible. Thus the diagonal images span all diagonal matrices after scalar extension to $L$. Multiplying the diagonal matrix units by powers of the shift gives every matrix unit, proving $A\otimes_KL\cong M_m(L)$.

The particularly useful splitting criterion is

$$
\boxed{(L/K,\sigma,a)\text{ is split}\iff a\in N_{L/K}L^*.}
$$

If $a=N(b)$, let the algebra act on $L$ by multiplication for $\ell$ and by the semilinear operator $b\sigma$ for $u$. Its $m$th power is multiplication by $N(b)=a$, so this gives an isomorphism with $\operatorname{End}_K(L)$, by simplicity and dimension. Conversely, a split algebra acts on an $m$-dimensional $K$-space $V$. Restriction to the subfield $L$ makes $V$ one-dimensional over $L$, and $u$ is a nonzero $\sigma$-semilinear operator. In an $L$-basis it is $b\sigma$, so $u^m=a$ forces $a=N(b)$. More generally the relative [Brauer group](../../../../../brauer-group.md) split by a cyclic $L/K$ is $K^*/N_{L/K}L^*$, with multiplication of parameters corresponding to addition of classes.

For a [finite field](../../../../../finite-field.md), a finite [division algebra](../../../../../division-algebra.md) is commutative by Wedderburn's little theorem. Therefore every [central simple algebra](../../../../../central-simple-algebra.md) is a [matrix algebra](../../../../../matrix-algebra.md) and $\boxed{\operatorname{Br}(\mathbb F_q)=0}$. The cyclic-algebra viewpoint gives the same conclusion for cyclic classes because the norm between [finite fields](../../../../../finite-field.md) is surjective on their cyclic multiplicative groups.

For a nonarchimedean local field, the [local Brauer invariant](../../../../../local-brauer-invariant.md) gives

$$
\boxed{\operatorname{Br}(K)\cong\mathbb Q/\mathbb Z.}
$$

An unramified cyclic extension of degree $m$, with [arithmetic Frobenius](../../../../../frobenius-automorphism.md) generator, gives invariant $v_K(a)/m$ to its [cyclic algebra](../../../../../cyclic-algebra.md). Question 2 shows that all units are norms; norm [valuations](../../../../../valuation.md) are multiples of $m$. Thus the relative classes are $\mathbb Z/m\mathbb Z$, represented by powers of a [uniformizer](../../../../../uniformizer.md). Allowing all $m$ realizes all invariants. At the infinite local fields, $\operatorname{Br}(\mathbb C)=0$, while $\operatorname{Br}(\mathbb R)\cong\mathbb Z/2\mathbb Z$, with the nonzero class represented by Hamilton's quaternions and invariant $1/2$.

For a [number field](../../../../../number-field.md), the [Albert-Brauer-Hasse-Noether theorem](../../../../../albert-brauer-hasse-noether-theorem.md) supplies the exact sequence

$$
0\longrightarrow\operatorname{Br}(K)
\longrightarrow\bigoplus_v\operatorname{Br}(K_v)
\xrightarrow{\ \sum_v\operatorname{inv}_v\ }\mathbb Q/\mathbb Z
\longrightarrow0.
$$

Hence a global algebra is determined by its finitely many nonzero local invariants, whose sum is zero; it is split precisely when all its local classes vanish. Every [division algebra](../../../../../division-algebra.md) over a [number field](../../../../../number-field.md) is cyclic, so [cyclic algebras](../../../../../cyclic-algebra.md) provide representatives for the global classes as well. Their norm parameters translate splitting into local norm conditions and the reciprocity constraint on the sum of invariants. The local invariant theorem, Wedderburn's little theorem and the global invariant theorem are the standard structural results used here; their role in the requested computation is explicit.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
