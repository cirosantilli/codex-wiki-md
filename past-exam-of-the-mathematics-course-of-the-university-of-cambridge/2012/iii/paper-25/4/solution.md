<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The limit form of the [Special adjoint functor theorem](../../../../../special-adjoint-functor-theorem.md) is as follows. Let $\mathcal C$ be a [locally small category](../../../../../locally-small-category.md), a [complete category](../../../../../complete-category.md), and a [well-powered category](../../../../../well-powered-category.md), and suppose it has a [small cogenerating family](../../../../../cogenerating-set.md) $(Q_i)_{i\in I}$. Let $\mathcal D$ be a [locally small category](../../../../../locally-small-category.md). Then a [functor](../../../../../functor.md) $G:\mathcal C\to\mathcal D$ has a [left adjoint](../../../../../adjoint-functors.md) **if and only if it preserves all small [categorical limits](../../../../../categorical-limit.md)**. The dual exchanges completeness, well-poweredness and cogenerators for cocompleteness, well-copoweredness and generators, and characterizes [functors](../../../../../functor.md) with a [right adjoint](../../../../../adjoint-functors.md).

Here a [cogenerating set](../../../../../cogenerating-set.md) distinguishes unequal parallel maps by postcomposition into one of the $Q_i$. A [well-powered category](../../../../../well-powered-category.md) has a set of [subobjects](../../../../../subobject.md) of each fixed object. Completeness means existence of all small [categorical limits](../../../../../categorical-limit.md). We use the [initial-object lemma for complete categories with a weakly initial set](../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md): a [complete category](../../../../../complete-category.md) that is [locally small](../../../../../locally-small-category.md) has an [initial object](../../../../../initial-object.md) exactly when it has a [weakly initial set](../../../../../weakly-initial-set.md). A proof is given in Question 5(c). We also use the fact that when $G$ preserves small [categorical limits](../../../../../categorical-limit.md), the [comma category](../../../../../comma-category.md) $(B\downarrow G)$ is complete, with its limits constructed in $\mathcal C$; local smallness is inherited from $\mathcal C$. Finally, having an [initial object](../../../../../initial-object.md) in $(B\downarrow G)$ for each $B$ is the [universal arrow from an object to a functor](../../../../../universal-arrow-from-an-object-to-a-functor.md) characterization of a [left adjoint](../../../../../adjoint-functors.md).

Assume $G$ preserves small [categorical limits](../../../../../categorical-limit.md), and fix $B\in\mathcal D$. We will construct a [weakly initial set](../../../../../weakly-initial-set.md) in $(B\downarrow G)$, rather than assume a solution set. Start with an arbitrary object $(C,x)$, where $x:B\to GC$. Call a [subobject](../../../../../subobject.md) $m:S\hookrightarrow C$ supporting if $x=G(m)x_S$ for some $x_S:B\to GS$. There is at least one, namely $1_C$. Because $G$ preserves [pullbacks in a category](../../../../../pullback-category-theory.md), it preserves [monomorphisms](../../../../../monomorphism.md): the self-pullback characterization of a monic map is preserved. Consequently each $x_S$ is unique.

There is a set of supporting [subobjects](../../../../../subobject.md) by well-poweredness. Their [intersection of subobjects](../../../../../intersection-of-subobjects.md) exists by completeness; write it $m_0:C_0\hookrightarrow C$. Applying $G$ to this intersection [categorical limit](../../../../../categorical-limit.md) gives a unique $x_0:B\to GC_0$ lifting all the $x_S$, and hence $x=G(m_0)x_0$. Minimality says that any [subobject](../../../../../subobject.md) $n:R\hookrightarrow C_0$ supporting $x_0$ is invertible: $m_0n$ supports $x$, so $m_0$ factors through $m_0n$, giving a right inverse to the monic $n$.

If $u,v:C_0\to Q_i$ satisfy $G(u)x_0=G(v)x_0$, their [equalizer](../../../../../equaliser.md) supports $x_0$, since $G$ preserves that [equalizer](../../../../../equaliser.md). It is therefore an [isomorphism](../../../../../isomorphism.md), and $u=v$. We have obtained an [injective function](../../../../../injective-function.md)

$$
\mathcal C(C_0,Q_i)\longrightarrow\mathcal D(B,GQ_i),\qquad u\longmapsto G(u)x_0.
$$

Let $J_i$ be its image, a subset of the fixed [set](../../../../../set-split.md) $S_i=\mathcal D(B,GQ_i)$. The [evaluation embedding into cogenerator products](../../../../../evaluation-embedding-into-cogenerator-products.md) is a [monomorphism](../../../../../monomorphism.md)

$$
C_0\hookrightarrow P_J:=\prod_{i\in I}\prod_{s\in J_i}Q_i.
$$

Indeed each $s\in J_i$ corresponds to a unique map $C_0\to Q_i$, and the [cogenerating set](../../../../../cogenerating-set.md) property makes the resulting family jointly monic. Notice that we use the realized subsets $J_i$, not all of $S_i$: there need not be a map $C_0\to Q_i$ available for an unused index.

There is a set of tuples $J=(J_i)$, since $I$ and every $S_i$ are sets. For each resulting $P_J$, choose representatives of its [subobjects](../../../../../subobject.md); these form a set by well-poweredness. For every representative $R$, include every map $y:B\to GR$, a set by local smallness of $\mathcal D$. All resulting pairs $(R,y)$ form a set. Our given $(C,x)$ receives a map from such a pair: transport $x_0$ along the [isomorphism](../../../../../isomorphism.md) between $C_0$ and the chosen representative, then compose its inverse with $m_0$. Thus these pairs form a [weakly initial set](../../../../../weakly-initial-set.md) in $(B\downarrow G)$. This is the [cogenerator bound for comma-category solution sets](../../../../../cogenerator-bound-for-comma-category-solution-sets.md).

The [initial-object lemma for complete categories with a weakly initial set](../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md) gives an [initial object](../../../../../initial-object.md) $(LB,\eta_B)$. For $h:B\to B'$, define $Lh$ by the unique equation

$$
G(Lh)\eta_B=\eta_{B'}h.
$$

Uniqueness proves the [functor](../../../../../functor.md) laws and gives the [natural bijections](../../../../../natural-bijection.md)

$$
\boxed{\mathcal C(LB,C)\cong\mathcal D(B,GC),\qquad f\longmapsto G(f)\eta_B.}
$$

Thus $L\dashv G$. Conversely, a [right adjoint](../../../../../adjoint-functors.md) preserves small [categorical limits](../../../../../categorical-limit.md): its adjunction identifies maps into the proposed limiting object with compatible families of maps into the diagram. This proves both directions of the [limit form of the special adjoint functor theorem](../../../../../limit-form-of-the-special-adjoint-functor-theorem.md). Applying the argument to the [opposite categories](../../../../../opposite-category.md) proves the dual statement. Choices of representatives and adjoint objects are understood in the usual ambient-universe convention for large [categories](../../../../../category-split.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
