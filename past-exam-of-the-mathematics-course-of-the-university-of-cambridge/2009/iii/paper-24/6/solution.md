<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Work internally with the [Heyting algebra](../../../../../heyting-algebra.md) $\Omega$ and the truth value $u$ of $U\hookrightarrow1$. For $o(u)(p)=u\Rightarrow p$, the identities

$$
u\Rightarrow\top=\top,\quad p\le u\Rightarrow p,\quad u\Rightarrow(p\wedge q)=(u\Rightarrow p)\wedge(u\Rightarrow q),\quad u\Rightarrow(u\Rightarrow p)=(u\wedge u)\Rightarrow p=u\Rightarrow p
$$

prove that it is an [open local operator](../../../../../open-local-operator.md).

For a [monomorphism](../../../../../monomorphism.md) $m:S\hookrightarrow X$ with characteristic map $\chi$, density means $u\Rightarrow\chi=\top$, equivalently $u\le\chi$. This says exactly that $U\times X$ is contained in $S$, or that the pullback mono $U\times S\to U\times X$ is invertible. Consequently

$$
\boxed{m\text{ is }o(U)\text{-dense}\iff U^*(m)\text{ is an isomorphism}.}
$$

An object $X$ is an $o(U)$-sheaf exactly when the canonical map $\eta_X:X\to X^U$, taking a value to its constant function on $U$, is invertible. Indeed $T\times U\hookrightarrow T$ is dense for every $T$. The sheaf condition makes $\mathcal E(T,X)\to\mathcal E(T\times U,X)\cong\mathcal E(T,X^U)$ bijective for every $T$, which proves $\eta_X$ invertible by the [Yoneda lemma](../../../../../yoneda-lemma.md). Conversely, if $\eta_X$ is invertible and $m:S\hookrightarrow T$ is dense, the isomorphism $S\times U\cong T\times U$ gives

$$
\mathcal E(T,X)\cong\mathcal E(T\times U,X)\cong\mathcal E(S\times U,X)\cong\mathcal E(S,X),
$$

so $X$ is a sheaf.

The pullback [functor](../../../../../functor.md) $L:\mathcal E\to\mathcal E/U$ has right adjoint $\Pi_U$, sending $A\to U$ to $A^U$. Every map $X\times U\to A$ is automatically over $U$, since $U$ is [subterminal object](../../../../../subterminal-object.md), proving this adjunction directly. Its counit $U\times A^U\to A$ is evaluation and is invertible. The inverse sends $a\in A$ to its image in $U$ together with the constant function $U\to A$ of value $a$; all elements of $U$ agree, so the composites are identities. The right adjoint is therefore full and faithful, and its image consists of objects fixed by $X\to X^U$. The sheaf characterization above proves

$$
\boxed{\mathbf{sh}_{o(U)}(\mathcal E)\simeq\mathcal E/U.}
$$

For a general [local operator](../../../../../lawvere-tierney-topology.md) $j$, its [dense monomorphism classifier](../../../../../dense-monomorphism-classifier.md) is the ordered [subobject](../../../../../subobject.md)

$$
J=\{p\in\Omega:jp=\top\}\hookrightarrow\Omega.
$$

A mono is [j-dense](../../../../../j-dense-monomorphism.md) exactly when its characteristic map factors through $J$. If $j=o(u)$, then $J=\{p:u\le p\}$, which has least element $u$. This is least internally over every parameter object, not just among global points.

Conversely suppose a global $u:1\to J$ is internally least. Upward closure of $J$ gives $jp=\top$ exactly when $u\le p$, in every context. For $S\hookrightarrow X$ let $\overline S$ be its $j$-closure, with characteristic predicate $jp$. The mono $S\hookrightarrow\overline S$ is dense: restricting $jp$ to $\overline S$ gives truth. Its characteristic map therefore lands in $J$, so leastness of $u$ gives $U\cap\overline S\subseteq S$. Internally this is

$$
u\wedge jp\le p,\qquad\text{hence }jp\le u\Rightarrow p.
$$

On the other hand $ju=\top$, and applying $j$ to $u\wedge(u\Rightarrow p)\le p$ gives $j(u\Rightarrow p)\le jp$. Inflationarity then gives $u\Rightarrow p\le jp$. Both inequalities yield

$$
\boxed{J\text{ has a least element }u\iff j=o(U),\qquad j(p)=u\Rightarrow p.}
$$

This proves the [least dense truth characterizes an open local operator](../../../../../least-dense-truth-characterizes-an-open-local-operator.md) criterion without replacing its internal order condition by the weaker condition on global truth values.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
