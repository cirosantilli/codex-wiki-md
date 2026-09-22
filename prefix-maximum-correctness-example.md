# Prefix maximum correctness example

↑ **Parent:** [Algorithm correctness](algorithm-correctness.md)

Given a nonempty finite [sequence](sequence.md) $a=(a_0,\ldots,a_{n-1})$ of [integers](integer-split.md), return its [maximum](maximum-of-a-subset-of-a-total-order.md) value. Represent the [sequence](sequence.md) by an [array](array-data-structure.md) whose contents remain unchanged during execution. The [precondition](precondition.md) requires an [integer](integer-split.md) length $n\geq1$ and exact, terminating [integer](integer-split.md) comparisons and [variable assignments](variable-assignment.md). The [postcondition](postcondition.md) for returned value $r$ is

$$
r\in\{a_i:0\leq i<n\}\quad\text{and}\quad a_i\leq r\ \text{for every }0\leq i<n.
$$

Thus the [output](output-computing.md) belongs to the [finite set](finite-set.md) of entries and is at least every entry. The contract permits ties and negative [integers](integer-split.md); it asks for a value, not the position of a particular occurrence. There is no [maximum](maximum-of-a-subset-of-a-total-order.md) of an empty [set](set-split.md) of [integers](integer-split.md), so empty [input](input-computer-science.md) is deliberately outside this [precondition](precondition.md). A service accepting empty [inputs](input-computer-science.md) needs a different [formal specification](formal-specification.md), such as a separate absent result.

This [Python](python-programming-language.md) implementation makes the [variable assignments](variable-assignment.md) explicit. Its index arithmetic models exact [integer](integer-split.md) arithmetic; fixed-width implementations additionally need enough index range for $n$:
```
def find_max(a):
    n = len(a)
    best = a[0]
    k = 1
    while k < n:
        if a[k] > best:
            best = a[k]
        k = k + 1
    return best
```
For the original [input](input-computer-science.md) $[3,1,4,4,2]$, initialization gives $k=1$ and $\mathrm{best}=3$. Reading $a_1=1$ keeps $3$; reading $a_2=4$ changes it to $4$; reading $a_3=4$ and $a_4=2$ keeps $4$. At successive condition checks, the pairs $(k,\mathrm{best})$ are $(1,3),(2,3),(3,4),(4,4),(5,4)$. The returned [maximum](maximum-of-a-subset-of-a-total-order.md) is $4$.

<a id="image-maximum-values-of-successive-prefixes-in-the-original-integer-array"></a>
![](prefix-maximum-invariant-trace.png)

**[Figure 5](#image-maximum-values-of-successive-prefixes-in-the-original-integer-array). Maximum values of successive prefixes in the original integer array**. Each row shows the processed prefix of $[3,1,4,4,2]$ immediately before checking $k<n$. Blue cells have been processed; grey cells have not. The [loop invariant](loop-invariant.md) records the [maximum](maximum-of-a-subset-of-a-total-order.md) of the blue entries, while the [loop variant](loop-variant.md) $n-k$ counts remaining entries. These are exact constructed execution states.

At each condition check, use the [loop invariant](loop-invariant.md)

$$
I:\qquad 1\leq k\leq n,\qquad \mathrm{best}=\max\{a_i:0\leq i<k\},
$$

together with the fact that the [input](input-computer-science.md) [array](array-data-structure.md) is unchanged. The prefix is the first $k$ entries of the [sequence](sequence.md), so its [finite set](finite-set.md) of values is nonempty. The [maximum](maximum-of-a-subset-of-a-total-order.md) need not be unique as an occurrence: the invariant concerns its value.

Initialization establishes $I$: $k=1$ and $\mathrm{best}=a_0$, the [maximum](maximum-of-a-subset-of-a-total-order.md) of a one-element [set](set-split.md). For preservation, suppose $I$ and $k<n$ hold. Then $a_k$ is a valid [array](array-data-structure.md) entry. Either the comparison replaces $\mathrm{best}$ with the larger value $a_k$, or it keeps a value at least $a_k$. Before increasing $k$, the resulting value is

$$
\max\bigl(\max\{a_i:0\leq i<k\},a_k\bigr)=\max\{a_i:0\leq i<k+1\}.
$$

The [variable assignment](variable-assignment.md) $k\gets k+1$ restores the complete [loop invariant](loop-invariant.md). Between the two [variable assignments](variable-assignment.md), the old prefix formula may temporarily be false; the [loop invariant](loop-invariant.md) is required at condition checks, not at every instruction.

At exit, $k\geq n$, while $I$ gives $k\leq n$. Hence $k=n$, and $I$ gives exactly the required [postcondition](postcondition.md). This establishes [partial correctness](partial-correctness.md). The preservation argument is [mathematical induction](mathematical-induction.md) on the number of completed iterations, covering every permitted [integer](integer-split.md) [sequence](sequence.md), rather than just the pictured [input](input-computer-science.md).

For [algorithm termination](algorithm-termination.md), the [loop variant](loop-variant.md) $V=n-k$ is a nonnegative [integer](integer-split.md) whenever $I$ holds. If $k<n$, then $V\geq1$. Every body terminates under the [precondition](precondition.md) and changes $V$ to $V-1$. Starting at $n-1$, it reaches zero after exactly $n-1$ iterations. For $n=1$, the initial value is already zero and the body is never entered. Together with [partial correctness](partial-correctness.md), this proves [total correctness](total-correctness.md).

Starting $\mathrm{best}$ at zero instead of $a_0$ fails on the original negative [input](input-computer-science.md) $[-7,-3,-3,-8]$: it returns zero, which is neither an entry nor the [maximum](maximum-of-a-subset-of-a-total-order.md) $-3$. Keeping $k=1$ forever preserves the correct initial prefix claim but loops forever when $n>1$; a [loop invariant](loop-invariant.md) alone does not ensure [algorithm termination](algorithm-termination.md). Using `>=` instead of `>` still returns the same [maximum](maximum-of-a-subset-of-a-total-order.md) value when entries tie, although a version returning a position would need an explicit tie rule.

## ↑ Ancestors (4)

1. [Algorithm correctness](algorithm-correctness.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Loop invariant](loop-invariant.md)
- [Loop variant](loop-variant.md)
