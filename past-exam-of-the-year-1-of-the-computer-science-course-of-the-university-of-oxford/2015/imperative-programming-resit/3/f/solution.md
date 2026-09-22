<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

If the [merge algorithm](../../../../../merge-algorithm.md) from part (b) is retained with a disjoint destination, use a [circular buffer](../../../../../circular-buffer.md) of $2n$ cells. Represent the live segment by its start modulo $2n$ and its length $n$. The other $n$ cells are free; the next merge needs at most $n$ output cells. Appending its output and advancing the live start releases exactly as many obsolete source cells. Logical run boundaries and copying indices are reduced modulo $2n$. The final sorted [sequence](../../../../../sequence.md) may wrap, in which case an [array rotation](../../../../../array-rotation.md) makes it contiguous. Thus

$$
\boxed{2n\text{ cells suffice while retaining the disjoint-output merge}.}
$$

This is also the worst-case requirement if all source cells must be retained until a whole disjoint merge has been written: the final two runs can have combined length $n$.

Under the question's literal wording, however, no [running time](../../../../../running-time.md) requirement or disjoint-output restriction is imposed on the modified implementation. The absolute smallest [array](../../../../../array-data-structure.md) is

$$
\boxed{n\text{ cells, with }O(1)\text{ auxiliary scalar storage}.}
$$

To achieve this, replace the disjoint-output merge by an [in-place merge](../../../../../in-place-merge.md): compare the next unread values of the two adjacent runs; when the second is smaller, save it in one scalar, shift the intervening first-run block right by one, and insert it before that block. This is a sorted merge using no extra [array](../../../../../array-data-structure.md). Its [loop invariant](../../../../../loop-invariant.md) is that the finished prefix is the sorted merge of the consumed portions and the two remaining runs stay sorted. Each step consumes one value, proving termination.

After merging the first two runs in place, rotate the merged prefix behind the untouched suffix. Three [array reversals](../../../../../array-reversal.md) implement this rotation with one scalar: reverse the merged prefix, reverse the suffix, then reverse the whole segment. The resulting live [sequence](../../../../../sequence.md) is exactly the one produced in part (c). Repeat the same run schedule until sorted. The shift and reversal loops respectively preserve the copied block and exchanged end pairs; their [loop variants](../../../../../loop-variant.md) are the unshifted length and half the unreversed length. The modification can be substantially slower, but preserves the [loop invariant](../../../../../loop-invariant.md) and decreasing run count from part (d). Fewer than $n$ cells cannot even hold the specified $n$ input entries. Thus $2n$ is the natural circular-workspace answer for the original merge primitive, while $n$ is attainable when minimizing storage over all implementations allowed by the stated time-free specification.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
