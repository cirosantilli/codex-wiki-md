<h1 id="1/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since the [radical of an ideal](../../../../../radical-of-an-ideal.md) $\sqrt{\mathfrak q}$ is $(r)$, some positive power of $r$ belongs to $\mathfrak q$. Choose the least such exponent $k$. Then $(r^k)\subseteq\mathfrak q$ and $r^j\notin\mathfrak q$ for $0\leq j<k$, with $r^0=1$ excluded because the [primary ideal](../../../../../primary-ideal.md) $\mathfrak q$ is proper.

Take $x\in\mathfrak q$. If $x\notin(r^k)$, choose the largest $j\in\{0,\ldots,k-1\}$ for which $x\in(r^j)$, and write $x=r^ju$. Maximality of $j$ implies $u\notin(r)=\sqrt{\mathfrak q}$: otherwise $x\in(r^{j+1})$, a contradiction, including when $j=k-1$. The [primary ideal](../../../../../primary-ideal.md) condition applied to $r^ju\in\mathfrak q$ therefore forces $r^j\in\mathfrak q$, contrary to the choice of $k$.

Consequently every $x\in\mathfrak q$ lies in $(r^k)$, and

$$
\boxed{\mathfrak q=(r^k),\qquad k=\min\{n\geq1:r^n\in\mathfrak q\}.}
$$

Together with [i](../i.md), this classifies the [primary ideals for a regular principal prime](../../../../../primary-ideals-for-a-regular-principal-prime.md). The exponent is unique: if $(r^k)=(r^{k+1})$, then $r^k=r^{k+1}c$, and cancellation of the [non-zero-divisor](../../../../../non-zero-divisor.md) $r^k$ would give $1=rc$, contradicting that $(r)$ is proper. No [Noetherian](../../../../../noetherian-ring.md) hypothesis is needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the commutative algebra course of the University of Oxford](../../../../split.md)
6. [Commutative algebra course of the University of Oxford](../../../../../commutative-algebra-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
