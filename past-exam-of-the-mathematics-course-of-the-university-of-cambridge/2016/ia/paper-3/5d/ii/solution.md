<h1 id="5d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**An example is the [unitriangular group of degree three over F3](../../../../../../unitriangular-group-of-degree-three-over-f3.md)**, consisting of

$$
M(a,b,c)=\begin{pmatrix}1&a&c\\0&1&b\\0&0&1\end{pmatrix},\qquad a,b,c\in\mathbb F_3.
$$

This is an [upper unitriangular group](../../../../../../upper-unitriangular-group.md) of order $3^3=27$. Direct [matrix multiplication](../../../../../../matrix-multiplication.md) gives

$$
M(a,b,c)M(a',b',c')=M(a+a',b+b',c+c'+ab').
$$

The formula gives closure, identity $M(0,0,0)$, and inverse $M(-a,-b,ab-c)$; associativity follows from [matrix multiplication](../../../../../../matrix-multiplication.md). The two elements $M(1,0,0)$ and $M(0,1,0)$ do not commute: their products have respectively $c=1$ and $c=0$.

Every element has the form $I+N$ with $N^3=0$. Since the [finite field](../../../../../../finite-field.md) $\mathbb F_3$ has characteristic three, the binomial expansion gives

$$
(I+N)^3=I+3N+3N^2+N^3=I.
$$

Hence every nonidentity element has order exactly three. **This is a nonabelian [finite group](../../../../../../finite-group.md) with [exponent of a finite group](../../../../../../exponent-of-a-finite-group.md) equal to three.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
