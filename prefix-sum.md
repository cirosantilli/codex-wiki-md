# Prefix sum

↑ **Parent:** [Sum](sum.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prefix_sum)

A prefix sum stores the accumulated [sum](sum.md) through a specified position in a finite [sequence](sequence.md) or [array](array-data-structure.md). For inputs $a_1,\ldots,a_n$, include the [empty sum](empty-sum.md) $P_0=0$ and set

$$
P_m=\sum_{i=1}^m a_i,\qquad P_m=P_{m-1}+a_m\quad(1\leq m\leq n).
$$

For the original input $(4,-2,5,-1,3,-4)$, the prefix array including $P_0$ is $(0,4,2,7,6,9,5)$. A negative entry makes the accumulated [sum](sum.md) decrease; a prefix sum does not have to be monotone. Conversely, the original entry is recovered by [subtraction](subtraction.md): $a_m=P_m-P_{m-1}$.

The useful cancellation is that any contiguous block has [sum](sum.md)

$$
\boxed{\sum_{i=\ell}^r a_i=P_r-P_{\ell-1}\qquad(1\leq\ell\leq r\leq n).}
$$

Both prefixes include the entries before $\ell$; subtracting cancels those entries. In the example, the [sum](sum.md) from positions two through four is $-2+5-1=2$, recovered as $P_4-P_1=6-4$. The [arithmetic mean](arithmetic-mean.md) of that block is $2/3$, obtained by dividing its [sum](sum.md) by its length. Prefix sums therefore make many repeated questions about an unchanged [array](array-data-structure.md) cheap: reuse accumulated totals instead of resumming every block.

<a id="image-two-prefix-sums-recover-a-contiguous-block-by-subtraction"></a>
![](prefix-sum-range-cancellation.png)

**[Figure 10](#image-two-prefix-sums-recover-a-contiguous-block-by-subtraction). Two prefix sums recover a contiguous block by subtraction**. The original six-entry [array](array-data-structure.md) has negative as well as positive values. Highlighted entries two through four sum to two. Their accumulated endpoint values are $P_1=4$ and $P_4=6$, so $P_4-P_1=2$. The initial $P_0=0$ also handles a block beginning at the first entry without a separate arithmetic rule.

The sequential recurrence builds all $n+1$ prefixes in $O(n)$ [time complexity](time-complexity.md) and storage; each block query needs two reads and one [subtraction](subtraction.md), hence $O(1)$ [time complexity](time-complexity.md). These counts assume constant-cost arithmetic and access to [array](array-data-structure.md) entries. If one input changes, all later stored prefixes change, so this simple representation is most useful when queries outnumber updates. For [integer](integer-split.md) inputs, sufficient numeric capacity must be retained; with [floating-point arithmetic](floating-point-arithmetic-split.md), subtracting large nearby prefixes can lose relative accuracy for a small block total. The exact mathematical identity does not eliminate representation error.

The apparently sequential recurrence also motivates a [prefix scan](prefix-scan.md): [associativity](associative-property.md) permits a tree of partial calculations that yields all accumulated results in parallel. Guy E. Blelloch's 1990 technical report systematically develops this operation and its applications; its authored chapter version explains the two tree sweeps used to obtain all prefixes. [Blelloch, Prefix Sums and Their Applications, CMU-CS-90-190, November 1990](https://www.cs.cmu.edu/afs/cs.cmu.edu/project/scandal/public/papers/CMU-CS-90-190.html). [Blelloch, authored chapter version, §§1.1–1.2: sequential scans and parallel tree sweeps](https://www.cs.cmu.edu/~guyb/papers/Ble93.pdf).

**Table of contents**

- [Suffix sum](suffix-sum.md)
- [Prefix scan](prefix-scan.md)

## ↑ Ancestors (7)

1. [Sum](sum.md)
2. [Summation](summation.md)
3. [Addition](addition.md)
4. [Arithmetic](arithmetic-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Counting sort prefix ranges](counting-sort-prefix-ranges.md)
- [Difference array](difference-array.md)
- [Entringer number](entringer-number.md)
- [Entringer triangle](entringer-triangle.md)
- [Fenwick tree](fenwick-tree.md)
- [Golomb sequence](golomb-sequence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/30j/b/solution.md)
- [Prefix scan](prefix-scan.md)
- [Prefix sum](prefix-sum.md)
- [Rank query](rank-query.md)
- [Stable digit sort](stable-digit-sort.md)
- [Stable record placement in counting sort](stable-record-placement-in-counting-sort.md)
- [Sum of an eventually periodic sequence](sum-of-an-eventually-periodic-sequence.md)
