<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [balanced category](../../../../../balanced-category.md) is one in which every [morphism](../../../../../morphism.md) that is both a [monomorphism](../../../../../monomorphism.md) and an [epimorphism](../../../../../epimorphism.md) is an [isomorphism](../../../../../isomorphism.md). A [strong monomorphism](../../../../../strong-monomorphism.md) $m:A\to B$ is a monomorphism right orthogonal to all epimorphisms: whenever $e:X\to Y$ is epic and $a:X\to A$, $b:Y\to B$ satisfy $ma=be$, there is a unique $d:Y\to A$ with $de=a$ and $md=b$. A [regular monomorphism](../../../../../regular-monomorphism.md) is an [equalizer](../../../../../equaliser.md) of some parallel pair of morphisms. Its equalizer property supplies the indicated lift after epic cancellation, so every regular monomorphism is strong.

If every monomorphism is strong and $m:A\to B$ is also epic, apply strongness to the square whose left and right sides are both $m$, with horizontal arrows $1_A$ and $1_B$. The lift $d:B\to A$ satisfies $dm=1_A$ and $md=1_B$. Thus $m$ is invertible and the [category](../../../../../category-split.md) is balanced.

Conversely, suppose the category is balanced and has [pullbacks in a category](../../../../../pullback-category-theory.md). Given the lifting square above, form $P=A\times_B Y$ with projections $p:P\to Y$, $q:P\to A$. The pair $(a,e)$ gives $h:X\to P$ with $ph=e$, $qh=a$. The pullback of the [monomorphism](../../../../../monomorphism.md) $m$ is monic, so $p$ is monic. It is also epic: $rp=sp$ implies $re=se$, hence $r=s$ because $e$ is epic. Balancedness makes $p$ invertible. Now $d=qp^{-1}$ satisfies both required equations, and monicity of $m$ proves uniqueness. Hence **in a balanced category with pullbacks, every monomorphism is strong**.

For the finite example, choose a strong monomorphism $m:A\to B$ that is not regular. It is not an isomorphism, since an isomorphism is the equalizer of an identical pair. It is not epic either, since an epic strong monomorphism is invertible by the first argument. Consequently there are distinct arrows $r,s:B\rightrightarrows D$ with $rm=sm$. Since $m$ is not the equalizer of this pair, there is a map $h:X\to B$ with $rh=sh$ that does not factor through $m$. Monicity rules out failure of uniqueness, so failure of existence is the only possible failure of its equalizer property.

Define $\mathcal C_0$ to have four formally distinct objects $a,b,x,d$ and exactly the following six nonidentity arrows:

$$
m_0:a\to b,\quad h_0:x\to b,\quad r_0,s_0:b\rightrightarrows d,\quad k_0:a\to d,\quad l_0:x\to d.
$$

Their only nontrivial composites are

$$
r_0m_0=s_0m_0=k_0,\qquad r_0h_0=s_0h_0=l_0.
$$

There are no longer composable strings of nonidentity arrows, so these rules define an associative [category](../../../../../category-split.md). Sending $a,b,x,d$ to $A,B,X,D$, respectively, and the six arrows to $m,h,r,s,rm,rh$, defines a [functor](../../../../../functor.md). It is a [faithful functor](../../../../../faithful-functor.md): every hom-set has at most one arrow except $\mathcal C_0(b,d)=\{r_0,s_0\}$, and their images are distinct. Faithfulness does not require the four image objects to be distinct.

The map $m_0$ is monic, by direct inspection of arrows into $a$. Neither $m_0$ nor $h_0$ is epic, since the distinct pair $r_0,s_0$ agrees after either. Every other nonidentity arrow has target $d$ and is epic, because there is only one arrow out of $d$. A lifting square against $m_0$ whose left side is one of these epimorphisms would require an arrow $d\to b$, which does not exist. Squares whose left side is an identity have the evident unique lift. Thus $m_0$ is a [strong monomorphism](../../../../../strong-monomorphism.md).

It is not a [regular monomorphism](../../../../../regular-monomorphism.md). The only distinct parallel pair out of $b$ is $r_0,s_0$, and $h_0$ equalizes it but has no factorization through $m_0$, since there is no arrow $x\to a$. An identical pair has $1_b$ as its equalizer and cannot have the noninvertible $m_0$ as its equalizer. Therefore

$$
\boxed{\mathcal C_0\text{ has four objects, six nonidentity arrows, and a strong nonregular monomorphism}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
