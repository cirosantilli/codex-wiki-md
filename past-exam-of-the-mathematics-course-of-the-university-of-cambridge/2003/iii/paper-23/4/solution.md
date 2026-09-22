<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [central simple algebra](../../../../../central-simple-algebra.md) over $K$ is a finite-dimensional associative $K$-[algebra](../../../../../algebra-split.md) with no nonzero proper two-sided [ideals](../../../../../ideal.md) and with center $K$. The [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) writes it uniquely as $M_r(D)$ with $D$ a central [division algebra](../../../../../division-algebra.md). After a finite separable [splitting field](../../../../../splitting-field.md) extension it becomes $M_d$, so its dimension is $d^2$, and $d$ is its [degree of a central simple algebra](../../../../../degree-of-a-central-simple-algebra.md). Passing from $D$ to a [matrix algebra](../../../../../matrix-algebra.md) over $D$ does not change its [Brauer class](../../../../../brauer-class.md).

The [Brauer group](../../../../../brauer-group.md) consists of these classes, with product induced by [tensor product](../../../../../tensor-product.md). Extending to a common [splitting field](../../../../../splitting-field.md) shows that a [tensor product of central simple algebras](../../../../../tensor-product-of-central-simple-algebras.md) is again central simple; its two-sided [ideals](../../../../../ideal.md) and center descend from the corresponding full [matrix algebra](../../../../../matrix-algebra.md). The neutral class is $[K]$, and the inverse of $[A]$ is $[A^{\mathrm{op}}]$, because

$$
A\otimes_K A^{\mathrm{op}}\cong\operatorname{End}_K(A),\qquad a\otimes b\mapsto(x\mapsto axb).
$$

The displayed map becomes the standard isomorphism for matrices over a [splitting field](../../../../../splitting-field.md), so it is already an isomorphism over $K$. Thus [Brauer classes](../../../../../brauer-class.md) measure precisely the obstruction to being a split [matrix algebra](../../../../../matrix-algebra.md).

An explicit family is supplied by [cyclic algebras](../../../../../cyclic-algebra.md). Let $L/K$ be cyclic of degree $n$, with generator $\sigma$, and let $a\in K^\times$. Define

$$
A=(L/K,\sigma,a)=\bigoplus_{i=0}^{n-1}Lu^i,\qquad ux=\sigma(x)u,\qquad u^n=a.
$$

This is an associative [algebra](../../../../../algebra-split.md): form the skew polynomial ring with relation $ux=\sigma(x)u$ and quotient by the central relation $u^n-a$. Reduction of powers gives the displayed $n^2$-dimensional $K$-[basis](../../../../../basis.md). An element commuting with every $x\in L$ has no $u^i$ coefficient for $i\ne0$, since $\sigma^i$ is not the identity. Commuting also with $u$ forces the remaining coefficient into $K$. Hence the center is $K$.

Here is an explicit splitting construction. On $L^n$, with [basis](../../../../../basis.md) $e_0,\ldots,e_{n-1}$, put

$$
D(x)e_j=\sigma^j(x)e_j,\qquad Ue_j=e_{j-1}\ (j\ge1),\qquad Ue_0=a e_{n-1}.
$$

Then $UD(x)=D(\sigma x)U$ and $U^n=aI$. After extending scalars to $L$, the separable decomposition $L\otimes_KL\cong\prod_{j=0}^{n-1}L$ supplies all diagonal matrices, and their products with powers of $U$ supply all [matrix units](../../../../../matrix-unit.md). Therefore

$$
A\otimes_KL\cong M_n(L).
$$

Any nonzero proper two-sided [ideal](../../../../../ideal.md) of $A$ would extend to one of $M_n(L)$, which is impossible. Thus this construction really gives a [central simple algebra](../../../../../central-simple-algebra.md), with [splitting field](../../../../../splitting-field.md) $L$.

Its central arithmetic feature is the [splitting criterion for a cyclic algebra](../../../../../splitting-criterion-for-a-cyclic-algebra.md):

$$
\boxed{(L/K,\sigma,a)\text{ splits}\iff a\in N_{L/K}L^\times.}
$$

If $a=Nc$, let $L$ act by multiplication on the $K$-[vector space](../../../../../vector-space-split.md) $L$, and let $u$ act as $c\sigma$. Its nth power is multiplication by $Nc=a$, so this gives a representation $A\to\operatorname{End}_K(L)$. It is injective by simplicity and an isomorphism by equal dimension. Conversely, if $A\cong\operatorname{End}_K(V)$ with $\dim_K V=n$, its embedded field $L$ makes $V$ one-dimensional over $L$. The relation for $u$ says that $u$ is $\sigma$-semilinear. In an $L$-[basis](../../../../../basis.md) it must have the form $c\sigma$, whose nth power is $Nc$. The relation $u^n=a$ forces $a=Nc$.

More generally the [crossed-product algebra of a Galois extension](../../../../../crossed-product-algebra-of-a-galois-extension.md) attaches an [algebra](../../../../../algebra-split.md) to a multiplicative two-cocycle. Changing the cocycle by a coboundary rescales its basis and preserves the [Brauer class](../../../../../brauer-class.md). Descent of a split [matrix algebra](../../../../../matrix-algebra.md) identifies

$$
\ker\bigl(\operatorname{Br}(K)\to\operatorname{Br}(L)\bigr)\cong H^2(\operatorname{Gal}(L/K),L^\times).
$$

For cyclic $L/K$, cyclic [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) identifies this second [cohomology group](../../../../../cohomology-group.md) with $K^\times/NL^\times$. In a crossed product, rescale successive cyclic basis elements to powers of a single $u$; the remaining datum is $u^n=a$, changed by a [field norm](../../../../../field-norm.md) when $u$ is rescaled. This explains why [cyclic algebras](../../../../../cyclic-algebra.md) give every class split by a cyclic extension, and why multiplication of their parameters is addition of their [Brauer classes](../../../../../brauer-class.md).

For a [finite field](../../../../../finite-field.md) $K=\mathbb F_q$, every finite [splitting field](../../../../../splitting-field.md) $L=\mathbb F_{q^n}$ is cyclic over $K$. The [field norm](../../../../../field-norm.md) is the power map $x\mapsto x^{(q^n-1)/(q-1)}$ on its cyclic multiplicative [group](../../../../../group-split.md), and is onto $\mathbb F_q^\times$. Thus every relative [Brauer class](../../../../../brauer-class.md) is zero, and every [central simple algebra](../../../../../central-simple-algebra.md) has zero class:

$$
\boxed{\operatorname{Br}(\mathbb F_q)=0.}
$$

For a non-Archimedean [local field](../../../../../local-field.md) $K$, the valuation classification of central [division algebras](../../../../../division-algebra.md) shows that every [Brauer class](../../../../../brauer-class.md) splits over a finite [unramified extension](../../../../../unramified-extension.md). For the degree-$n$ [unramified extension](../../../../../unramified-extension.md) $L/K$ with arithmetic [Frobenius](../../../../../frobenius-automorphism.md) $\sigma$, units are norms and norm [valuations](../../../../../valuation.md) are multiples of $n$. Hence the cyclic relative [Brauer group](../../../../../brauer-group.md) is $\mathbb Z/n\mathbb Z$, represented by $a=\pi^r$. The compatible [local Brauer invariant](../../../../../local-brauer-invariant.md) is

$$
\operatorname{inv}_K[(L/K,\sigma,a)]=\frac{v_K(a)}n\pmod{\mathbb Z}.
$$

The union over all $n$ gives

$$
\boxed{\operatorname{Br}(K)\cong\mathbb Q/\mathbb Z.}
$$

A class with invariant $r/n$ in lowest terms has a central [division algebra](../../../../../division-algebra.md) representative of [degree of a central simple algebra](../../../../../degree-of-a-central-simple-algebra.md) $n$. This is the local valuation classification used above; the explicit [cyclic algebras](../../../../../cyclic-algebra.md) exhibit all of its invariants. At the Archimedean places, $\operatorname{Br}(\mathbb C)=0$, while $\operatorname{Br}(\mathbb R)=\mathbb Z/2\mathbb Z$: its nontrivial class is the [quaternion algebra](../../../../../quaternion-algebra.md) $(\mathbb C/\mathbb R,\text{conjugation},-1)$, since complex [norms](../../../../../norm.md) are positive.

For a [number field](../../../../../number-field.md), the [Albert-Brauer-Hasse-Noether theorem](../../../../../albert-brauer-hasse-noether-theorem.md) describes the [Brauer group](../../../../../brauer-group.md) by the exact sequence

$$
0\longrightarrow\operatorname{Br}(K)\longrightarrow\bigoplus_v\operatorname{Br}(K_v)\xrightarrow{\ \sum_v\operatorname{inv}_v\ }\mathbb Q/\mathbb Z\longrightarrow0.
$$

Thus its classes are exactly finite-support families of local invariants with sum zero; real invariants are $0$ or $1/2$ and complex invariants are zero. Every global [Brauer class](../../../../../brauer-class.md) has a cyclic splitting extension, so [cyclic algebras](../../../../../cyclic-algebra.md) also realize all global classes. If $\chi(\sigma)=1/n$, their local invariants are $\chi_v(\operatorname{rec}_{K_v}(a))$, with $\chi_v$ restricted to the local decomposition subgroup. The sum-zero relation for a principal parameter is the invariant form of [Artin reciprocity](../../../../../artin-reciprocity-law.md). Injectivity supplies the local-to-global splitting test, which yields the [Hasse norm theorem](../../../../../hasse-norm-theorem.md) for cyclic extensions as explained in the preceding solution. Here the local valuation classification and the global invariant theorem are the structural theorems used to describe the [Brauer groups](../../../../../brauer-group.md); the construction and norm-splitting calculation have been proved explicitly.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
