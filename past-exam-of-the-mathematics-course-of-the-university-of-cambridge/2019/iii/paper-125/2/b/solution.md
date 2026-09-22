<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A one-dimensional commutative [formal group law](../../../../../../formal-group-law.md) over a ring $R$ is a series $F(X,Y)\in R[[X,Y]]$ satisfying

$$
F(X,0)=X,
\qquad F(X,Y)=F(Y,X),
\qquad F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

An isomorphism $u:F\to G$ is a series $u(T)\in TR[[T]]$ with a compositional inverse and

$$
u(F(X,Y))=G(u(X),u(Y)).
$$

The multiplication series is defined recursively by $[0]_F=0$, $[1]_F=T$ and $[n+1]_F=F([n]_F,T)$, with the [formal inverse](../../../../../../formal-inverse.md) handling negative $n$. Its linear term is

$$
[n]_F(T)=nT+O(T^2).
$$

By the [invertible morphism criterion for formal group laws](../../../../../../invertible-morphism-criterion-for-formal-group-laws.md), it is an isomorphism exactly when its linear coefficient $n$ is a unit of $R$. Indeed, when $n\in R^\times$, recursive coefficient comparison constructs a unique compositional inverse; applying the morphism identity for $[n]_F$ shows that the inverse also respects $F$. Conversely, an invertible series must have a unit linear coefficient. Therefore

$$
\boxed{[n]_F\text{ is an isomorphism}\quad\Longleftrightarrow\quad n\in R^\times.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
