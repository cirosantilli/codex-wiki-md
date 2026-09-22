<h1 id="40e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The $m$th [Krylov subspace](../../../../../../krylov-subspace.md) is

$$
\boxed{
\mathcal K_m(A,v)
=\operatorname{span}\{v,Av,\ldots,A^{m-1}v\}
}.
$$

Because $A$ has a complete eigenbasis, decompose

$$
v=v_1+\cdots+v_s,
$$

where $v_j$ is the projection of $v$ onto the eigenspace belonging to the $j$th distinct eigenvalue $\lambda_j$; some $v_j$ may vanish. Then

$$
A^kv=\sum_{j=1}^s\lambda_j^kv_j.
$$

Every generator of $\mathcal K_m(A,v)$ therefore belongs to $\operatorname{span}\{v_1,\ldots,v_s\}$, and

$$
\boxed{\dim\mathcal K_m(A,v)\leq s\quad\text{for every }m}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40E](../../40e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
