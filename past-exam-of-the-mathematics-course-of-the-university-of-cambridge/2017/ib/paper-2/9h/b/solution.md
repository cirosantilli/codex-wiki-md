<h1 id="9h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the same multiplier convention, the [Lagrangian dual problem](../../../../../../lagrangian-dual-problem.md) is

$$
q(\lambda)=\inf_{x\in X}[f(x)+\lambda^T(b-g(x))],\qquad
\boxed{\sup_{\lambda\in\mathbb R^m}q(\lambda).}
$$

For every feasible $x$ and every $\lambda$, the equality constraint implies $q(\lambda)\le L(x,\lambda)=f(x)$. Taking first the infimum over feasible $x$ and then the supremum over $\lambda$ proves [weak duality](../../../../../../weak-duality.md):

$$
\boxed{d^*:=\sup_\lambda q(\lambda)\le p^*:=\inf_{x\in X,\ g(x)=b} f(x).}
$$

The inequalities remain meaningful with the usual extended-value conventions, including $q(\lambda)=-\infty$ when the Lagrangian is unbounded below. Equality of optimum values, or their attainment, does not follow from [weak duality](../../../../../../weak-duality.md). If the sufficient pair in part (a) exists, it attains equality, since $q(\lambda^*)=L(x^*,\lambda^*)=f(x^*)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9H](../../9h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
