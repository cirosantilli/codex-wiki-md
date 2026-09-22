<h1 id="7e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define

$$
B=\bigcap_{n=0}^{\infty}f^n(X),
\qquad A=X\setminus B.
$$

Certainly $f(B)\subseteq B$. If $y\in B$, then $y\in f(X)$ and has a unique predecessor $x$ because $f$ is injective. For every $n$, writing $y=f^{n+1}(z)$ and using uniqueness gives $x=f^n(z)$; hence $x\in B$ and $y\in f(B)$. Thus $f(B)=B$.

If $f(a)\in B$, its unique predecessor must lie in $B$, so $a\in B$; consequently $f(A)\subseteq A$. If a point belonged to every $f^n(A)$ for $n\geq1$, it would belong to $B$ and also to $f(A)\subseteq A$, which is impossible. Therefore

$$
\boxed{X=A\cup B,\qquad \bigcap_{n=1}^{\infty}f^n(A)=\varnothing,\qquad f(B)=B}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7E](../../7e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
