# Natural density

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_density)

For a [set](set-split.md) $S$ of [nonnegative integers](natural-number.md), its natural density is the limiting proportion of the first $N$ [nonnegative integers](natural-number.md) that belong to $S$:

$$
d(S)=\lim_{N\to\infty}\frac{|S\cap\{0,\ldots,N-1\}|}{N},
$$

provided this [limit](limit-of-a-function.md) exists. Write $C_S(N)=|S\cap\{0,\ldots,N-1\}|$ for the counting [function](function-split.md). The numerator is a finite [cardinality](cardinality.md); the denominator is exactly $N$, including zero. Every existing [natural density](natural-density.md) lies between zero and one.

For the even [nonnegative integers](natural-number.md) $E=\{0,2,4,\ldots\}$, there are $m$ elements below $N=2m$ and $m+1$ below $N=2m+1$. Thus $C_E(N)=\lceil N/2\rceil$ using the [ceiling function](ceiling-function.md), and $d(E)=1/2$. For the [square numbers](square-number.md) $Q=\{0,1,4,9,\ldots\}$, the exact count for $N\geq1$ is

$$
C_Q(N)=\lfloor\sqrt{N-1}\rfloor+1,\qquad d(Q)=0.
$$

The [floor function](floor-function.md) counts the allowed indices $1,\ldots,\lfloor\sqrt{N-1}\rfloor$, and the extra one counts zero. At $N=10$, the [square numbers](square-number.md) below ten are $0,1,4,9$, so the proportion is $4/10$; at $N=100$, it is $10/100$. The count grows like the [square root](square-root.md) of $N$, while the denominator grows like $N$.

The [prime numbers](prime-number.md) also have [natural density](natural-density.md) zero. If $P$ is their [set](set-split.md), the [Prime number theorem](prime-number-theorem.md) gives $C_P(N)\sim N/\log N$, hence $C_P(N)/N\to0$. The [Prime number theorem](prime-number-theorem.md) is a substantial result about the count, rather than a consequence of the fact that there are infinitely many [prime numbers](prime-number.md). [Andrew V. Sutherland, MIT 18.785 lecture 16, Riemann's zeta function and the prime number theorem, 2025](https://math.mit.edu/classes/18.785/2025/LectureNotes16.pdf)

Why use [natural density](natural-density.md) when [cardinality](cardinality.md) already measures size? The even [nonnegative integers](natural-number.md), the [square numbers](square-number.md), and the [prime numbers](prime-number.md) all have the same countably infinite [cardinality](cardinality.md), yet their proportions among large initial [integer intervals](integer-interval.md) differ. [Natural density](natural-density.md) distinguishes frequent membership from sparse membership. Equivalently, under a [uniform distribution on a finite set](discrete-uniform-distribution.md) of $N$ possible [nonnegative integers](natural-number.md), $C_S(N)/N$ is the [probability](probability.md) of landing in $S$. A [set without natural density](set-without-natural-density.md) shows why this limiting proportion need not exist.

<a id="image-exact-proportions-below-n-even-integers-squares-and-an-alternating-block-set"></a>
![](natural-density-samples.png)

**[Figure 8](#image-exact-proportions-below-n-even-integers-squares-and-an-alternating-block-set). Exact proportions below N: even integers, squares, and an alternating-block set**. Every point uses the count in $\{0,\ldots,N-1\}$ divided by $N$, with zero included among the even [integers](integer.md) and [square numbers](square-number.md). The right panel marks exact block-boundary counts for a [set without natural density](set-without-natural-density.md). Its low and high proportions approach $1/3$ and $2/3$ along different [subsequences](subsequence.md).

**Table of contents**

- [Set without natural density](set-without-natural-density.md)
- [Upper asymptotic density](upper-asymptotic-density.md)
- [Full-density sequence](full-density-sequence.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Full-density sequence](full-density-sequence.md)
- [Limit superior](limit-superior.md)
- [Natural density](natural-density.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-108/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108/2/solution.md)
- [Set without natural density](set-without-natural-density.md)
- [Sparse peaks can determine a limit superior](sparse-peaks-can-determine-a-limit-superior.md)
- [Subsequential limit](subsequential-limit.md)
- [Upper asymptotic density](upper-asymptotic-density.md)
