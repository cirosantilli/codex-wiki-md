<h1 id="5d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To obtain a [countable closure under real polynomial roots](../../../../../../countable-closure-under-real-polynomial-roots.md), start with $B_0=\{1,\pi\}$ and explicitly retain previous elements at each stage:

$$
B_{n+1}=B_n\cup\phi(B_n),\qquad X=\bigcup_{n=0}^{\infty}B_n.
$$

Part (b) shows that $\phi$ takes [countable sets](../../../../../../countable-set.md) to [countable sets](../../../../../../countable-set.md); consequently all $B_n$ and then $X$ are countable by the [countable union of countable sets](../../../../../../countable-union-of-countable-sets.md) theorem. Also $1,\pi\in X$.

For a nonzero [polynomial](../../../../../../polynomial-split.md) $P(t)=c_0+\cdots+c_dt^d$ with all $c_j\in X$, choose stages $n_j$ containing the finitely many coefficients and put $N=\max_jn_j$. The inclusions $B_n\subseteq B_{n+1}$ ensure that every coefficient belongs to $B_N$. Every real [root of a polynomial](../../../../../../root-of-a-polynomial.md) $P$ therefore belongs to $\phi(B_N)\subseteq B_{N+1}\subseteq X$. **This [countable set](../../../../../../countable-set.md) $X$ has all the required properties.** Retaining $B_n$ explicitly avoids assuming the generally false inclusion $A\subseteq\phi(A)$: for example, $\phi(\{1\})$ does not contain $1$, since a nonzero [polynomial](../../../../../../polynomial-split.md) all of whose coefficients are one is positive at $1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5D](../../5d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
