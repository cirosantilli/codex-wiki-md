<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use two permanent [stacks](../../../../../stack-data-structure.md), $F$ and $B$, and one temporary [stack](../../../../../stack-data-structure.md), $T$. At operation boundaries $T$ is empty. Maintain the [representation invariant](../../../../../representation-invariant.md) that the [deque](../../../../../double-ended-queue.md), read from front to back, is the top-to-bottom contents of $F$ followed by the bottom-to-top contents of $B$. Thus the tops of $F$ and $B$ are the two accessible ends. Maintain their sizes using two counters, requiring only $O(1)$ additional storage in [Big O notation](../../../../../big-o-notation.md).

Adding at the front pushes onto $F$; adding at the back pushes onto $B$. Removing at an end whose permanent [stack](../../../../../stack-data-structure.md) is nonempty simply pops that [stack](../../../../../stack-data-structure.md). If both permanent [stacks](../../../../../stack-data-structure.md) are empty, report an empty [deque](../../../../../double-ended-queue.md).

Suppose a front removal finds $F$ empty and $B$ contains $m>0$ elements. Rebalance as follows:

- Move the top $\lfloor m/2\rfloor$ elements of $B$ onto $T$.
- Move all remaining $\lceil m/2\rceil$ elements of $B$ onto $F$.
- Move all elements of $T$ back onto $B$.
- Pop and return the top of $F$.

The parked elements are the back half of the [deque](../../../../../double-ended-queue.md); the unparked elements are the front half. Moving the front half onto $F$ reverses their [stack](../../../../../stack-data-structure.md) order and exposes the correct front element. Parking and restoring the back half reverses it twice, preserving its original order in $B$. The temporary [stack](../../../../../stack-data-structure.md) is empty again. For a back removal with $B$ empty, exchange the roles of $F$ and $B$ throughout. **Rebalance approximately half the elements, so both ends retain accessible elements after a large transfer.**

For the [amortized analysis](../../../../../amortized-analysis.md), count each push or pop as one unit and use the [potential method](../../../../../potential-method.md) with

$$
\Phi=3\bigl||F|-|B|\bigr|.
$$

Initially the [deque](../../../../../double-ended-queue.md) is empty, so $\Phi=0$, and $\Phi$ is always nonnegative. An ordinary insertion or removal costs one unit and changes the size difference by at most one, giving [amortized cost](../../../../../amortized-cost.md) at most $4$.

For a rebalancing removal, let $h=\lfloor m/2\rfloor$. The parked half makes two transfers per element and the other half makes one; each transfer is a pop and a push. Including the final removal, the actual cost is

$$
c=4h+2(m-h)+1=2m+2h+1\leq3m+1.
$$

Before rebalancing the absolute size difference is $m$. Immediately after the split it is at most $1$, and after the removal it is at most $2$. Hence

$$
\widehat c=c+\Delta\Phi\leq(3m+1)+3(2-m)=7.
$$

Size tests and counter updates change only these constants. Summing the [amortized costs](../../../../../amortized-cost.md) and using nonnegative final potential proves **$O(1)$ amortized running time for all four operations, with three [stacks](../../../../../stack-data-structure.md) and $O(1)$ additional storage**. An individual rebalancing operation can still take [linear time](../../../../../linear-time.md) in the current size.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
