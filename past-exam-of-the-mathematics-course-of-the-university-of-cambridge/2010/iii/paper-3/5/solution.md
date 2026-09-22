<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Put $D=\mathbb Q/\mathbb Z$. The [character module](../../../../../character-module.md) $M^*=\operatorname{Hom}_{\mathbb Z}(M,D)$ has the natural action

$$
\boxed{(a\phi)(m)=\phi(am).}
$$

Additivity is immediate, and $a(b\phi)(m)=\phi(bam)=\phi(abm)$, using commutativity of $A$. The identity of $A$ acts as the identity. We establish the extension and duality tools used in the four implications, so no flatness or injectivity criterion is assumed without proof.

An [injective module](../../../../../injective-module.md) $E$ is one for which every homomorphism from a [submodule](../../../../../submodule.md) $U\subseteq V$ extends to $V$. The [Baer criterion](../../../../../baer-criterion.md) says it suffices to test the inclusions of ideals $I\subseteq A$. Necessity follows directly from the definition. For sufficiency, suppose every $I\to E$ extends to $A$. Given $h:U\to E$, use [Zorn's lemma](../../../../../zorn-s-lemma.md) to choose a maximal extension $(W,h_W)$ inside $V$; extensions along a chain have a well-defined union. If $v\in V\setminus W$, let

$$
I=\{a\in A:av\in W\},\qquad \theta(a)=h_W(av).
$$

This is an ideal and an $A$-linear map. Its extension to $A$ has the form $a\mapsto ae$ for some $e\in E$. Then

$$
h'(w+av)=h_W(w)+ae
$$

is well-defined: if two expressions represent the same element, their coefficient difference lies in $I$, where the two prescribed values agree. It extends $h_W$ to the strictly larger module $W+Av$, a contradiction. Thus $W=V$, proving the [Baer criterion](../../../../../baer-criterion.md) for arbitrary modules and ideals.

The group $D$ is divisible. A homomorphism $n\mathbb Z\to D$, for $n>0$, extends to $\mathbb Z$ by choosing $d\in D$ with $nd$ equal to its value at $n$; the zero ideal causes no restriction. The proved [Baer criterion](../../../../../baer-criterion.md) over $\mathbb Z$ therefore makes $D$ injective. It is also a cogenerator: a nonzero element $x$ of an abelian group generates either a finite cyclic group of order $n>1$, which maps $x$ to $1/n+\mathbb Z$, or an infinite cyclic group, which maps $x$ to $1/2+\mathbb Z$. Injectivity extends this character to the whole group. Thus **every nonzero element is detected by an additive character**.

It follows that a group homomorphism $u:T\to U$ is injective exactly when

$$
u^*: \operatorname{Hom}_{\mathbb Z}(U,D)
\longrightarrow\operatorname{Hom}_{\mathbb Z}(T,D)
$$

is surjective. For an injection, extension into the injective group $D$ proves surjectivity. Conversely, a character nonzero on an element of $\ker u$ cannot be the pullback of a character on $U$. This is the detection property of the [injective cogenerator of abelian groups](../../../../../injective-cogenerator-of-abelian-groups.md).

Finally, for any $A$-module $N$ there is a natural character form of the [Tensor-hom adjunction](../../../../../tensor-hom-adjunction.md):

$$
\boxed{\operatorname{Hom}_A(N,M^*)
\simeq\operatorname{Hom}_{\mathbb Z}(N\otimes_AM,D).}
$$

An $A$-linear map $h$ gives the pairing $(n,m)\mapsto h(n)(m)$. It is balanced because $h(an)(m)=(ah(n))(m)=h(n)(am)$. Conversely a balanced additive pairing determines $h$ by this formula. The [universal property of the tensor product of modules](../../../../../universal-property-of-the-tensor-product-of-modules.md) makes these constructions mutually inverse, and compatible with restriction maps.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
