# Partition into distinct parts

↑ **Parent:** [Integer partition](integer-partition.md)

An [integer partition](integer-partition.md) with no repeated part. For example, the [partitions into distinct parts](partition-into-distinct-parts.md) of $5$ are $5$, $4+1$, and $3+2$. If $d(i,n)$ counts those with all parts at most $i$, separating those that omit $i$ from those that use it exactly once gives

$$
 d(i,n)=d(i-1,n)+d(i-1,n-i)
$$

for $i,n\geq1$, with $d(i,0)=1$, $d(0,n)=0$ for $n>0$, and negative remaining sums counted as zero. Removing the unique part $i$ gives a [bijection](bijection.md) proving the second term; retaining the same maximum $i$ there would instead allow repetitions.

## ↑ Ancestors (6)

1. [Integer partition](integer-partition.md)
2. [Set partition](set-partition.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
