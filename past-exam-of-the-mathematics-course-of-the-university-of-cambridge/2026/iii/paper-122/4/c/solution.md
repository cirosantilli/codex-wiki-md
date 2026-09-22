<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The assertion as printed is false for unrestricted part sizes. Take $|A|=2$, let every vertex of $B$ be adjacent to one fixed vertex of $A$ and to no other vertex of $A$, and put $p=1/2$. The graph has $e(G)=p|A||B|$, but for $t=2$ the two distinct vertices of $A$ have no common neighbour, contradicting the claimed positive lower bound.

The corrected [common-neighbourhood sampling bound](../../../../../../common-neighbourhood-sampling-bound.md), which is sufficient for the requested Ramsey consequence, assumes $|A|$ is sufficiently large compared with $t^2/p$. Indeed, averaging over uniformly chosen ordered distinct $x_1,\ldots,x_t\in A$ gives

$$
\mathbb E|N(x_1)\cap\cdots\cap N(x_t)|
=\sum_{y\in B}\frac{(d(y))_t}{(|A|)_t}.
$$

Convexity and $\sum_y d(y)\geq p|A||B|$ imply that this is at least

$$
|B|\left(p-\frac{t-1}{|A|}\right)^t.
$$

If $|A|\geq4t^2/p$, then $(1-(t-1)/(p|A|))^t\geq1/2$, yielding the intended $p^t|B|/2$ bound with distinct vertices.

Now red-blue colour $K_N$, where $N=Ct2^t$, and split its vertices into equal parts $A,B$. One colour has cross-density at least $p=1/2$; call it red. Here $|A|\gg t^2$, so the corrected bound supplies $t$ vertices of $A$ having at least

$$
2^{-t}|B|/2\geq t
$$

common red neighbours when $C$ is large. Choosing any $t$ of those neighbours gives a red $K_{t,t}$. Hence

$$
\boxed{R(K_{t,t})=O(t2^t).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
