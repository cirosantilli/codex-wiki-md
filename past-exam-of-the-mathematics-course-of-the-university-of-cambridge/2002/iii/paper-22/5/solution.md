<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $t:1\hookrightarrow\Omega$ for truth. Let $g:U\hookrightarrow\Omega$ be the [subobject](../../../../../subobject.md) classified by the [monomorphism](../../../../../monomorphism.md) $f$. Its classifier pullback gives $fg=t!_U$. The left side is monic, so $!_U:U\to1$ is monic as well: **$U$ is subterminal**.

Let $i:V\hookrightarrow U$ be classified by $g$. The pullback square for $i$ says that $V\to1$ is also the pullback of $g$ along $t$. Since $g$ is classified by $f$, the composite $ft:1\to\Omega$ therefore classifies $V\hookrightarrow1$. Pulling this [subobject](../../../../../subobject.md) back along $!_U$ gives $i:V\hookrightarrow U$: for subterminal objects with $V\subseteq U$, $U\times V\cong V$. Uniqueness of characteristic maps now gives $ft!_U=g$. Combining with $fg=t!_U$ proves

$$
\boxed{f^2g=ft!_U=g.}
$$

To deduce the full identity, let $u:1\to\Omega$ classify $U\hookrightarrow1$. The pullback of $g$ along $f$ is $t!_U:U\hookrightarrow\Omega$. Indeed $ft!_U=g$, and if $fa=gb$, monicity of $f$ forces $a=t!_Ub$, giving the universal property. The classifier of that pullback is $f^2$. But the [subobject](../../../../../subobject.md) $t!_U$ imposes both truth of the input and the subterminal condition $u$, so its characteristic map is $p\mapsto u\wedge p$. The meet operation here is defined using only [finite limits](../../../../../finite-limit.md) and the classifier. Thus $f^2=u\wedge(-)$. In particular $f^2t=u=f^2u$, by the unit and idempotence laws for meet. Since $f^2$ is monic, $t=u$, and hence

$$
\boxed{f^2=1_\Omega.}
$$

This proves the [monic endomorphism of a subobject classifier](../../../../../monic-endomorphism-of-a-subobject-classifier.md) property under exactly the stated finite-limit assumptions; no Boolean logic was used.

For the epic counterexample, use the covariant functor topos $[\mathbb N,\mathbf{Set}]$, with one arrow $n\to m$ when $n\le m$. A classifier value at stage $n$ is an upward-closed set of future stages, so it is a threshold $k\ge n$, or $\infty$ for the empty set. The transition from $n$ to $n+1$ sends $k$ to $\max(k,n+1)$ and fixes $\infty$. Define

$$
F_n(k)=\max(n,k-1),\qquad F_n(\infty)=\infty.
$$

For the transition to $n+1$, both composites send finite $k$ to $\max(n+1,k-1)$, so the maps are natural. Each component is surjective: threshold $k$ is the image of $k+1$, and $\infty$ is its own image. [Epimorphisms](../../../../../epimorphism.md) in a functor topos are objectwise surjective, so $F$ is epic. But $F_n(n)=F_n(n+1)=n$, making it noninjective and not invertible. Thus **the classifier has an epic endomorphism which is not an [isomorphism](../../../../../isomorphism.md)**, the [shift epimorphism of the natural-number presheaf classifier](../../../../../shift-epimorphism-of-the-natural-number-presheaf-classifier.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
