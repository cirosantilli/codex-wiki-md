<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First the [expected value](../../../../../../../expected-value-split.md) of the [absorption time](../../../../../../../absorption-time.md) is finite. From any interior state, consecutive leftward moves lead to absorption within at most $n$ steps, with [probability](../../../../../../../probability.md) at least $p=3^{-n}$. By [independence](../../../../../../../independent-random-variables.md) of the subsequent steps, the [probability](../../../../../../../probability.md) of surviving $jn$ steps is at most $(1-p)^j$. Summing this [geometric series](../../../../../../../geometric-series.md) bounds the [expected value](../../../../../../../expected-value-split.md) of the [absorption time](../../../../../../../absorption-time.md) by $n/p$.

Now apply [first-step analysis](../../../../../../../first-step-analysis.md). Starting from $k$ in the interior, one step is always used. Conditional on that step, the remaining [expected values](../../../../../../../expected-value-split.md) are $e_{k+1}$, $e_k$, and $e_{k-1}$, each with [probability](../../../../../../../probability.md) $1/3$. The [law of total expectation](../../../../../../../law-of-total-expectation.md) therefore gives

$$
e_k=1+\frac13e_{k+1}+\frac13e_k+\frac13e_{k-1}.
$$

The term $1$ remains even when the particle stays at $k$, because a step has elapsed. Rearranging gives

$$
\boxed{\frac13e_{k+1}-\frac23e_k+\frac13e_{k-1}=-1,\qquad 1\leq k\leq n-1.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
