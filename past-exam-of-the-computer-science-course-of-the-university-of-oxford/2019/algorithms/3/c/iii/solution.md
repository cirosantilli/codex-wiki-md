<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First discard duplicate input [sets](../../../../../../set-split.md), and let $m=|\mathcal F|$. If $m>2^k$, reject by part (i); this rejection can be encoded as the fixed no-instance $U=\{u\}$, $\mathcal F=\{\{u\}\}$, $k=0$ of the [set basis problem](../../../../../../set-basis-problem.md). Otherwise, represent each ground element $x$ by its incidence column

$$
\sigma(x)=\bigl(\mathbf1_{x\in B}\bigr)_{B\in\mathcal F}\in\{0,1\}^m.
$$

Keep one element from each class of equal columns. By repeatedly applying part (ii), this preserves the answer. The reduced number of elements $q$ satisfies

$$
\boxed{m\leq2^k,\qquad q\leq2^m\leq2^{2^k}.}
$$

Relabel these representatives and store their reduced incidence [matrix](../../../../../../matrix.md). Its $mq$ membership bits, the dimensions and $k$ have encoded length bounded solely by a computable [function](../../../../../../function-split.md) of $k$; the leading incidence bound is $2^{k+2^k}$. Thus this is a [kernelization](../../../../../../kernelization.md), even though it is not a polynomial kernel. Forming columns and grouping identical ones takes [polynomial time](../../../../../../polynomial-time.md) in the original explicit input length. To test $m>2^k$, compare bit lengths or truncate exponentiation at $m+1$; never construct an enormous $2^k$ merely to perform this preprocessing comparison.

For completeness, the bounded instance can be solved explicitly. Enumerate all ordered lists of $k$ [subsets](../../../../../../subset.md) of the $q$-element ground [set](../../../../../../set-split.md), allowing empty members to pad shorter bases. There are at most $2^{kq}$ such lists. For a candidate basis and each reduced input [set](../../../../../../set-split.md) $B$, form the [union](../../../../../../set-union.md) of every candidate basis [set](../../../../../../set-split.md) contained in $B$. If this [union](../../../../../../set-union.md) equals $B$, a representation exists; if it does not, no [union](../../../../../../set-union.md) of that candidate's members can represent $B$, because any member not contained in $B$ would add a forbidden element. Testing every $B$ therefore verifies a candidate in time polynomial in $m,q,k$.

The preprocessing is polynomial in the original input length, and the remaining search depends only on $k$. Hence **the [set basis problem](../../../../../../set-basis-problem.md) is [fixed-parameter tractable](../../../../../../fixed-parameter-tractability.md) with respect to $k$**. Empty input families and $k=0$ are covered by the same empty-[union](../../../../../../set-union.md) convention.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Algorithms](../../../../algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
