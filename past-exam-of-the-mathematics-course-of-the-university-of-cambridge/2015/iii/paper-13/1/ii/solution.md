<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Kneser graph](../../../../../../kneser-graph.md) $KG(n,k)$ has the $k$-element subsets of $[n]$ as its [vertices](../../../../../../vertex-graph-theory.md); two [vertices](../../../../../../vertex-graph-theory.md) are adjacent exactly when the corresponding subsets are disjoint. The [Lovász theorem on Kneser graphs](../../../../../../lovasz-theorem-on-kneser-graphs.md) determines its [chromatic number](../../../../../../chromatic-number.md). A [graph colouring](../../../../../../graph-coloring.md) is therefore a partition of the $k$-sets into [intersecting families](../../../../../../intersecting-family.md).

First construct a [graph colouring](../../../../../../graph-coloring.md) with $d+2=n-2k+2$ colours. If a $k$-set meets $[d+1]$, give it the colour of its least element. Give every remaining $k$-set colour $d+2$. Two sets with one of the first $d+1$ colours share that colour's element. The last colour consists of $k$-sets in a $(2k-1)$-element ground set, so it too is an [intersecting family](../../../../../../intersecting-family.md). Thus $\chi(KG(n,k))\leq d+2$.

For the converse we establish the [Gale hemisphere lemma](../../../../../../gale-hemisphere-lemma.md) explicitly, using a signed [moment curve](../../../../../../moment-curve.md). Choose $t_1<\cdots<t_n$ and put

$$
w_i=(-1)^i(1,t_i,\ldots,t_i^d),\qquad v_i=w_i/\|w_i\|\in S^d.
$$

Every [open hemisphere](../../../../../../open-hemisphere.md) $\{v:x\cdot v>0\}$ contains at least $k$ labelled points $v_i$. To see this, put $p(t)=x_0+x_1t+\cdots+x_dt^d$. It is a nonzero [polynomial](../../../../../../polynomial-split.md) of [polynomial degree](../../../../../../degree-of-a-polynomial.md) at most $d$. First suppose none of the $p(t_i)$ vanishes. Write $b_i=\operatorname{sgn}((-1)^ip(t_i))$. If only $P\leq k-1$ of the $b_i$ were positive, the $N=n-P$ negative signs would occupy at most $P+1$ consecutive blocks. There would be at least

$$
N-(P+1)=n-2P-1\geq d+1
$$

adjacent pairs with both $b_i,b_{i+1}$ negative. Each such pair forces $p(t_i)$ and $p(t_{i+1})$ to have opposite signs. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) would give $d+1$ distinct [roots of a polynomial](../../../../../../root-of-a-polynomial.md), a contradiction.

If $p$ vanishes at $z$ of the sample points, then $z\leq d$. A [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) $q$ of [polynomial degree](../../../../../../degree-of-a-polynomial.md) at most $z-1$ can be chosen with $(-1)^iq(t_i)<0$ at all those points. For sufficiently small $\varepsilon>0$, the [polynomial](../../../../../../polynomial-split.md) $p+\varepsilon q$ keeps every previously nonzero sign, has no zero sample values, and makes every previously zero value negative after multiplication by $(-1)^i$. Its positive count is exactly the positive count of $p$, so the preceding argument proves the [open hemisphere](../../../../../../open-hemisphere.md) assertion also in this case. For $d=0$, the labelled points alternate between the two points of $S^0$; distinct labels, rather than distinct positions, are what is needed.

Suppose now that $KG(n,k)$ had a [graph colouring](../../../../../../graph-coloring.md) with at most $d+1$ colours, padding the palette with unused colours if necessary. For each colour $j$, let

$$
U_j=\bigcup_{\substack{A\subseteq[n],\ |A|=k\\A\text{ has colour }j}}
\{x\in S^d:x\cdot v_i>0\text{ for every }i\in A\}.
$$

These are [open sets](../../../../../../open-set.md), and the [Gale hemisphere lemma](../../../../../../gale-hemisphere-lemma.md) says that they cover $S^d$. If both $x$ and $-x$ belonged to $U_j$, two $k$-sets of colour $j$ would lie in opposite [open hemispheres](../../../../../../open-hemisphere.md). They would be disjoint, hence adjacent in the [Kneser graph](../../../../../../kneser-graph.md), contradicting the [graph colouring](../../../../../../graph-coloring.md). The [Lusternik-Schnirelmann-Borsuk theorem](../../../../../../lusternik-schnirelmann-theorem.md) excludes this cover. Therefore **the lower bound matches the explicit colouring**:

$$
\boxed{\chi(KG(n,k))=d+2=n-2k+2.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
