<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

Complete the random assignment by assigning passenger $N$ to the one vacant seat. This turns the uniformly random seating of the first $N-1$ passengers into a uniformly random [permutation](../../../../../permutation.md) of all $N$ passengers. Following an occupant to the seat on their ticket traverses precisely the cycle containing $N$; the process ends at the initially vacant seat.

The [cycle length of a tagged element in a uniform permutation](../../../../../cycle-length-of-a-tagged-element-in-a-uniform-permutation.md) is uniform on $\{1,\ldots,N\}$. Indeed, for length $\ell$, its count is $\binom{N-1}{\ell-1}(\ell-1)!(N-\ell)!=(N-1)!$, out of $N!$ equally likely permutations. A cycle of length $\ell$ displaces $\ell-1$ already-seated passengers. The mean number of displacements is therefore $(N-1)/2$. Conditional on the cycle, summing the mean duration $\mu^{-1}$ of each displacement gives

$$
\boxed{\mathbb E(\text{displacement delay})=\frac{N-1}{2\mu}.}
$$

This counts the delay caused by moving already-seated passengers, as the final wording suggests. If “each move” is intended also to charge the last passenger's own initial seating, even when their seat was vacant, the number of timed moves is $\ell$ instead, and the answer is $(N+1)/(2\mu)$. These conventions differ by the baseline boarding time $\mu^{-1}$; the distinction is present in the source wording.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
