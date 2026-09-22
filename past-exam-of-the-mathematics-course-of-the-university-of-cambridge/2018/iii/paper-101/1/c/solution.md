<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We first establish the [nilradical as the intersection of prime ideals](../../../../../../nilradical-as-the-intersection-of-prime-ideals.md):

$$
\operatorname{Nil}(A)=\bigcap_{\mathfrak p\in\operatorname{Spec}A}\mathfrak p.
$$

Every [nilpotent element](../../../../../../nilpotent.md) belongs to every [prime ideal](../../../../../../prime-ideal.md). In the other direction, if $a$ is not nilpotent, the [multiplicative subset](../../../../../../multiplicatively-closed-set.md) $T=\{1,a,a^2,\ldots\}$ avoids zero. By the [Zorn lemma](../../../../../../zorn-s-lemma.md), there is an [ideal](../../../../../../ideal.md) $J$ maximal among those disjoint from $T$. It is a [prime ideal](../../../../../../prime-ideal.md): if $uv\in J$ and neither $u$ nor $v$ belongs to $J$, then $J+(u)$ and $J+(v)$ each meet $T$. Multiplying elements in these two intersections gives an element of $T$ lying in $J$, a contradiction. Since $a\notin J$, this proves the identity. The identity also holds for the zero [ring](../../../../../../ring.md), with the intersection over an empty family interpreted as the whole [ring](../../../../../../ring.md).

A [Zariski-closed set](../../../../../../zariski-closed-set.md) $V_R(I)$ contains the image of $f$ exactly when

$$
I\subseteq\bigcap_{\mathfrak q\in\operatorname{Spec}S}\varphi^{-1}(\mathfrak q)
=\varphi^{-1}(\operatorname{Nil}(S))
=\sqrt{\ker\varphi}.
$$

The last equality follows because $\varphi(r)$ is a [nilpotent element](../../../../../../nilpotent.md) exactly when $r^n\in\ker\varphi$ for some $n\geq1$. Consequently the smallest [Zariski-closed set](../../../../../../zariski-closed-set.md) containing the image, namely its [closure](../../../../../../closure-topology.md), is

$$
\overline{f(\operatorname{Spec}S)}=V_R(\sqrt{\ker\varphi})=V_R(\ker\varphi).
$$

This is all of $\operatorname{Spec}R$ precisely when the [kernel of a ring homomorphism](../../../../../../kernel-of-a-ring-homomorphism.md) is contained in every [prime ideal](../../../../../../prime-ideal.md) of $R$. Hence

$$
\boxed{f(\operatorname{Spec}S)\text{ is dense in }\operatorname{Spec}R
\iff\ker\varphi\subseteq\operatorname{Nil}(R).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
