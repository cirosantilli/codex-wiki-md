<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In this one-dimensional setting, a commutative [formal group law](../../../../../../formal-group-law.md) over a commutative [ring](../../../../../../ring.md) $R$ is a [formal power series](../../../../../../formal-power-series.md) $F(X,Y)\in R[[X,Y]]$ with

$$
F(X,0)=X,\quad F(0,Y)=Y,\quad F(X,Y)=F(Y,X),\quad
F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

In particular $F(X,Y)=X+Y+$ terms of total degree at least two. There is a unique [formal inverse](../../../../../../formal-inverse.md) $i_F(T)=-T+O(T^2)$; coefficient recursion solves $F(T,i_F(T))=0$.

A morphism from [formal group law](../../../../../../formal-group-law.md) $F$ to $G$ is $f(T)\in TR[[T]]$ satisfying

$$
f(F(X,Y))=G(f(X),f(Y)).
$$

The [invertible morphism criterion for formal group laws](../../../../../../invertible-morphism-criterion-for-formal-group-laws.md) is

$$
\boxed{f\text{ is an isomorphism}\quad\Longleftrightarrow\quad f^{\prime}(0)\in R^{\times}.}
$$

Necessity follows by differentiating $g\circ f=T$ at zero for an inverse $g$. Conversely, write $f(T)=a_1T+a_2T^2+\cdots$ with $a_1$ a [unit](../../../../../../unit-in-a-ring.md). In constructing $g(T)=b_1T+b_2T^2+\cdots$, the coefficient of $T$ fixes $b_1=a_1^{-1}$; at degree $n$, the equation $f(g(T))=T$ has the form $a_1b_n+$ an already known expression $=0$. This determines every $b_n$ over $R$. The same construction gives an inverse on the other side, and uniqueness makes the two inverses agree. Finally apply $g$ to the morphism identity with $X=g(U),Y=g(V)$ to obtain

$$
g(G(U,V))=F(g(U),g(V)).
$$

Thus the inverse is itself a morphism of [formal group laws](../../../../../../formal-group-law.md), not merely an inverse [formal power series](../../../../../../formal-power-series.md). Over a general [ring](../../../../../../ring.md), nonzero derivative is insufficient: it must be a [unit](../../../../../../unit-in-a-ring.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
