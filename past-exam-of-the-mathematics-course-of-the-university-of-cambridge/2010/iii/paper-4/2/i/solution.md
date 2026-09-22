<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the [primitive three-cycle criterion](../../../../../../primitive-three-cycle-criterion.md) through supports. First, suppose a [subgroup](../../../../../../subgroup.md) contains $A_U$, the [alternating group](../../../../../../alternating-group.md) on a set $U$ of at least three letters, and a [three-cycle](../../../../../../three-cycle.md) with support $E$ meeting $U$.

If $E$ adds one letter, it has two letters in $U$. The group $A_U$ is transitive on unordered pairs of $U$: for three letters its cyclic action permutes the three pairs, and for at least four letters one can adjust the parity of a [permutation](../../../../../../permutation.md) sending one pair to another while preserving its target pair. Conjugating the new cycle, and using inverses, supplies every [three-cycle](../../../../../../three-cycle.md) on two old letters and the new letter. Together with $A_U$, these generate $A_{U\cup E}$.

If $E$ adds two letters, write its cycle as $\tau=(a\,b\,c)$ with $a\in U$. Choose $a'\in U\setminus\{a\}$ and conjugate within $A_U$ to obtain $\tau'=(a'\,b\,c)$. Then

$$
\tau(\tau')^{-1}=(a\,b\,a').
$$

The preceding case first adds $b$; applying it again to $\tau$ adds $c$. This proves [connected triple supports generate an alternating group](../../../../../../connected-triple-supports-generate-an-alternating-group.md), by successively merging the intersecting triples of a connected support hypergraph. We used that [three-cycles](../../../../../../three-cycle.md) generate [alternating groups](../../../../../../alternating-group.md): pairs of [transpositions](../../../../../../transposition-permutation.md) with a common letter are [three-cycles](../../../../../../three-cycle.md), while a pair of disjoint [transpositions](../../../../../../transposition-permutation.md) is a product of two [three-cycles](../../../../../../three-cycle.md).

Now take all conjugates in $G$ of the given [three-cycle](../../../../../../three-cycle.md). Their support hypergraph is $G$-invariant, and its connected components form a [block system](../../../../../../block-system.md). Transitivity makes their union the whole set. There is an edge, so a component has more than one vertex. A [primitive group action](../../../../../../primitive-group-action.md) forces a single component. The preceding merging argument proves

$$
\boxed{A_n\le G.}
$$

For the first family of counterexamples, let

$$
G=PGL_2(p)\curvearrowright\mathbb P^1(\mathbb F_p),\qquad p>3.
$$

Its elements are [Möbius transformations](../../../../../../mobius-transformation.md) $x\mapsto(ax+b)/(cx+d)$, modulo nonzero scalar [matrices](../../../../../../matrix.md). Any ordered triple of distinct [projective points](../../../../../../projective-point.md) is the image of $(\infty,0,1)$ under exactly one such transformation: representatives of the first two target lines form a [basis](../../../../../../basis.md), and scaling the two columns sends their sum to the third target line. Thus the action is [sharply three-transitive](../../../../../../sharp-three-transitivity.md), hence [two-transitive](../../../../../../two-transitive-group-action.md) and primitive. Its degree is $p+1$ and order $p(p^2-1)$. It is divisible by $p$, but

$$
\frac{|A_{p+1}|}{|PGL_2(p)|}=\frac{(p-2)!}{2}>1,
$$

so it cannot contain $A_{p+1}$.

For the second example take

$$
\boxed{p=7,\quad G=PGL_2(8),\quad n=9,\quad |G|=504.}
$$

The same projective-line construction over $\mathbb F_8$ is [sharply three-transitive](../../../../../../sharp-three-transitivity.md). Its order is divisible by 7 and is less than $|A_9|=181440$, so it does not contain $A_9$. For a concrete field one can use $\mathbb F_8=\mathbb F_2[u]/(u^3+u+1)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
