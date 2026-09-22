<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A one-dimensional commutative [formal group law](../../../../../../formal-group-law.md) over $\mathcal O_K$ is a power series $F(X,Y)\in\mathcal O_K[[X,Y]]$ satisfying

$$
F(X,0)=X,
\quad F(0,Y)=Y,
\quad F(F(X,Y),Z)=F(X,F(Y,Z)),
\quad F(X,Y)=F(Y,X).
$$

For $r\geq1$, the ideal $\pi^r\mathcal O_K$ becomes a group, denoted $F(\pi^r\mathcal O_K)$, under $x+_Fy=F(x,y)$; convergence follows because both inputs lie in the maximal ideal.

Over the characteristic-zero field $K$, there is a unique [formal logarithm](../../../../../../formal-logarithm.md)

$$
\log_F(T)=T+O(T^2)
$$

satisfying $\log_F(F(X,Y))=\log_F(X)+\log_F(Y)$. Its coefficients have bounded denominator growth, so for sufficiently large $r$ both $\log_F$ and its inverse [formal group exponential](../../../../../../formal-group-exponential.md) converge on $\pi^r\mathcal O_K$ and preserve that ideal. They give

$$
F(\pi^r\mathcal O_K)\simeq(\pi^r\mathcal O_K,+)\simeq(\mathcal O_K,+),
$$

where the final isomorphism is multiplication by $\pi^{-r}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
