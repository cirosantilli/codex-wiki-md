<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [locally small category](../../../../../locally-small-category.md) $\mathcal C$, an object $A$, and a functor $F:\mathcal C\to\mathbf{Set}$, the covariant [Yoneda lemma](../../../../../yoneda-lemma.md) is the natural bijection

$$
\operatorname{Nat}(\mathcal C(A,-),F)\longrightarrow F(A),
\qquad \alpha\longmapsto\alpha_A(1_A).
$$

Its inverse sends $x\in F(A)$ to the [natural transformation](../../../../../natural-transformation.md) whose component at $B$ maps $f:A\to B$ to $F(f)(x)$.

Suppose now that $\mathcal C$ is a [small category](../../../../../small-category.md). For $F:\mathcal C\to\mathbf{Set}$, form the [coproduct in a category](../../../../../coproduct.md)

$$
P=\coprod_{(A,x),\ x\in F(A)}\mathcal C(A,-).
$$

The [Yoneda lemma](../../../../../yoneda-lemma.md) associates to every summand the natural transformation determined by $x$, and these transformations combine to a map $p:P\to F$. At an object $B$, the element $y\in F(B)$ is the image of $1_B$ in the summand indexed by $(B,y)$, so $p$ is a [pointwise epimorphism in a functor category](../../../../../pointwise-epimorphism-in-a-functor-category.md). Each [representable functor](../../../../../representable-functor.md) $\mathcal C(A,-)$ is a [projective object in a category](../../../../../projective-object.md), since

$$
\operatorname{Nat}(\mathcal C(A,-),- )\cong\operatorname{ev}_A
$$

and evaluation preserves pointwise epimorphisms. A coproduct of projectives is projective, so $P$ is the required projective object. This is the [projective cover of a set-valued functor by representables](../../../../../projective-cover-of-a-set-valued-functor-by-representables.md).

We next prove the three equivalent conditions. If every [morphism](../../../../../morphism.md) of $\mathcal C$ is a [monomorphism](../../../../../monomorphism.md), then for $f:B\to C$ and every $A$, postcomposition

$$
\mathcal C(A,B)\longrightarrow\mathcal C(A,C),
\qquad g\longmapsto fg
$$

is injective. Thus every covariant [representable functor](../../../../../representable-functor.md) is a [monofunctor](../../../../../monofunctor.md). Conversely, taking $A=B$ shows that injectivity for every representable implies that $fg=fh$ forces $g=h$, so every $f$ is monic.

If all representables are monofunctors, the object $P$ above is a monofunctor because a coproduct of injective functions is injective. Hence every $F$ is an epimorphic image of a monofunctor. Conversely, suppose every functor is an epimorphic image of a monofunctor and apply this to a representable $R$. Choose an epimorphism $q:M\twoheadrightarrow R$ with $M$ a monofunctor. Since $R$ is projective, $1_R$ lifts to $s:R\to M$ with $qs=1_R$. Thus $R$ is a [retract in a category](../../../../../retract-in-a-category.md) of $M$. Every retract of a monofunctor is a monofunctor: if $R(f)x=R(f)y$, then injectivity of $M(f)$ applied to $s(x)$ and $s(y)$ gives $s(x)=s(y)$, and applying $q$ gives $x=y$. This completes the equivalence.

Finally, every functor $\mathcal C\to\mathbf{Set}$ is a monofunctor exactly when every morphism of $\mathcal C$ is a [split monomorphism](../../../../../split-monomorphism.md). The forward implication is immediate because every functor preserves a left inverse. For the converse, fix $f:A\to B$ and form a quotient of $\mathcal C(A,-)\sqcup1$ by identifying the distinguished point with every arrow of the form $kf:A\to X$, where $k:B\to X$. In the resulting functor $Q$, the two elements $[1_A]$ and $*$ of $Q(A)$ have equal images under $Q(f)$ because $[f]=*$. If every functor is a monofunctor, $Q(f)$ is injective, so $[1_A]=*$. By construction this means $1_A=rf$ for some $r:B\to A$. Thus $f$ is split monic. Equivalently, every morphism of $\mathcal C$ must be an [absolute monomorphism](../../../../../absolute-monomorphism.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
