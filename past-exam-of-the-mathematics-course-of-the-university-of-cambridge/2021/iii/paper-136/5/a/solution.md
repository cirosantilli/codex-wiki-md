<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A one-dimensional commutative [formal group law](../../../../../../formal-group-law.md) over a ring $R$ is a series $F(X,Y)\in R[[X,Y]]$ satisfying

$$
F(X,0)=X,
\qquad F(X,Y)=F(Y,X),
\qquad F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

The identity axiom gives $F(X,Y)=X+Y+$ terms of total degree at least two. Seek

$$
i(X)=-X+a_2X^2+a_3X^3+\cdots.
$$

After $a_2,\ldots,a_{n-1}$ have been chosen, the coefficient of $X^n$ in $F(X,i(X))$ is $a_n$ plus a known expression in the earlier coefficients. There is therefore a unique choice of $a_n$ making it zero. Recursion constructs the [formal inverse](../../../../../../formal-inverse.md) $i(X)$ with $F(X,i(X))=0$ and $i(X)\equiv-X\pmod{X^2}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
