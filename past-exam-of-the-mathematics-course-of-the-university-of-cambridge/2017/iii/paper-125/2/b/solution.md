<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In this setting a [formal group law](../../../../../../formal-group-law.md) means a one-dimensional commutative series $F(X,Y)\in\mathcal O_K[[X,Y]]$ with

$$
F(X,0)=X,\quad F(0,Y)=Y,\quad F(X,Y)=F(Y,X),\quad
F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

These identities force $F(X,Y)=X+Y+$ terms of total degree at least two. There is a unique [formal inverse](../../../../../../formal-inverse.md) $i_F(T)=-T+O(T^2)$ with $F(T,i_F(T))=0$.

A morphism to another [formal group law](../../../../../../formal-group-law.md) $G$ is a series $h(T)=cT+O(T^2)$ satisfying $h(F(X,Y))=G(h(X),h(Y))$. The [invertible morphism criterion for formal group laws](../../../../../../invertible-morphism-criterion-for-formal-group-laws.md) is

$$
\boxed{h\text{ is an isomorphism over }\mathcal O_K\iff c\in\mathcal O_K^{\times}.}
$$

Necessity follows by comparing linear coefficients in $h^{-1}\circ h=T$. For sufficiency, solve recursively for a compositional inverse $j(T)=c^{-1}T+\cdots$: at every stage the new coefficient is obtained by dividing by the unit $c$, so all coefficients stay in $\mathcal O_K$. Applying $j$ to the morphism identity shows that $j$ is itself a [group homomorphism](../../../../../../group-homomorphism.md) of [formal group laws](../../../../../../formal-group-law.md).

In particular, the multiplication series satisfies $[n]_F(T)=nT+O(T^2)$. Since $p\nmid n$, the [multiplication isomorphism of a formal group law](../../../../../../multiplication-isomorphism-of-a-formal-group-law.md) makes $[n]_F$ invertible over $\mathcal O_K$. Its series and inverse converge on $\mathfrak m_K$, so multiplication by $n$ is bijective on $E_1(K)$, and on $E_1(L)$ for every finite extension $L/K$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
