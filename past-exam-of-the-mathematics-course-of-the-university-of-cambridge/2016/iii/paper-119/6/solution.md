<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An **[abelian category](../../../../../abelian-category.md)** is an [additive category](../../../../../additive-category.md) with a [kernel in a category](../../../../../kernel-in-a-category.md) and a [cokernel in a category](../../../../../cokernel-in-a-category.md) for every morphism, in which every [monomorphism](../../../../../monomorphism.md) is a kernel and every [epimorphism](../../../../../epimorphism.md) is a cokernel. In particular, every [epimorphism](../../../../../epimorphism.md) $p$ is the cokernel of its own kernel: if $p$ is initially a cokernel of $u$, then $u$ factors through $\ker p$, and the two cokernel universal properties agree. The dual statement holds for [monomorphisms](../../../../../monomorphism.md). Finite [biproducts](../../../../../biproduct.md) and kernels construct [finite limits](../../../../../finite-limit.md).

For [pullback stability of epimorphisms in an abelian category](../../../../../pullback-stability-of-epimorphisms-in-an-abelian-category.md), let $p:B\to C$ be an [epimorphism](../../../../../epimorphism.md) and $k:C'\to C$ any morphism. The map

$$
d=[p,-k]:B\oplus C'\to C
$$

is epic, since its restriction to the $B$ summand is $p$. Its [kernel in a category](../../../../../kernel-in-a-category.md) $i=(h,p'):B'\to B\oplus C'$ exhibits the [pullback in a category](../../../../../pullback-category-theory.md): the equation $d(h,p')=0$ means $ph=kp'$ and has exactly that universal property.

Suppose $v:C'\to D$ satisfies $vp'=0$. The morphism $[0,v]:B\oplus C'\to D$ annihilates $i$, so, because $d$ is the [cokernel in a category](../../../../../cokernel-in-a-category.md) of $i$, it factors as $[0,v]=wd$ for some $w:C\to D$. Restricting to $B$ gives $wp=0$, and epicity gives $w=0$. Hence $v=0$. Applying this to the difference of any two morphisms agreeing after $p'$ proves that $p'$ is an [epimorphism](../../../../../epimorphism.md). Therefore

$$
\boxed{\text{Epimorphisms in an abelian category are stable under pullback}.}
$$

This proof uses normality from the definition, rather than assuming the stability to be proved.

For the [pullback of a short exact sequence in an abelian category](../../../../../pullback-of-a-short-exact-sequence-in-an-abelian-category.md), use the displayed square's notation $g,g',h,k$. Exactness makes $f:A\to B$ the [kernel in a category](../../../../../kernel-in-a-category.md) of $g$. Since $gf=0=k0$, the [pullback in a category](../../../../../pullback-category-theory.md) gives a unique

$$
f':A\to B',\qquad hf'=f,\qquad g'f'=0.
$$

If $u:X\to B'$ has $g'u=0$, then $g(hu)=kg'u=0$, so there is a unique $v:X\to A$ with $fv=hu$. Both projections of the pullback give $f'v=u$: their composites with $h$ are equal and their composites with $g'$ are zero. The uniqueness of $v$ follows from monicity of $f$. Thus $f'$ is the [kernel in a category](../../../../../kernel-in-a-category.md) of $g'$. By the preceding stability result, $g'$ is an [epimorphism](../../../../../epimorphism.md). We obtain the required [exact sequence in an abelian category](../../../../../exact-sequence-in-an-abelian-category.md):

$$
\boxed{0\longrightarrow A\xrightarrow{f'}B'\xrightarrow{g'}C'\longrightarrow0.}
$$

Finally form the [pullback in a category](../../../../../pullback-category-theory.md) $E=P\times_CP'$ of the two projective presentations. Pulling back each of their [short exact sequences in an abelian category](../../../../../short-exact-sequence-in-an-abelian-category.md) gives

$$
0\longrightarrow K\longrightarrow E\longrightarrow P'\longrightarrow0,
\qquad
0\longrightarrow K'\longrightarrow E\longrightarrow P\longrightarrow0.
$$

Because each of $P'$ and $P$ is a [projective object in a category](../../../../../projective-object.md), the respective final [epimorphisms](../../../../../epimorphism.md) have sections: lift their identity morphisms through those epimorphisms. The usual [additive category](../../../../../additive-category.md) splitting argument identifies each middle object with the [biproduct](../../../../../biproduct.md) of its kernel and quotient. Explicitly, a kernel inclusion $j$ and section $s$ give the isomorphism $[j,s]$ from that biproduct to the middle object; $1-sq$ factors through $j$ and provides its inverse's kernel component. Hence

$$
E\cong K\oplus P',\qquad E\cong K'\oplus P,
$$

and we conclude the **[Schanuel lemma in an abelian category](../../../../../schanuel-lemma-in-an-abelian-category.md)**:

$$
\boxed{K\oplus P'\cong K'\oplus P.}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
