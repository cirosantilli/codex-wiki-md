<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $f$ is a continuous bijection $\mathbb R\to\mathbb R$, it is a Borel isomorphism. Conditional on $X_{-i}=x_{-i}$, the $i$th coordinate of $F(X)$ has the pushforward of $\pi(dx_i\mid x_{-i})$ under $f$. Therefore applying one $K$-update and then $F$ has exactly the same law as applying one $Q$-update to $F(x)$, using the same random coordinate.

Formally, for every Borel set $A$,

$$
Q(F(x),A)=K(x,F^{-1}(A)).
$$

Composition preserves this conjugacy, so induction on $t$ gives

$$
Q^t(F(x),A)=K^t(x,F^{-1}(A)).
$$

Hence

$$
\boxed{Y\sim K^t(x,\cdot)\implies F(Y)\sim Q^t(F(x),\cdot).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
