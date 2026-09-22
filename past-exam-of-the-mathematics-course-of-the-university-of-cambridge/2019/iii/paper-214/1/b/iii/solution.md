<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write

$$
q_n=\mathbb P_p(0\leftrightarrow\partial B(n)),
\qquad a_n=\mathbb P_p(0\leftrightarrow e_n).
$$

Since $e_n\in\partial B(n)$, $q_n\geq a_n$, and therefore

$$
\limsup_{n\to\infty}-\frac1n\log q_n\leq\phi(p).
$$

For the opposite inequality, choose $x=(n,x_2,\ldots,x_d)$ as in part (ii). Reflection about $x$ sends $0$ to $2ne_1$ and preserves the lattice. Thus the increasing events $\{0\leftrightarrow x\}$ and $\{x\leftrightarrow2ne_1\}$ have the same probability. The [FKG inequality](../../../../../../../fkg-inequality.md) yields

$$
a_{2n}\geq\mathbb P_p(0\leftrightarrow x)^2
\geq\left(\frac{q_n}{|\partial B(n)|}\right)^2.
$$

Consequently

$$
-\frac1n\log q_n
\geq-\frac1{2n}\log a_{2n}
-\frac1n\log|\partial B(n)|.
$$

The polynomial boundary-size estimate makes the last term tend to zero, while the first tends to $\phi(p)$. Hence

$$
\boxed{\lim_{n\to\infty}-\frac1n\log q_n=\phi(p).}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 214](../../../../paper-214-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
