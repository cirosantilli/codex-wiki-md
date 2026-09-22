<h1 id="10e/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Part (i) gives $\mathbb P(A)=2/3$. Since $\{X_1=0\}\subseteq A$ and has probability $1/2$,

$$
\boxed{\mathbb P(X_1=0\mid A)=\frac{1/2}{2/3}=\frac34}.
$$

Conditioned on $A$, a walk at one moves to zero with probability $3/4$ and to two with probability $1/4$. A walk at two must next move to one, since a move to three would violate $A$. If

$$
e_i=\mathbb E_i(T\mid A),
$$

first-step analysis gives

$$
e_1=1+\frac14e_2,
\qquad
e_2=1+e_1.
$$

Solving,

$$
\boxed{\mathbb E(T\mid A)=e_1=\frac53}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [10E](../../../10e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
