<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Brauer group](../../../../../brauer-group.md) of a [field](../../../../../field.md) consists of [equivalence classes](../../../../../equivalence-class.md) of [central simple algebras](../../../../../central-simple-algebra.md), with addition induced by [tensor product](../../../../../tensor-product.md), zero represented by [matrix algebras](../../../../../matrix-algebra.md), and inverse represented by the [opposite algebra](../../../../../opposite-algebra.md). Localization sends a global algebra to its scalar extensions at the completions. For a non-Archimedean completion of a [number field](../../../../../number-field.md), the [local Brauer invariant](../../../../../local-brauer-invariant.md) is an [isomorphism](../../../../../isomorphism.md)

$$
\operatorname{inv}_v:\operatorname{Br}(K_v)\xrightarrow{\sim}\mathbb Q/\mathbb Z.
$$

Normalize it so that an unramified [cyclic algebra](../../../../../cyclic-algebra.md) of degree $m$, with [arithmetic Frobenius](../../../../../frobenius-automorphism.md) generator and parameter $a$, has invariant $v(a)/m$. For a real completion, $\operatorname{Br}(\mathbb R)=\mathbb Z/2$ with the Hamilton [quaternion algebra](../../../../../quaternion-algebra.md) mapped to $1/2$; for a complex completion the [Brauer group](../../../../../brauer-group.md) is zero.

The global computation is the [exact sequence](../../../../../exact-sequence.md) in the [Albert-Brauer-Hasse-Noether theorem](../../../../../albert-brauer-hasse-noether-theorem.md):

$$
\boxed{0\longrightarrow\operatorname{Br}(K)
\longrightarrow\bigoplus_v\operatorname{Br}(K_v)
\xrightarrow{\sum_v\operatorname{inv}_v}\mathbb Q/\mathbb Z
\longrightarrow0.}
$$

Thus a global Brauer class is determined uniquely by a finite-support family of local invariants. Such a family occurs if and only if its sum is zero; at real places the only allowed entries are $0,1/2$, and at complex places the entry is zero. [Injectivity](../../../../../injective-function.md) is a local-global splitting principle; the middle exactness is the reciprocity constraint; [surjectivity](../../../../../surjective-function.md) of the sum follows already from any one finite local summand. These are separate assertions, not merely different descriptions of the sum formula.

For an explicit [group](../../../../../group-split.md) description, choose one finite place $v_0$. Assign arbitrary finite-support invariants at all other finite places and arbitrary allowed invariants at the real places, then set the invariant at $v_0$ equal to minus their sum. This gives

$$
\operatorname{Br}(K)\cong
\left(\bigoplus_{v\ {
m finite},\ v\ne v_0}\mathbb Q/\mathbb Z\right)
\oplus(\mathbb Z/2)^{r_1}.
$$

The description by the entire invariant family is canonical; this displayed elimination of one coordinate depends on the choice of $v_0$.

The connection with [Artin reciprocity](../../../../../artin-reciprocity-law.md) is especially transparent for [cyclic algebras](../../../../../cyclic-algebra.md). Let $\chi:\operatorname{Gal}(L/K)\hookrightarrow\mathbb Q/\mathbb Z$ describe a cyclic extension, with $\chi(\sigma)=1/n$. Write $(\chi,a)$ for the class of $(L/K,\sigma,a)$. The local reciprocity pairing is

$$
\operatorname{inv}_v(\chi_v,a_v)
=\chi_v\bigl(\operatorname{Art}_{K_v}(a_v)\bigr).
$$

It follows from the [local fundamental class](../../../../../local-fundamental-class.md) construction of the [Local Artin map](../../../../../local-artin-map.md); on an unramified character it is precisely the normalization $v(a_v)/n$. The [group kernel](../../../../../kernel-of-a-group-homomorphism.md) in the parameter is the local norm [group](../../../../../group-split.md), and restriction/corestriction give the norm compatibility of this pairing.

For a principal parameter $a\in K^\times$, the zero-sum identity for its global [cyclic algebra](../../../../../cyclic-algebra.md) therefore reads

$$
\sum_v\chi_v(\operatorname{Art}_{K_v}(a))=0.
$$

On the other hand the idelic [Artin reciprocity law](../../../../../artin-reciprocity-law.md) is

$$
\prod_v\operatorname{Art}_{L/K,v}(a)=1
\quad(a\in K^\times),
$$

and evaluating this product by $\chi$ gives exactly that zero-sum identity. Conversely, testing every cyclic character of a finite abelian [Galois group](../../../../../galois-group.md) separates its elements, so the zero-sum identities for [cyclic algebras](../../../../../cyclic-algebra.md) imply this principal-idele reciprocity law for every finite [abelian extension](../../../../../abelian-extension.md). At almost all places a unit and an unramified character pair trivially, so the sums and products are finite.

The full idelic statement identifies the [group kernel](../../../../../kernel-of-a-group-homomorphism.md) as $K^\times N_{L/K}J_L$ and induces $J_K/(K^\times N_{L/K}J_L)\cong\operatorname{Gal}(L/K)$. It explains why the local norm-residue pairings must glue globally. The global Brauer theorem supplies, in addition, the [injectivity](../../../../../injective-function.md) and realization statements needed to compute all algebra classes; the principal-product identity alone would not prove those statements. For [cyclic algebras](../../../../../cyclic-algebra.md) its [injectivity](../../../../../injective-function.md) yields the [Hasse norm theorem](../../../../../hasse-norm-theorem.md), as in Question 3. In degree two, an invariant is either zero or $1/2$, so the zero-sum law becomes the [Hilbert reciprocity law](../../../../../hilbert-reciprocity-law.md) $\prod_v(a,b)_v=1$. For example, a [quaternion algebra](../../../../../quaternion-algebra.md) over $\mathbb Q$ can be ramified at precisely a prescribed [finite set](../../../../../finite-set.md) of places, including possibly the real place, if and only if that set has even cardinality; the invariants uniquely determine its Brauer class. This illustrates how arithmetic reciprocity becomes a concrete constraint on global algebra structure.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
