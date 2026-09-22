<h1 id="9f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The 36 ordered outcomes are equiprobable. For $2\le s\le12$, let $c_s=6-|s-7|$ count outcomes with sum $s$. Then $\mathbb P(A_s)=c_s/36$ and $\mathbb P(B_i)=1/6$ for $1\le i\le6$. Their joint [probability](../../../../../../probability.md) is $1/36$ if $1\le s-i\le6$, and zero otherwise.

If the joint [probability](../../../../../../probability.md) is zero, independence is impossible in these ranges because both marginal probabilities are positive. If it is $1/36$, the [independent events](../../../../../../independent-events.md) condition requires $1/36=c_s/216$, or $c_s=6$. This happens only for $s=7$, and then all six values of $i$ allow the partner $7-i$. Therefore **within the possible sums and faces**

$$
\boxed{s=7,\qquad i\in\{1,2,3,4,5,6\}.}
$$

If arbitrary integer labels outside these ranges are included, an impossible sum or face defines an empty [event](../../../../../../event.md), which is trivially independent of every [event](../../../../../../event.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
