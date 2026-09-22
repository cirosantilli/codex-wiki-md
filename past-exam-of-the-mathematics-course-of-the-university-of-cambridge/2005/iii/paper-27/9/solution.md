<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

We give a relative consistency proof: **a model of ZFC yields a model of NFU**. This proves the requested consistency relative to the usual background set theory; it does not claim the optimal, much weaker consistency bound for bare [NFU](../../../../../new-foundations-with-urelements.md).

Recall that [New Foundations with urelements](../../../../../new-foundations-with-urelements.md) has a unary set predicate $S$, atoms without members, extensionality restricted to sets, and comprehension for every [stratified formula](../../../../../stratified-formula.md). Stratification assigns integer types to variables, with equal types at equality and adjacent types at membership. We construct a model of [simple typed set theory with atoms](../../../../../simple-typed-set-theory-with-atoms.md) with a [type-shifting automorphism](../../../../../type-shifting-automorphism.md), then identify its types using that automorphism.

Start with a model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) and a [Skolem expansion](../../../../../skolem-expansion.md) of it. By the [compactness theorem](../../../../../compactness-theorem.md) there is a model $N$ of the same expanded theory with an increasing integer-indexed [order-indiscernible sequence](../../../../../order-indiscernible-sequence.md) of ordinals $\langle c_i:i\in\mathbb Z\rangle$, all above $\omega$. Here is the finite-satisfiability argument. A finite fragment names only finitely many $c_i$ and asks for equal truth values of finitely many formulas on increasing tuples. In the starting model choose an infinite increasing sequence of ordinals above $\omega$. Colour its finite subsets by these truth vectors, successively treating each tuple length. The [Ramsey's theorem](../../../../../ramsey-s-theorem.md) supplies an infinite homogeneous subsequence for the finitely many colours and arities. Its first required number of elements interprets all named $c_i$ and satisfies that fragment. Compactness gives the entire sequence. This argument works for the countable expanded language because each fragment uses only finitely many formulas.

Replace $N$ by the [Skolem hull](../../../../../skolem-hull.md) of the $c_i$. The map

$$
j\bigl(t(c_{i_1},\ldots,c_{i_r})\bigr)=t(c_{i_1+1},\ldots,c_{i_r+1})
$$

is well defined by indiscernibility: equal terms remain equal after shifting their increasing lists of indices. The same argument preserves every formula. Shifting indices backwards gives its inverse, so $j$ is an automorphism of the hull, and $j(c_i)=c_{i+1}>c_i$. The [Skolem hull](../../../../../skolem-hull.md) is elementary by its witness functions. This is a concrete [Ehrenfeucht-Mostowski model](../../../../../ehrenfeucht-mostowski-model.md); it is not an elementary class self-embedding of the actual well-founded universe.

Set $D_i=V_{c_i}^{N}$, interpreted externally as the objects belonging to that internal rank segment, for every integer $i$. At type $i$ declare

$$
S_i(x)\quad\Longleftrightarrow\quad N\models x\subseteq D_{i-1},
$$

and define adjacent-type membership by

$$
x\mathrel{\varepsilon_i}y\quad\Longleftrightarrow\quad
N\models x\in y\quad\text{and}\quad S_{i+1}(y).
$$

The members of a type-$i+1$ set are exactly a subset of $D_i$; a type-$i+1$ atom has no $\varepsilon_i$-members. Every internal subset of $D_i$ is an object of $D_{i+1}$, since $c_{i+1}>c_i$. Extensionality for sets is inherited from $N$. For a typed formula involving finitely many types, restrict its quantifiers to the corresponding internal $D_k$ and express each $S_k$ and $\varepsilon_k$ by the displayed definitions. [Separation](../../../../../axiom-schema-of-specification.md) in $N$ gives the required subset of $D_i$, which represents its comprehension at type $i+1$. This verifies the typed theory even though many higher-type objects are atoms. The automorphism $j$ carries $D_i,S_i,\varepsilon_i$ to the next type.

On domain $D_0$, define $S(x)=S_0(x)$ and

$$
x\mathrel E y\quad\Longleftrightarrow\quad x\mathrel{\varepsilon_0}j(y).
$$

If $S(y)$ is false, $S_1(j(y))$ is false, so $y$ has no $E$-members. For sets $y,z$, equality of their $E$-extensions gives equality of the typed sets $j(y),j(z)$ and hence $y=z$. To check stratified comprehension, translate a variable of type $k$ into $j^k(x)$. The automorphism laws make membership and equality translate exactly. A stratified predicate on a variable of type zero defines a typed subset $B$ of $D_0$, represented by a set at type one. Then $b=j^{-1}(B)\in D_0$ has $E$-extension exactly that predicate. A uniform type shift handles any other type assigned to the comprehended variable. The resulting untyped structure is a model of [NFU](../../../../../new-foundations-with-urelements.md).

## ↑ Ancestors (10)

1. [9](../9.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
