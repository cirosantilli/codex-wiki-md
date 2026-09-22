<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Work in the domain-classifying site of part (ii), with generic domain $K=a_JU$. For finitely presented rings $A$, the object $a_JyA$ is an available stage. Tuples of sections of $K$ are locally represented by tuples of actual elements of $A$, because $U\to a_JU$ is locally surjective and sheafification preserves finite products. It is therefore enough to prove the requested implication on such representatives.

We first note the [empty-cover criterion for the domain-classifying site](../../../../../../empty-cover-criterion-for-the-domain-classifying-site.md): $a_JyB$ is initial if and only if the finitely presented ring $B$ is the zero ring. One direction is the generating empty cover. Conversely, any nonzero ring has a [maximal ideal](../../../../../../maximal-ideal.md) and hence a homomorphism to a field. That field is a set-based integral domain and defines a point of the classifying topos. The inverse image of $a_JyB$ at this point is $\operatorname{Hom}_{\mathrm{Ring}}(B,L)$, which is nonempty for the chosen field $L$. It therefore cannot be the inverse image of an [initial object](../../../../../../initial-object.md). This uses only the ordinary maximal-ideal existence principle externally, not excluded middle in the internal logic.

Suppose $a_1,\ldots,a_n\in A$ represent a tuple lying in the negation of the all-units [subobject](../../../../../../subobject.md). Write $t=a_1\cdots a_n$ and consider the finitely presented [localization of a ring](../../../../../../localization-of-a-ring.md)

$$
B=A[1/t]\cong A[z]/(tz-1).
$$

Every $a_i$ is invertible in $B$, since $(\prod_{j\ne i}a_j)z$ is an inverse. But the pulled-back tuple still lies in the negation of the all-units [subobject](../../../../../../subobject.md). Thus the whole stage $a_JyB$ maps into both that [subobject](../../../../../../subobject.md) and its negation, forcing this stage to be initial. The empty-cover criterion gives $B=0$.

The localization $A[1/t]$ is zero precisely when $t^N=0$ in $A$ for some integer $N\geq1$, by the equality criterion in localization. Repeated use of the generating zero-product covers now gives a covering family

$$
A\longrightarrow A/(a_i)\qquad(1\leq i\leq n).
$$

Indeed, splitting $t^N=t\,t^{N-1}=0$ and inducting first forces $t=0$ locally; splitting the product $a_1\cdots a_n=0$ then forces one $a_i=0$ locally. More formally the two inductions are coherent derivations from the zero-product axiom, so their quotient families belong to the generated topology. The sheaf semantics of disjunction consequently gives

$$
\boxed{\neg\left(\bigwedge_{i=1}^n\exists y_i\,(x_iy_i=1)\right)\ \Longrightarrow\ \bigvee_{i=1}^n(x_i=0).}
$$

This is the [finite-tuple weak-field property of the generic integral domain](../../../../../../finite-tuple-weak-field-property-of-the-generic-integral-domain.md). The argument is intuitionistically valid inside the topos, although its description of the site uses ordinary external set theory. There is no appeal to preservation of negation by an arbitrary geometric inverse image.

For the converse assertion, let $R$ be any internally nontrivial commutative unital ring satisfying the $n=2$ implication. Assume $xy=0$. If $x$ and $y$ were both units, multiplying by their two inverses would give $0=1$, contradicting nontriviality. Therefore

$$
xy=0\quad\Longrightarrow\quad\neg\bigl(\operatorname{Unit}(x)\wedge\operatorname{Unit}(y)\bigr).
$$

The assumed two-variable implication then gives $x=0\vee y=0$. Together with nontriviality this is exactly the internal integral-domain axiom. Hence **a nontrivial ring satisfying the two-variable case is an integral domain**.

For example, the ordinary integral domain $\mathbb Z$ fails the one-variable implication at $2$. This does not contradict the generic result: the displayed implication uses negation and is non-coherent, so it need not survive the inverse image that classifies an arbitrary set-based domain.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Section B](../../section-b.md)
4. [Paper 20](../../../paper-20-split.md)
5. [Iii](../../../split.md)
6. [2014](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
