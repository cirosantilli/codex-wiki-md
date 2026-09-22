<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A one-dimensional commutative [formal group law](../../../../../../formal-group-law.md) over a ring $R$ is a series $F(X,Y)\in R[[X,Y]]$ satisfying

$$
F(X,0)=X,
\qquad F(X,Y)=F(Y,X),
\qquad F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

An isomorphism from $F$ to $G$ is a series $h(T)=uT+O(T^2)$ with $u\in R^*$ and

$$
h(F(X,Y))=G(h(X),h(Y)).
$$

Over a characteristic-zero field $K$, every such formal group is isomorphic to the additive formal group. Differentiate the associativity identity and define the invariant differential

$$
\omega_F(T)=\left(\frac{\partial F}{\partial Y}(T,0)\right)^{-1}dT.
$$

Termwise integration is possible in characteristic zero; the [formal logarithm](../../../../../../formal-logarithm.md)

$$
\log_F(T)=\int_0^T\omega_F
$$

has leading term $T$. Invariance of $\omega_F$ gives

$$
d\log_F(F(X,Y))=d\log_F(X)+d\log_F(Y),
$$

and evaluation at $(0,0)$ removes the integration constant. Hence $\log_F(F(X,Y))=\log_F(X)+\log_F(Y)$. Its unit linear coefficient gives a compositional inverse, so it is an isomorphism to $X+Y$. Therefore any two one-dimensional commutative formal groups over $K$ are isomorphic.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
