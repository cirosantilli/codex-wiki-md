<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A one-dimensional commutative [formal group law](../../../../../../formal-group-law.md) over $R$ is a power series $F(X,Y)\in R[[X,Y]]$ satisfying

$$
F(X,0)=X,qquad F(X,Y)=F(Y,X),qquad
F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

A homomorphism $\theta:\mathcal F\to\mathcal G$ is a series $\theta(T)\in TR[[T]]$ such that

$$
\theta(F(X,Y))=G(\theta(X),\theta(Y)).
$$

Write $\theta(T)=uT+O(T^2)$. If $u=\theta'(0)$ is a unit, recursive comparison of coefficients constructs a unique compositional inverse $\psi(T)\in TR[[T]]$ with $\psi(\theta(T))=T=\theta(\psi(T))$. Apply $\psi$ to the homomorphism identity and substitute $X=\psi(U)$, $Y=\psi(V)$ to obtain

$$
F(\psi(U),\psi(V))=\psi(G(U,V)).
$$

**Thus $\psi$ is a homomorphism from $\mathcal G$ to $\mathcal F$, so $\theta$ is an isomorphism.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
