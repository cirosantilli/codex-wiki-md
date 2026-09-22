<h1 id="14a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [closure](../../../../../../closure-topology.md) $\operatorname{cl}(A)$ is the intersection of all [closed subsets](../../../../../../closed-set.md) containing $A$; equivalently it consists of the points whose every open [neighbourhood](../../../../../../neighbourhood-mathematics.md) meets $A$.

Suppose $f$ is continuous and $x\in\operatorname{cl}(A)$. For any open [neighbourhood](../../../../../../neighbourhood-mathematics.md) $V$ of $f(x)$, [continuity](../../../../../../continuous-function.md) makes $f^{-1}(V)$ an open [neighbourhood](../../../../../../neighbourhood-mathematics.md) of $x$, so it meets $A$. Hence $V$ meets $f(A)$, showing $f(x)\in\operatorname{cl}(f(A))$. This proves $f(\operatorname{cl}(A))\subseteq\operatorname{cl}(f(A))$.

Conversely suppose this inclusion holds for every subset $A$. For a [closed subset](../../../../../../closed-set.md) $C\subseteq Y$, let $A=f^{-1}(C)$. Then $f(A)\subseteq C$ and therefore $\operatorname{cl}(f(A))\subseteq C$. By the assumed inclusion, $f(\operatorname{cl}(A))\subseteq C$, so $\operatorname{cl}(A)\subseteq f^{-1}(C)=A$. Since $A\subseteq\operatorname{cl}(A)$ always, $A$ is closed. Thus every [closed set](../../../../../../closed-set.md) has closed [preimage](../../../../../../preimage.md), equivalently every [open set](../../../../../../open-set.md) has open [preimage](../../../../../../preimage.md). This is [continuity](../../../../../../continuous-function.md), proving **the claimed equivalence**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14A](../../14a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
