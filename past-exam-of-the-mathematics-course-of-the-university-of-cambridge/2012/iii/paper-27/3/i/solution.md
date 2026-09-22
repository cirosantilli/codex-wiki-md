<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the one-dimensional commutative convention, a [formal group law](../../../../../../formal-group-law.md) over $R$ is a [formal power series](../../../../../../formal-power-series.md) $F(X,Y)=X+Y+\text{terms of degree at least two}$ satisfying $F(X,0)=X$, $F(0,Y)=Y$, $F(X,Y)=F(Y,X)$ and $F(F(X,Y),Z)=F(X,F(Y,Z))$. The [formal inverse](../../../../../../formal-inverse.md) is a series $I(T)=-T+O(T^2)$ with $F(T,I(T))=0$. For $R=\mathbb Z_p$ all these series converge on $p\mathbb Z_p$, which becomes a group with operation $F$.

Repeated formal addition gives the [multiplication isomorphism of a formal group law](../../../../../../multiplication-isomorphism-of-a-formal-group-law.md) $[n]_F(T)=nT+O(T^2)$. If $p\nmid n$, the coefficient $n$ is a unit in the [p-adic integers](../../../../../../p-adic-integer.md). We can construct an inverse $H(T)=n^{-1}T+\sum_{j\geq2}h_jT^j$ by coefficient recursion. At degree $j$, the equation $[n]_F(H(T))=T$ has the form $nh_j+\text{known integral terms}=0$; dividing by the unit $n$ keeps $h_j$ integral. The inverse is two-sided by uniqueness of formal composition inverses. Since integral coefficients multiplied by successive powers of $t\in p\mathbb Z_p$ tend to zero, both series converge on that set and their formal identities hold there. This proves [prime-to-residue-characteristic multiplication on a formal group](../../../../../../prime-to-residue-characteristic-multiplication-on-a-formal-group.md):

$$
\boxed{[n]_F:F(p\mathbb Z_p)\xrightarrow{\sim}F(p\mathbb Z_p),\qquad p\nmid n.}
$$

The argument also applies at $p=2$ for odd $n$; it does not require a logarithm or torsion-freeness.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
