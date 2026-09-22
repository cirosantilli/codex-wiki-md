<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\pi:F\to H$ send the free generators to the given presentation generators, and let $N=\ker\pi$, the [normal closure](../../../../../../normal-closure.md) of the relators $w_j$. The [Mihailova subgroup](../../../../../../mihailova-subgroup.md) here is exactly the [fiber product of groups](../../../../../../fiber-product-of-groups.md)

$$
\boxed{L=\{(u,v)\in F\times F:\pi(u)=\pi(v)\}.}
$$

To prove this equality, each specified generator belongs to the displayed fiber product, so $L$ is contained in it. The diagonal generators produce every $(a,a)$. Conjugating $(1,w_j)^{\pm1}$ by a diagonal element gives $(1,a^{-1}w_j^{\pm1}a)$; products give all $(1,n)$ for $n\in N$. Conversely, if $\pi(u)=\pi(v)$, then $u^{-1}v\in N$ and

$$
(u,v)=(u,u)(1,u^{-1}v)\in L.
$$

In particular $(1,w)\in L$ if and only if $w=1$ in $H$. Thus membership in this finitely generated subgroup is undecidable, despite the soluble [word problem for a group](../../../../../../word-problem-for-groups.md) in the ambient [direct product of groups](../../../../../../direct-product-of-groups.md) $F\times F$.

For an explicit finite presentation, use $a_i$ and $b_i$ for the first and second copies of the free basis. The base has presentation $\langle a_1,\ldots,a_m,b_1,\ldots,b_m\mid[a_i,b_j]=1\ (1\leq i,j\leq m)\rangle$. The pairs $(x_i,x_i)$ and $(1,w_j(x))$ are $a_ib_i$ and $w_j(b)$. Consequently the requested [HNN extension](../../../../../../hnn-extension.md) has the finite presentation

$$
\boxed{G=\left\langle a_1,\ldots,a_m,b_1,\ldots,b_m,t\ \middle|\
[a_i,b_j]=1,\ [t,a_ib_i]=1,\ [t,w_j(b)]=1\right\rangle.}
$$

Commutation with the displayed subgroup generators implies commutation with all their products and inverses, so these finitely many relations are exactly the specified centralizing extension. The associated subgroup is $L$ on both sides, and the associated isomorphism is the identity.

For an input word $w$ in the generators of $H$, form $p=w(b)\in P$ and the effectively constructed word

$$
W=t^{-1}ptp^{-1}.
$$

If $w=1$ in $H$, then $p=(1,w)\in L$ and $W=1$ by centralization. If $w\ne1$, then $p\notin L$; the displayed word contains stable letters and no [pinch in an HNN extension](../../../../../../pinch-in-an-hnn-extension.md), so [Britton's lemma](../../../../../../britton-s-lemma.md) gives $W\ne1$. This is the [centralizing HNN extension detects subgroup membership](../../../../../../centralizing-hnn-extension-detects-subgroup-membership.md) equivalence

$$
\boxed{W=1\text{ in }G\quad\Longleftrightarrow\quad w=1\text{ in }H.}
$$

A solution of the [word problem for a group](../../../../../../word-problem-for-groups.md) in $G$ would therefore solve that in $H$, a contradiction. **The finitely presented extension $G$ has insoluble word problem.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
