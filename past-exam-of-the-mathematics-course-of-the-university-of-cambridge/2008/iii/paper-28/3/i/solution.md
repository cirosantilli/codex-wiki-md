<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A one-dimensional commutative [formal group law](../../../../../../formal-group-law.md) over the [p-adic integers](../../../../../../p-adic-integer.md) is a power series $\mathcal F(X,Y)\in\mathbb Z_p[[X,Y]]$ with

$$
\mathcal F(X,0)=X,\quad \mathcal F(0,Y)=Y,\quad
\mathcal F(X,Y)=\mathcal F(Y,X),
$$



$$
\mathcal F(\mathcal F(X,Y),Z)=\mathcal F(X,\mathcal F(Y,Z)).
$$

Its linear part is $X+Y$, and it has a unique [formal inverse](../../../../../../formal-inverse.md) $i(T)=-T+O(T^2)$ satisfying $\mathcal F(T,i(T))=0$. A formal-group homomorphism is a series $h(T)\in T\mathbb Z_p[[T]]$ satisfying $h(\mathcal F(X,Y))=\mathcal F(h(X),h(Y))$.

Define $[n](T)$ by adding $T$ to itself $n$ times with the [formal group law](../../../../../../formal-group-law.md). Induction on the linear part gives

$$
[n](T)=nT+O(T^2).
$$

Associativity and commutativity make $[n]$ a formal-group homomorphism. Since $p\nmid n$, its linear coefficient is a unit in $\mathbb Z_p$. We now construct its [compositional inverse of a formal power series](../../../../../../compositional-inverse-of-a-formal-power-series.md), rather than merely assert that the nonzero coefficient is sufficient.

Write $[n](T)=nT+a_2T^2+\cdots$ and seek $g(T)=b_1T+b_2T^2+\cdots$ with $[n](g(T))=T$. The degree-one coefficient gives $b_1=n^{-1}$. At degree $k\ge2$, the coefficient is $nb_k$ plus a polynomial in the already chosen $b_1,\ldots,b_{k-1}$ and $a_2,\ldots,a_k$. Division by the unit $n$ uniquely chooses $b_k\in\mathbb Z_p$. This recursively constructs $g$ over the same ring. A right inverse is constructed in the same way; associativity of composition identifies it with $g$, so $g\circ[n]=[n]\circ g=T$.

To prove that $g$ respects the group law, apply $[n]$ to the two candidate series:

$$
[n]\bigl(\mathcal F(g(X),g(Y))\bigr)
=\mathcal F(X,Y)
=[n]\bigl(g(\mathcal F(X,Y))\bigr).
$$

Cancel by composing with $g$. The result is $\mathcal F(g(X),g(Y))=g(\mathcal F(X,Y))$. Thus

$$
\boxed{[n]:\mathcal F\longrightarrow\mathcal F\text{ is an isomorphism over }\mathbb Z_p.}
$$

This is the [multiplication isomorphism of a formal group law](../../../../../../multiplication-isomorphism-of-a-formal-group-law.md), a special case of the [invertible morphism criterion for formal group laws](../../../../../../invertible-morphism-criterion-for-formal-group-laws.md). If $p\mid n$, its linear coefficient is not a unit, so the same isomorphism assertion would fail.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
