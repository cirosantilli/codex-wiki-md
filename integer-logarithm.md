# Integer logarithm

↑ **Parent:** [Logarithm](logarithm.md)

For [integers](integer-split.md) $b>1$ and $n>0$, the [integer logarithm](integer-logarithm.md) is the largest [nonnegative integer](natural-number.md) $i$ such that $b^i\leq n$. Equivalently,

$$
 b^i\leq n<b^{i+1},\qquad i=\lfloor\log_b n\rfloor.
$$

The equivalence follows from the monotonicity of [exponentiation](exponentiation.md) in its exponent and the definition of the [floor function](floor-function.md). For example, $3^4=81\leq100<243=3^5$, so the base-three [integer logarithm](integer-logarithm.md) of $100$ is $4$.

A multiplication loop maintains $p=b^i\leq n$ and accepts another factor $b$ while $pb\leq n$. [Repeated squaring](exponentiation-by-squaring.md) makes the search faster: precompute $b^{2^k}$ starting at $k=0$, and consider these factors in decreasing $k$. Include a factor when the accumulated product remains at most $n$. If $L=\lfloor\log_b n\rfloor$, the [loop invariant](loop-invariant.md) before considering $k$ is $i\leq L<i+2^{k+1}$. Accepting $2^k$ exactly when $i+2^k\leq L$ halves that uncertainty, proving the [greedy algorithm](greedy-algorithm.md) returns $L$. This takes $O(1+\log(1+\log_b n))$ arithmetic operations; it is not the same claim as this bound on [bit complexity](bit-complexity.md).

For positive operands in bounded [integer arithmetic](integer-arithmetic.md), test $p\leq n\mathbin{\mathrm{DIV}}q$ before multiplying by $q$. [Integer division](integer-division.md) makes this equivalent to $pq\leq n$ while preventing [integer overflow](integer-overflow.md) in a rejected candidate.

## ↑ Ancestors (8)

1. [Logarithm](logarithm.md)
2. [Exponential function](exponential-function.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Integer logarithm](integer-logarithm.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/1/a/solution.md)
