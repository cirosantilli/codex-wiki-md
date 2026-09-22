<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [monomorphism](../../../../../monomorphism.md) is a left-cancellable morphism. A [strong monomorphism](../../../../../strong-monomorphism.md) $m:S\to A$ has the right lifting property against every [epimorphism](../../../../../epimorphism.md): from a commutative square

$$
\begin{array}{ccc}
X&\xrightarrow{u}&S\\
\downarrow e&&\downarrow m\\
Y&\xrightarrow{v}&A
\end{array}
$$

with $e$ epic, one obtains $d:Y\to S$ satisfying $de=u$ and $md=v$. A [regular monomorphism](../../../../../regular-monomorphism.md) is an [equalizer](../../../../../equaliser.md) of a parallel pair.

Suppose $m:S\to A$ equalizes $r,s:A\rightrightarrows C$. In the square above,

$$
rve=rmu=smu=sve.
$$

Since $e$ is epic, $rv=sv$, so the universal property of the equalizer gives the required $d$. Thus every regular monomorphism is strong.

Let $m_i:S_i\to A$ be strong for $i=1,2$, and let $P=S_1\times_A S_2$. Given a lifting square against $P\to A$, compose its top map with each projection. Strength of $m_i$ produces maps $d_i:Y\to S_i$ with $m_id_i=v$. The pair $(d_1,d_2)$ has equal composites to $A$, hence induces $d:Y\to P$. Therefore [intersections of strong subobjects](../../../../../intersection-of-strong-subobjects.md) are strong.

Call a morphism [anodyne](../../../../../anodyne-morphism-in-a-category.md) when it is both monic and epic, and call an object [saturated](../../../../../saturated-object-with-respect-to-anodyne-morphisms.md) when it is injective with respect to every such morphism. Let $m:S\to B$ be a strong subobject of a saturated object. Given an anodyne $e:X\to Y$ and $u:X\to S$, saturation of $B$ extends $mu$ to some $v:Y\to B$. Strength of $m$ applied to $mu=ve$ lifts $v$ to $d:Y\to S$ with $de=u$. Hence $S$ is saturated.

Now embed $A$ as a subobject of a saturated object $B$. Since the category is [well-powered](../../../../../well-powered-category.md), the strong subobjects of $B$ through which $A\to B$ factors form a set; completeness supplies their intersection $j:R\to B$. The same coordinatewise lifting argument used for two factors shows that $j$ is strong, so $R$ is saturated.

The induced map $\eta:A\to R$ is monic. To prove it epic, let $f,g:R\rightrightarrows C$ satisfy $f\eta=g\eta$. Their equalizer $q:E\to R$ is regular and hence strong. Composites of strong monomorphisms are strong, so $jq:E\to B$ is a strong subobject containing $A$. Minimality of the intersection forces $R\to B$ to factor through $E$, which implies $f=g$. Thus $\eta$ is epic and therefore anodyne.

For every saturated $S$, each map $a:A\to S$ extends across $\eta$ to a map $\bar a:R\to S$. This extension is unique because $\eta$ is epic. Consequently $A\mapsto R$ is left adjoint to the inclusion of saturated objects: the full subcategory $\mathcal S$ is [reflective](../../../../../reflective-subcategory.md). This is the [saturated reflection from a strong-subobject intersection](../../../../../saturated-reflection-from-a-strong-subobject-intersection.md).

It remains to prove that $\mathcal S$ is [balanced](../../../../../balanced-category.md). First let $e:X\to Y$ be epic in $\mathcal S$. If $f,g:Y\rightrightarrows Z$ are morphisms in the ambient category, embed $Z$ into a saturated object $T$. Equality $fe=ge$ then implies equality after composing with $Z\to T$; epicity in the full subcategory gives equality there, and monicity of $Z\to T$ gives $f=g$. Thus $e$ is epic in the ambient category.

If $e:X\to Y$ is also monic in $\mathcal S$, it is monic in the ambient category as well. Indeed, for $u,v:W\rightrightarrows X$ with $eu=ev$, reflect $W$ by an anodyne map $W\to RW$. Saturation extends $u$ and $v$ to $\bar u,\bar v:RW\rightrightarrows X$; ambient epicity of $W\to RW$ and monicity of $e$ inside $\mathcal S$ give $\bar u=\bar v$, hence $u=v$. Therefore $e$ is anodyne in the ambient category. Saturation of $X$ extends $1_X$ across $e$ to a retraction $r:Y\to X$. Since $e$ is epic, $ere=e$ implies $er=1_Y$, so $e$ is an isomorphism. Hence $\mathcal S$ is balanced.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
