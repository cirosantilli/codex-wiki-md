<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $M=\max_{p\in[0,1]}\mathbb E(1+pR)^r$ and choose an optimizer $p^*$. Existence follows from [continuity](../../../../../../continuous-function.md) and [compactness](../../../../../../compact-space.md): the integrands are dominated by a constant times $1+|R|$. Induction in the [Bellman equation](../../../../../../bellman-equation.md) gives

$$
\boxed{J_n(x)=x^rM^{N-n},\qquad p_n=p^*\text{ is optimal at every period}.}
$$

Thus the maximal expected yield is $\boxed{M^N-1}$. Neither current wealth nor time changes the maximizing fraction; there may be several optimizers.

The right [derivative](../../../../../../derivative.md) at $p=0$ is $r\mathbb ER$, using the finite first moment and dominated differentiation near zero. If $\mathbb ER>0$, increasing $p$ slightly improves on $p=0$, so $\boxed{p^*>0}$. No explicit value of $p^*$ is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
