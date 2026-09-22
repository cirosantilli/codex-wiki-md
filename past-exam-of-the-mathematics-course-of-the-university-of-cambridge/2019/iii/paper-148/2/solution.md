<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The set $S=1+I$ is a [multiplicative subset](../../../../../multiplicatively-closed-set.md), since $(1+a)(1+b)=1+(a+b+ab)$. The [localization of a ring](../../../../../localization-of-a-ring.md) $S^{-1}R$ consists of fractions $r/s$, where

$$
\frac rs=\frac{r'}{s'}
\quad\Longleftrightarrow\quad
u(s'r-sr')=0\text{ for some }u\in S.
$$

Similarly, the [localization of a module](../../../../../localization-of-a-module.md) $S^{-1}M$ consists of fractions $m/s$, with the analogous equivalence relation. The canonical maps are

$$
R\longrightarrow S^{-1}R,\qquad r\longmapsto r/1,
\qquad
M\longrightarrow S^{-1}M,\qquad m\longmapsto m/1.
$$

The [Localization of a Noetherian ring](../../../../../localization-of-a-noetherian-ring.md) is Noetherian. Since a finitely generated module over a Noetherian ring is a [Noetherian module](../../../../../noetherian-module.md), localizing a finite generating set shows that $S^{-1}M$ is Noetherian over $S^{-1}R$.

The [prime ideal correspondence for localization](../../../../../prime-ideal-correspondence-for-localization.md) identifies $\operatorname{Spec}S^{-1}R$ with the primes $P\in\operatorname{Spec}R$ disjoint from $S$. Here

$$
P\cap(1+I)=\varnothing
\quad\Longleftrightarrow\quad
P+I\ne R,
$$

so the [spectrum of localization away from one plus an ideal](../../../../../spectrum-of-localization-away-from-one-plus-an-ideal.md) is

$$
\boxed{\operatorname{Spec}S^{-1}R\cong
\{P\in\operatorname{Spec}R:P+I\ne R\}.}
$$

An element $m$ maps to zero exactly when $(1+a)m=0$ for some $a\in I$. Such an equation gives $m=(-a)^jm\in I^jM$ for every $j$, proving one inclusion. Conversely, suppose $m\in\bigcap_{j\geq1}I^jM$. The [Artin-Rees lemma](../../../../../artin-rees-lemma.md) applied to $Rm\subseteq M$ says that for some $c$,

$$
I^nM\cap Rm=I^{n-c}(I^cM\cap Rm),\qquad n\geq c.
$$

Taking $n=c+1$ gives $m\in I(Rm)$, so $m=am$ for some $a\in I$. Then $(1-a)m=0$ and $1-a\in S$. Thus

$$
\boxed{\ker(M\to S^{-1}M)=\bigcap_{j\geq1}I^jM.}
$$

For failure without Noetherianity, take

$$
R=k[t^q:q\in\mathbb Q_{\geq0}],
\qquad I=(t^q:q>0).
$$

The strict chain $(t)\subsetneq(t^{1/2})\subsetneq(t^{1/4})\subsetneq\cdots$ shows that $R$ is not Noetherian. Since $t^q=(t^{q/2})^2$, one has $I^2=I$, and hence $\bigcap_jI^j=I\ne0$. But $R$ is an [integral domain](../../../../../integral-domain.md), so its localization map into $(1+I)^{-1}R$ is injective. This is the [non-Noetherian failure of the intersection formula for localization](../../../../../non-noetherian-failure-of-the-intersection-formula-for-localization.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 148](../../paper-148-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
