<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [monomorphism](../../../../../monomorphism.md) $m:A\to B$ is left cancellable: $mu=mv$ implies $u=v$ for all parallel arrows into $A$. A [strong monomorphism](../../../../../strong-monomorphism.md) is a [monomorphism](../../../../../monomorphism.md) with the following lifting property: if $e:X\to Y$ is an [epimorphism](../../../../../epimorphism.md) and $u:X\to A$, $v:Y\to B$ satisfy $mu=ve$, there is a diagonal $d:Y\to A$ with $de=u$ and $md=v$. It is unique by monicity. An [extremal monomorphism](../../../../../extremal-monomorphism.md) is a [monomorphism](../../../../../monomorphism.md) $m$ for which every factorization $m=he$ with $e$ an [epimorphism](../../../../../epimorphism.md) forces $e$ to be an [isomorphism](../../../../../isomorphism.md). We use the strong lifting formulation for the paper's terminology; below we also justify its equivalence with the extremal formulation under the complete, well-powered hypotheses. A [regular monomorphism](../../../../../regular-monomorphism.md) is an [equalizer](../../../../../equaliser.md) of two parallel arrows.

First, a [strong monomorphism](../../../../../strong-monomorphism.md) is extremal. In a factorization $m=he$, apply its lifting property with upper arrow $1_A$ and lower arrow $h$. This gives $d$ with $de=1_A$. Since $e$ is an [epimorphism](../../../../../epimorphism.md), $ed e=e$ implies $ed=1$, so $e$ is an [isomorphism](../../../../../isomorphism.md).

If $m:A\to B$ is an [equalizer](../../../../../equaliser.md) of $r,s:B\rightrightarrows C$, consider a lifting square as above. The equation $rve=smu=sve$ and the [epimorphism](../../../../../epimorphism.md) property give $rv=sv$. The [equalizer](../../../../../equaliser.md) property therefore gives a unique $d$ with $md=v$. Monicity then gives $de=u$. Hence **every [regular monomorphism](../../../../../regular-monomorphism.md) is a [strong monomorphism](../../../../../strong-monomorphism.md)**.

For the [intersection of strong subobjects](../../../../../intersection-of-strong-subobjects.md), let $m_i:A_i\to B$ be strong and let $p_i:P\to A_i$ exhibit their intersection, with $m=m_1p_1=m_2p_2$. Given $mu=ve$ with $e$ an [epimorphism](../../../../../epimorphism.md), the two [strong monomorphisms](../../../../../strong-monomorphism.md) supply diagonals $d_i:Y\to A_i$ satisfying $d_ie=p_iu$ and $m_id_i=v$. The [pullback in a category](../../../../../pullback-category-theory.md) property supplies $d:Y\to P$ with $p_id=d_i$. Its two projections show $de=u$, and $md=v$. Thus **the intersection is strong**. The same argument works for every existing small intersection of [strong monomorphisms](../../../../../strong-monomorphism.md). Also, composites of [strong monomorphisms](../../../../../strong-monomorphism.md) are strong: first lift through the outer one, then through the inner one.

Write $\mathcal S$ for the full [subcategory](../../../../../subcategory.md) formed by every [saturated object with respect to anodyne morphisms](../../../../../saturated-object-with-respect-to-anodyne-morphisms.md), using the paper's [anodyne morphism in a category](../../../../../anodyne-morphism-in-a-category.md) convention. Let $m:C\to B$ be a [strong monomorphism](../../../../../strong-monomorphism.md) and $B$ saturated. For an [anodyne morphism in a category](../../../../../anodyne-morphism-in-a-category.md) $e:X\to Y$ and $u:X\to C$, saturation extends $mu$ to $v:Y\to B$. Since $e$ is an [epimorphism](../../../../../epimorphism.md), the strong lifting property supplies $d:Y\to C$ extending $u$. Therefore **every strong [subobject](../../../../../subobject.md) of a saturated object is saturated**.

Now assume $\mathcal C$ is a [complete category](../../../../../complete-category.md) and a [well-powered category](../../../../../well-powered-category.md), with the given saturated embeddings. Choose a [monomorphism](../../../../../monomorphism.md) $a:A\to B$ into a saturated object. Intersect all strong [subobjects](../../../../../subobject.md) of $B$ through which $a$ factors. They form a set by the [well-powered category](../../../../../well-powered-category.md) hypothesis, and the identity of $B$ is one of them. Completeness constructs their intersection, so we obtain

$$
A\xrightarrow{\eta_A}LA\xrightarrow{m}B,\qquad m\eta_A=a.
$$

By the [intersection of strong subobjects](../../../../../intersection-of-strong-subobjects.md), $m$ is strong; hence $LA$ is saturated. Since $a$ is a [monomorphism](../../../../../monomorphism.md), so is $\eta_A$.

To prove that $\eta_A$ is an [epimorphism](../../../../../epimorphism.md), take $u,v:LA\rightrightarrows D$ with $u\eta_A=v\eta_A$. Their [equalizer](../../../../../equaliser.md) $j:E\to LA$ is a [regular monomorphism](../../../../../regular-monomorphism.md), and $\eta_A$ factors through it. The composite $mj:E\to B$ is strong, so it belongs to the family defining $LA$. Minimality gives $t:LA\to E$ with $mjt=m$. Cancelling $m$ gives $jt=1_{LA}$; since $j$ is a [monomorphism](../../../../../monomorphism.md), also $tj=1_E$. Thus $j$ is an [isomorphism](../../../../../isomorphism.md) and $u=v$. We have proved

$$
\boxed{\eta_A:A\to LA\text{ is both monic and epic, and }LA\text{ is saturated}.}
$$

This is the [saturated reflection from a strong-subobject intersection](../../../../../saturated-reflection-from-a-strong-subobject-intersection.md).

The construction of a least strong [subobject](../../../../../subobject.md) and the [equalizer](../../../../../equaliser.md) argument work for any morphism into any object, without requiring the source map to be monic or the target to be saturated. They give an [epimorphism](../../../../../epimorphism.md) followed by a [strong monomorphism](../../../../../strong-monomorphism.md). Applying this factorization to an [extremal monomorphism](../../../../../extremal-monomorphism.md) makes the first factor invertible; thus the extremal and strong formulations agree under the present complete, well-powered hypotheses.

For every saturated $S$, saturation extends every $f:A\to S$ across the [anodyne morphism in a category](../../../../../anodyne-morphism-in-a-category.md) $\eta_A$ to $\bar f:LA\to S$. Its extension is unique because $\eta_A$ is an [epimorphism](../../../../../epimorphism.md). Consequently

$$
\boxed{\mathcal S(LA,S)\cong\mathcal C(A,S),}
$$

naturally in $S$ and $A$. In particular, for $h:A\to A'$ define $Lh$ by $Lh\,\eta_A=\eta_{A'}h$; uniqueness proves the identity and composition laws. This constructs the [reflector](../../../../../reflector.md) and proves that $\mathcal S$ is a [reflective subcategory](../../../../../reflective-subcategory.md).

Finally we prove that $\mathcal S$ is a [balanced category](../../../../../balanced-category.md). If $e:U\to V$ is epic in $\mathcal S$ and $u,v:V\to X$ satisfy $ue=ve$, embed $X$ by a [monomorphism](../../../../../monomorphism.md) $j:X\to Y$ into a saturated object. Fullness makes $ju,jv$ arrows of $\mathcal S$, so $ju=jv$ and hence $u=v$. Thus **an [epimorphism](../../../../../epimorphism.md) in $\mathcal S$ is also epic in $\mathcal C$**.

A [monomorphism](../../../../../monomorphism.md) $f:U\to V$ in $\mathcal S$ is also monic in $\mathcal C$: for $a,b:X\to U$, extend them uniquely along $\eta_X$ to $\bar a,\bar b:LX\to U$. If $fa=fb$, cancellation of the ambient [epimorphism](../../../../../epimorphism.md) $\eta_X$ gives $f\bar a=f\bar b$, so monicity in $\mathcal S$ gives $\bar a=\bar b$ and $a=b$. Now if $f$ is both monic and epic in $\mathcal S$, it is an [anodyne morphism in a category](../../../../../anodyne-morphism-in-a-category.md) in $\mathcal C$. Saturation of $U$ extends $1_U$ across $f$ to $r:V\to U$ with $rf=1_U$. Ambient epicity gives $fr=1_V$. Fullness puts this inverse in $\mathcal S$, proving

$$
\boxed{\mathcal S\text{ is balanced}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
