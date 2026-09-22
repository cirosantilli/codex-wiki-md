<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Lopsided Lovász local lemma](../../../../../../lopsided-lovasz-local-lemma.md) states that, for bad events $E_i$ with a lopsidependency graph, numbers $x_i\in[0,1)$ satisfying

$$
\mathbb P(E_i)\leq x_i\prod_{j\sim i}(1-x_j)
$$

imply $\mathbb P(\bigcap_iE_i^c)>0$.

Fix any $0<\eta<1/6$, put $N=\lfloor k^{4/3+\eta}\rfloor$, and sample $G(N,p)$ with

$$
p=aN^{-2/3},
$$

where $a>0$ is a sufficiently small absolute constant. Let $A_Q$ be the event that a specified copy $Q$ of $C_4$ is present, and let $B_S$ be the event that a specified $k$-set $S$ is independent. Then

$$
\mathbb P(A_Q)=p^4,
\qquad
\mathbb P(B_S)=(1-p)^{\binom k2}leq e^{-pk^2/3}=:q.
$$

For product measures, the standard monotone-event lopsidependency graph joins an increasing event $A_Q$ to a decreasing event $B_S$ only when they use a common edge. Events of the same monotonicity need no lopsidependency edge. Thus each $A_Q$ has at most $4\binom{N-2}{k-2}$ neighbours of type $B$, and each $B_S$ has at most $Ck^2N^2$ neighbours of type $A$.

Set $x_A=2p^4$ and $x_B=2q$. Since

$$
pk=k^{1/9-2\eta/3+o(1)}\gg\log k,
$$

we have

$$
\binom{N-2}{k-2}x_B=o(1).
$$

On the other side,

$$
Ck^2N^2x_A=O(a^4k^2N^{-2/3}),
$$

whereas $-\log q\geq(a/3)k^2N^{-2/3}$. Choosing $a$ small makes both local-lemma inequalities hold. There is therefore a graph on $N$ vertices containing no $C_4$ and no independent $k$-set. Taking, for example, $\eta=1/12$ proves

$$
\boxed{R(C_4,K_k)\geq\Omega(k^{4/3+1/12}).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
