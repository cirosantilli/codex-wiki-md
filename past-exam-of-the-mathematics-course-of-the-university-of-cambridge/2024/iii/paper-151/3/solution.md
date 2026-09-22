<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $a,b\in I$, the [square-zero ideal](../../../../../square-zero-ideal.md) condition gives

$$
(1+a)(1+b)=1+a+b+ab=1+a+b,
\qquad (1+a)^{-1}=1-a.
$$

Thus the [square-zero unit subgroup](../../../../../square-zero-unit-subgroup.md) $1+I$ is abelian, and

$$
I_{\mathrm{add}}\longrightarrow1+I,
\qquad a\longmapsto1+a
$$

is a [group isomorphism](../../../../../group-isomorphism.md) from the [additive group](../../../../../additive-group.md) of $I$.

Use the specified [ring isomorphism](../../../../../ring-isomorphism.md) $R/I\cong\mathbb ZG$. For $x\in\mathbb ZG$, choose a lift $r\in R$ and define $x\cdot a=ra$ for $a\in I$. Two lifts differ by an element of $I$, whose product with $a$ vanishes, so this is well defined. Right multiplication is handled identically. The two actions commute by [associativity](../../../../../associative-property.md), making $I$ a [bimodule](../../../../../bimodule.md). If $u\in R$ lifts $g\in G$, then $u$ is a [unit](../../../../../unit-in-a-ring.md): a lift $v$ of $g^{-1}$ makes both $uv$ and $vu$ elements of $1+I$, hence units, and a ring element with both a left and a right inverse is invertible. Conjugation therefore defines

$$
g\cdot a=uau^{-1}.
$$

Changing $u$ by an element of $I$ does not change this expression because $I^2=0$. Moreover,

$$
u(1+a)u^{-1}=1+uau^{-1},
$$

so $a\mapsto1+a$ is an isomorphism of $\mathbb ZG$-modules for these [conjugation actions](../../../../../conjugation-action.md).

Let $R^\times\to(R/I)^\times$ be reduction on [unit groups](../../../../../unit-group.md), and define $U$ as the inverse image of the distinguished subgroup $G\subseteq(\mathbb ZG)^\times$. Every $g\in G$ has a unit lift by the preceding argument, and the kernel consists exactly of the units congruent to $1$, namely $1+I$. Multiplication in $R$ therefore gives the [group extension](../../../../../group-extension.md)

$$
1\longrightarrow1+I\longrightarrow U\longrightarrow G\longrightarrow1.
$$

Choose a set-theoretic section $s:G\to U$ with $s(1)=1$. Its [extension cocycle](../../../../../extension-cocycle.md)

$$
c(g,h)=s(g)s(h)s(gh)^{-1}\in1+I
$$

satisfies the [two-cocycle](../../../../../two-cocycle.md) identity by [associativity](../../../../../associative-property.md). A different section changes $c$ by a [group coboundary](../../../../../group-coboundary.md), so [second group cohomology classifies group extensions](../../../../../second-group-cohomology-classifies-group-extensions.md) gives a well-defined class

$$
x=[c]\in H^2(G,1+I).
$$

The same construction for $(R_1,I_1)$ gives $U_1$, an extension cocycle $c_1$, and $x_1=[c_1]\in H^2(G,1+I_1)$.

The answer to the final question is no. An abstract [ring isomorphism](../../../../../ring-isomorphism.md) $R_1\cong R$ need not carry the distinguished ideal $I_1$ to $I$, need not induce the identity under the two chosen identifications of the [quotient rings](../../../../../quotient-ring.md) with $\mathbb ZG$, and need not induce the prescribed $\mathbb ZG$-module isomorphism $\theta$. Hence it need not give an isomorphism of the two displayed [group extensions](../../../../../group-extension.md), so it imposes no equality $\phi(x_1)=x$. That equality does hold if the ring isomorphism has all three compatibility properties, because it then carries one extension cocycle to the other up to a [group coboundary](../../../../../group-coboundary.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 151](../../paper-151-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
