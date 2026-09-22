# Set without natural density

↑ **Parent:** [Natural density](natural-density.md)

Include the positive [integers](integer-split.md) in $[1,2),[4,8),[16,32),[64,128),\ldots$, and exclude the intervening [integer intervals](integer-interval.md) and zero. Equivalently, include $[2^{2k},2^{2k+1})\cap\mathbb Z$ for $k\geq0$. Each included block is large enough to raise the running proportion; the following excluded block lowers it again.

With $C_A(N)=|A\cap\{0,\ldots,N-1\}|$, the exact boundary counts follow from a [geometric series](geometric-series.md):

$$
C_A(4^k)=\sum_{j=0}^{k-1}4^j=\frac{4^k-1}{3},\qquad C_A(2\cdot4^k)=\sum_{j=0}^k4^j=\frac{4^{k+1}-1}{3}.
$$

The first sum is empty at $k=0$. Dividing by the corresponding boundary, rather than using one denominator for both, gives

$$
\frac{C_A(4^k)}{4^k}=\frac13-\frac{1}{3\cdot4^k},\qquad\frac{C_A(2\cdot4^k)}{2\cdot4^k}=\frac23-\frac{1}{6\cdot4^k}.
$$

For example, $C_A(16)=1+4=5$, whereas $C_A(32)=1+4+16=21$, yielding proportions $5/16$ and $21/32$. For $4^k\leq N\leq2\cdot4^k$, the exact count is $(4^k-1)/3+N-4^k$; for $2\cdot4^k\leq N\leq4^{k+1}$ it stays $(4^{k+1}-1)/3$. Hence the proportion increases through each included block and decreases through each excluded block. These boundary [subsequences](subsequence.md) give the actual [limit inferior](limit-inferior.md) and [limit superior](limit-superior.md):

$$
\liminf_{N\to\infty}\frac{C_A(N)}N=\frac13,\qquad\limsup_{N\to\infty}\frac{C_A(N)}N=\frac23.
$$

Since these differ, $A$ has no [natural density](natural-density.md). Its [upper asymptotic density](upper-asymptotic-density.md) still records its largest limiting proportion.

## ↑ Ancestors (5)

1. [Natural density](natural-density.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Natural density](natural-density.md)
- [Upper asymptotic density](upper-asymptotic-density.md)
