<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [regular category](../../../../../regular-category.md) has [finite limits](../../../../../finite-limit.md), factorizations of every arrow as a [regular epimorphism](../../../../../regular-epimorphism.md) followed by a [monomorphism](../../../../../monomorphism.md), and pullback-stable [regular epimorphisms](../../../../../regular-epimorphism.md). Equivalently one may require [coequalizers](../../../../../coequalizer.md) of [kernel pairs](../../../../../kernel-pair.md) and pullback stability of the resulting quotients. A [regular epimorphism](../../../../../regular-epimorphism.md) is a [coequalizer](../../../../../coequalizer.md) of some parallel pair; an [extremal epimorphism](../../../../../extremal-epimorphism.md) is an [epimorphism](../../../../../epimorphism.md) $e$ such that $e=mh$, with $m$ monic, forces $m$ to be invertible.

First, every [regular epimorphism](../../../../../regular-epimorphism.md) is extremal without assuming regularity of the whole category. Suppose $e:A\to B$ coequalizes $r,s$ and $e=mh$. Since $m$ is monic, $hr=hs$, so the universal property gives $k:B\to\operatorname{dom}(m)$ with $ke=h$. Then $mke=e$; cancellation of the [epimorphism](../../../../../epimorphism.md) $e$ gives $mk=1_B$. Monicity of $m$ now gives $km=1$, so $m$ is an [isomorphism](../../../../../isomorphism.md). Conversely, in a [regular category](../../../../../regular-category.md), factor an extremal $e$ as $mq$ with $q$ regular epic and $m$ monic. Extremality makes $m$ invertible, so $e$ is regular epic. Thus **covers and [regular epimorphisms](../../../../../regular-epimorphism.md) coincide**.

For a counterexample, work in the category of small categories, which has [finite limits](../../../../../finite-limit.md) constructed on objects and arrows. Let $C$ be two disjoint walking arrows $a\xrightarrow{u}b$ and $c\xrightarrow{v}d$. Let $D$ be the walking [isomorphism](../../../../../isomorphism.md), with two objects $0,1$ and inverse arrows $p:0\to1$, $q:1\to0$. Define $F:C\to D$ by $a,d\mapsto0$, $b,c\mapsto1$, $u\mapsto p$, $v\mapsto q$. These images generate all of $D$, so two functors agreeing after $F$ agree everywhere; thus $F$ is epic.

A monic functor is injective on objects and faithful, as tested by functors from the terminal category and from the walking arrow. If $F$ factors through such a functor $m:D'\to D$, its image contains both objects and both arrows $p,q$. Faithfulness forces their lifted composites to be the identities, so the image contains every arrow of $D$ and $m$ is an [isomorphism](../../../../../isomorphism.md). Hence $F$ is extremal.

It is not regular. Its [kernel pair](../../../../../kernel-pair.md) identifies the endpoint pairs $a,d$ and $b,c$ but has no relation forcing the composites of the images of $u,v$ to be identities. Concretely, send all four objects to the one-object category with endomorphism monoid $\{1,e\}$, $e^2=e\ne1$, and send both $u,v$ to $e$. This functor equalizes the [kernel pair](../../../../../kernel-pair.md): corresponding identities agree, and the only nonidentity arrow pairs in the [kernel pair](../../../../../kernel-pair.md) are an arrow paired with itself. It cannot factor through $D$, because images of $p,q$ would have to be inverse, whereas $e^2\ne1$. In a category with [kernel pairs](../../../../../kernel-pair.md), every [regular epimorphism](../../../../../regular-epimorphism.md) is the [coequalizer](../../../../../coequalizer.md) of its [kernel pair](../../../../../kernel-pair.md): its original coequalized pair factors through that [kernel pair](../../../../../kernel-pair.md), giving the universal property. Therefore **$F$ is an extremal but nonregular [epimorphism](../../../../../epimorphism.md)**, the promised [nonregular extremal epimorphism in the category of categories](../../../../../nonregular-extremal-epimorphism-in-the-category-of-categories.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
