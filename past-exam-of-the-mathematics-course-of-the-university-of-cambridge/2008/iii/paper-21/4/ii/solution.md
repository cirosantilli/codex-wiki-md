<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose affine neighborhoods $U_0=\operatorname{Spec}A$ of $x$ and $V_0=\operatorname{Spec}B$ of $y$, and orient the given [local ring](../../../../../../local-ring.md) isomorphism as

$$
\alpha:B_{\mathfrak m_y}\longrightarrow A_{\mathfrak m_x}.
$$

Both algebras are finitely presented over $k$. Choose finitely many generators of $B$. Their images under $\alpha$ are fractions in $A$ whose denominators do not vanish at $x$. After inverting the product of those denominators, they define [regular functions](../../../../../../regular-function.md) on an affine open neighborhood of $x$. The finitely many defining relations of $B$ vanish as germs at $x$; each vanishes on a further open neighborhood. Shrinking finitely many times therefore turns those fractions into an actual algebra homomorphism $B\to\mathcal O(U_1)$, and hence a [morphism of algebraic varieties](../../../../../../morphism-of-algebraic-varieties.md) $F:U_1\to V_0$ inducing $\alpha$ on the [local rings](../../../../../../local-ring.md).

A local-ring isomorphism preserves the [maximal ideal](../../../../../../maximal-ideal.md). Its induced residue-field map is the identity of $k$, because it is a $k$-algebra map. Evaluating every coordinate generator consequently shows $F(x)=y$. Apply the identical finite-generator and finite-relation construction to $\alpha^{-1}$ to obtain $G:V_1\to U_0$ with $G(y)=x$.

On $U_2=U_1\cap F^{-1}(V_1)$ the composition $GF$ is defined, and on $V_2=V_1\cap G^{-1}(U_1)$ the composition $FG$ is defined. Their maps on [local rings](../../../../../../local-ring.md) are the identities. Thus the coordinate differences between $GF$ and the identity vanish as germs at $x$; finitely many coordinate generators allow us to shrink to $U_3\subseteq U_2$ on which $GF$ actually is the identity. Likewise shrink to $V_3\subseteq V_2$ on which $FG$ is the identity. Finally take

$$
U=U_3\cap F^{-1}(V_3),\qquad V=V_3\cap G^{-1}(U_3).
$$

These are open neighborhoods of the specified points. If $u\in U$, then $F(u)\in V_3$ and $G(F(u))=u\in U_3$, so $F(u)\in V$. Conversely, if $v\in V$, then $G(v)\in U_3$ and $F(G(v))=v\in V_3$, so $G(v)\in U$. Therefore the restrictions are mutual inverse regular maps, proving

$$
\boxed{F:U\xrightarrow{\ \sim\ }V,\qquad F(x)=y.}
$$

This proves [isomorphic local rings determine isomorphic neighborhoods](../../../../../../isomorphic-local-rings-determine-isomorphic-neighborhoods.md) using actual [regular functions](../../../../../../regular-function.md) and finite presentations. The conclusion concerns neighborhood isomorphisms, rather than just isomorphisms of formal completions.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
