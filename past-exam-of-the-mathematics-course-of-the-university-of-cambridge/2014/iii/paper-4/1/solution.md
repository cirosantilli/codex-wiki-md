<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Construct the [free product](../../../../../free-product.md) from the empty word and all finite alternating words $g_1\cdots g_k$, whose [syllables in a free product](../../../../../syllable-in-a-free-product.md) are nonidentity elements of tagged copies of $G_1,G_2$, with adjacent syllables from different factors. Multiply by concatenating, multiplying adjacent elements in the same factor, and deleting identities until the word is reduced. The [normal form theorem for a free product](../../../../../normal-form-theorem-for-a-free-product.md) gives a unique result; reducing three concatenated words gives the same result under either parenthesization, so multiplication is associative. The empty word is the identity, and the inverse reverses the word and inverts each syllable. Each factor embeds as words of length one.

The [universal property of a free product](../../../../../universal-property-of-a-free-product.md) says that for every [group](../../../../../group-split.md) $K$ and [group homomorphisms](../../../../../group-homomorphism.md) $f_i:G_i\to K$ there is a unique [group homomorphism](../../../../../group-homomorphism.md) $f:G_1*G_2\to K$ extending both. Explicitly, send a reduced word to the product of its syllable images; reduction preserves this product. This gives existence, while generation by the two factors gives uniqueness.

A standard form of [Klein's combination theorem](../../../../../ping-pong-lemma.md), or the [ping-pong lemma](../../../../../ping-pong-lemma.md), is the following. Let nontrivial [subgroups](../../../../../subgroup.md) $G_1,G_2$ of the [homeomorphisms](../../../../../homeomorphism.md) of a [topological space](../../../../../topological-space.md) $X$ have disjoint nonempty [subsets](../../../../../subset.md) $X_1,X_2$ with

$$
g(X_2)\subseteq X_1\quad(1\ne g\in G_1),\qquad h(X_1)\subseteq X_2\quad(1\ne h\in G_2).
$$

Assume also that at least one factor has at least three elements. Then **the generated [subgroup](../../../../../subgroup.md) is $\boxed{\langle G_1,G_2\rangle\cong G_1*G_2}$**. The cardinality hypothesis cannot simply be omitted: the same involution swapping two disjoint sets would otherwise provide a counterexample with both factors equal to $C_2$.

Here is the [ping-pong lemma](../../../../../ping-pong-lemma.md) proof. A reduced word of odd length begins and ends in the same factor, so repeated application of the displayed inclusions sends the other factor's domain into that factor's domain. Disjointness shows that the word is not the identity. For an even reduced word, relabel the factors so that $|G_1|\geq3$, and invert the word if necessary to make it begin with $g\in G_1$ and end in $G_2$. Choose $s\in G_1\setminus\{1,g^{-1}\}$. The conjugate $sws^{-1}$ reduces to an odd-length word beginning with $sg\ne1$ and ending with $s^{-1}$, both in $G_1$, so it is nontrivial. Thus no nonempty reduced word lies in the kernel of the natural [group homomorphism](../../../../../group-homomorphism.md) $G_1*G_2\to\langle G_1,G_2\rangle$, proving the theorem.

For an explicit example, let $X=\mathbb R\cup\{\infty\}$ be the one-dimensional [Real projective space](../../../../../real-projective-space.md), and take the [Möbius transformations](../../../../../mobius-transformation.md)

$$
A(t)=t+2,\qquad B(t)=\frac{t}{2t+1},\qquad X_1=\{t:|t|>1\}\cup\{\infty\},\quad X_2=\{t:|t|<1\}.
$$

For every nonzero [integer](../../../../../integer.md) $n$, $A^n(t)=t+2n$ sends $X_2$ into $X_1$, while $B^n(t)=t/(2nt+1)$ sends $X_1$ into $X_2$. Indeed $|2nt+1|>|t|$ when $|t|>1$, and $B^n(\infty)=1/(2n)$. Both transformations have infinite order. Hence the [ping-pong lemma](../../../../../ping-pong-lemma.md) gives **$\boxed{\langle A,B\rangle\cong\mathbb Z*\mathbb Z=F_2}$**, a [free product](../../../../../free-product.md) of two nontrivial [finitely presented groups](../../../../../finitely-presented-group.md).

A [finitely presented group](../../../../../finitely-presented-group.md) admits a [group presentation](../../../../../group-presentation.md) $\langle S\mid R\rangle$ with both $S$ and $R$ finite; it is the quotient of the [free group](../../../../../free-group.md) on $S$ by the [normal closure](../../../../../normal-closure.md) of $R$. If

$$
G=\langle S\mid R\rangle,\qquad H=\langle T\mid U\rangle
$$

with disjoint generator sets, then

$$
\boxed{G*H=\langle S\sqcup T\mid R\sqcup U\rangle.}
$$

Maps from this [group presentation](../../../../../group-presentation.md) to any [group](../../../../../group-split.md) are exactly pairs of maps from $G$ and $H$, so the [universal property of a free product](../../../../../universal-property-of-a-free-product.md) proves the formula.

For a [group homomorphism](../../../../../group-homomorphism.md) $\phi:H\to\operatorname{Aut}(G)$, choose a word $w_{t,s}(S)$ representing $\phi(t)(s)$ for each $t\in T,s\in S$. The [presentation of a semidirect product](../../../../../presentation-of-a-semidirect-product.md) is

$$
\boxed{G\rtimes_\phi H=\langle S\sqcup T\mid R,U,\ t s t^{-1}=w_{t,s}\ (t\in T,s\in S)\rangle.}
$$

The presentation maps onto the specified [semidirect product](../../../../../semidirect-product.md). Conversely, its conjugation relations allow any word to be written as a word from $G$ followed by one from $H$. The natural maps from the two factors to the presented group satisfy the full action relation, because conjugation agrees with $\phi$ first on generators and hence on all elements. They define the reverse [group homomorphism](../../../../../group-homomorphism.md) $(g,h)\mapsto gh$. The two maps are inverse on every generator, proving the [group isomorphism](../../../../../group-isomorphism.md). There are finitely many cross-relations, so the result is again a [finitely presented group](../../../../../finitely-presented-group.md).

Apply this to the specified permutation action. The presentation is

$$
\langle x,y,z,c\mid c^3=1,\ cxc^{-1}=y,\ cyc^{-1}=z,\ czc^{-1}=x\rangle.
$$

Eliminate $y=cxc^{-1}$ and $z=c^2xc^{-2}$. The last cross-relation becomes $c^3xc^{-3}=x$, already implied by $c^3=1$. Thus

$$
\boxed{F_3\rtimes_\phi C_3\cong\langle x,c\mid c^3=1\rangle\cong\mathbb Z*C_3.}
$$

Both factors are nontrivial [finitely presented groups](../../../../../finitely-presented-group.md), as required.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
