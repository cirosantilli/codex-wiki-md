<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A one-dimensional commutative [formal group law](../../../../../../formal-group-law.md) over $\mathcal O_K$ is a power series $F(X,Y)\in\mathcal O_K[[X,Y]]$ satisfying

$$
F(X,0)=X,
\qquad F(X,Y)=F(Y,X),
\qquad F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

A morphism $h:\mathcal F\to\mathcal G$ is a series $h(T)\in T\mathcal O_K[[T]]$ satisfying

$$
h(F(X,Y))=G(h(X),h(Y)).
$$

If $h(T)=uT+O(T^2)$, the [invertible morphism criterion for formal group laws](../../../../../../invertible-morphism-criterion-for-formal-group-laws.md) says that $h$ is an isomorphism whenever $u\in\mathcal O_K^\times$. Indeed, recursive coefficient comparison constructs a unique compositional inverse $j(T)$; applying $j$ to the morphism identity shows that $j$ is a morphism in the opposite direction.

The multiplication series has

$$
[n]_{\mathcal F}(T)=nT+O(T^2).
$$

Since $p\nmid n$, its linear coefficient is a unit, so $[n]_{\mathcal F}$ is an automorphism of the group $\mathcal F(\pi\mathcal O_K)$. Its kernel is therefore zero, and

$$
\boxed{\mathcal F(\pi\mathcal O_K)[n]=0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
