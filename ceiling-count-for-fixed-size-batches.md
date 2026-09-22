# Ceiling count for fixed-size batches

↑ **Parent:** [Ceiling function](ceiling-function.md)

Suppose $N$ is a nonnegative [integer](integer-split.md) count of items and each batch holds at most $k$ items, where $k$ is a positive [integer](integer-split.md). The smallest sufficient number of batches is

$$
b=\left\lceil\frac Nk\right\rceil.
$$

Indeed, $bk\geq N$ exactly when the [integer](integer-split.md) $b$ is at least $N/k$. If $N=0$, no batches are needed. If $N$ is a multiple of $k$, no partly filled batch is needed.

For $102$ items with capacity $20$ per batch, $b=\lceil5.1\rceil=6$. Five batches can be full and the sixth holds two items, leaving $6\cdot20-102=18$ unused places. This is a different question from the five complete groups counted by $\lfloor102/20\rfloor$.

<a id="image-endpoint-aware-integer-counts-and-six-twenty-place-batches-needed-for-102-items"></a>
![](integer-interval-and-batch-counts.png)

**[Figure 3](#image-endpoint-aware-integer-counts-and-six-twenty-place-batches-needed-for-102-items). Endpoint-aware integer counts and six twenty-place batches needed for 102 items**.

Writing the [Euclidean division](euclidean-division.md) $N=kq+r$, $0\leq r<k$, gives the equivalent rule $b=q$ when $r=0$, and $b=q+1$ when $r>0$. This explains the [ceiling function](ceiling-function.md)'s jump: one extra item beyond a complete multiple demands a whole additional batch. For exact [integer arithmetic](integer-arithmetic.md), the identity $b=\lfloor(N+k-1)/k\rfloor$ avoids a fractional intermediate value; an implementation still needs an [integer](integer-split.md) representation large enough to hold $N+k-1$.

## ↑ Ancestors (8)

1. [Ceiling function](ceiling-function.md)
2. [Floor and ceiling functions](floor-and-ceiling-functions.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Ceiling function](ceiling-function.md)
- [Floor and ceiling functions](floor-and-ceiling-functions.md)
- [Integer arithmetic](integer-arithmetic.md)
