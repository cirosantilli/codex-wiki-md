<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Steinitz exchange lemma](../../../../../../../steinitz-exchange-lemma.md) states that if $u_1,\ldots,u_r$ are [linearly independent](../../../../../../../linear-independence.md) and $w_1,\ldots,w_s$ [span](../../../../../../../linear-span.md) a [vector space](../../../../../../../vector-space-split.md) $V$, then $r\leq s$ and some $r$ of the $w_j$ can be replaced by $u_1,\ldots,u_r$ while preserving the [spanning set](../../../../../../../spanning-set.md) property.

Here is the exchange argument. Suppose that after $k$ replacements, a [spanning set](../../../../../../../spanning-set.md) is

$$
u_1,\ldots,u_k,w_{k+1},\ldots,w_s,
$$

where the remaining $w_j$ have been relabelled if necessary. Express $u_{k+1}$ as a [linear combination](../../../../../../../linear-combination.md) of this family. At least one remaining $w_j$ has a nonzero [coefficient](../../../../../../../coefficient.md); otherwise $u_{k+1}$ belongs to the [span](../../../../../../../linear-span.md) of $u_1,\ldots,u_k$, contradicting [linear independence](../../../../../../../linear-independence.md). Relabel this entry $w_{k+1}$. Solving for $w_{k+1}$ shows that it lies in the [span](../../../../../../../linear-span.md) of

$$
u_1,\ldots,u_{k+1},w_{k+2},\ldots,w_s.
$$

The new family therefore still [spans](../../../../../../../linear-span.md) $V$. Starting at $k=0$ repeats this step until all $r$ independent [vectors](../../../../../../../vector.md) have been inserted. If $r>s$, after $s$ steps the next $u_{s+1}$ would lie in the [span](../../../../../../../linear-span.md) of $u_1,\ldots,u_s$, a contradiction. Thus $r\leq s$, and the construction proves the replacement assertion as well.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
