<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For $a\in\{0,1\}$ define a typed transition term $D_a:\sigma\to\sigma$ by a nested Boolean choice:

$$
D_a=\lambda x:\sigma.
eq_\sigma,x,q_0,q_{\delta(q_0,a)}
\bigl(eq_\sigma,x,q_1,q_{\delta(q_1,a)}
\bigl(\cdots(eq_\sigma,x,q_{n-2},q_{\delta(q_{n-2},a)},q_{\delta(q_{n-1},a)})\cdots\bigr)\bigr).
$$

Here a Church Boolean acts as an if-then-else operator. The assumed behavior of $eq_\sigma$ gives $D_aq_i\equiv_\beta q_{\delta(q_i,a)}$.

For $w=a_1\cdots a_k$, put

$$
\mathbf w=\lambda x:\sigma.D_{a_k}(D_{a_{k-1}}(\cdots D_{a_1}x\cdots)),
$$

and use $\mathbf\epsilon=\lambda x.x$. Induction on the word length gives

$$
\boxed{\mathbf wq_0\equiv_\beta q_{\delta^*(q_0,w)}.}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
