<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Count element reads and writes, ignoring simple-variable operations. A [swap](../../../../../swap.md) of distinct entries makes two reads and two writes, hence four expensive accesses. For $0<k<n$, the three-reversal method therefore costs

$$
4R,\qquad R=\left\lfloor\frac{n-k}{2}\right\rfloor+\left\lfloor\frac{k}{2}\right\rfloor+\left\lfloor\frac n2\right\rfloor.
$$

Here $R=n$ if $n$ and $k$ are both even, and $R=n-1$ otherwise.

For either block-exchange version, let $a=n-k$, $b=k$, and let $S(a,b)$ count element swaps. The recurrence is $S(a,a)=a$ and, when the lengths differ,

$$
S(a,b)=\min(a,b)+S\bigl(\min(a,b),|a-b|\bigr).
$$

The [Euclidean algorithm](../../../../../euclidean-algorithm.md) preserves $\gcd(a,b)$ under this subtraction. [Induction](../../../../../mathematical-induction.md) on $a+b$ therefore yields

$$
S(a,b)=a+b-\gcd(a,b)=n-\gcd(n,k).
$$

Thus both block-exchange methods cost **$4(n-\gcd(n,k))$ accesses**, no more than the three-reversal method. Their element-access counts are identical; the iterative one avoids the recursive stack. For example a half-length rotation uses $n/2$ swaps instead of approximately $n$ reversal swaps.

Each single-place pass in part (iv) reads every entry once and writes every entry once, costing **$2nk$ accesses**. For $k=1$, its $2n$ accesses beat the block method's $4(n-1)$ for $n>2$ and tie for $n=2$. For $k\geq2$ the block method costs strictly less than $2nk$. All three methods as written return without accesses for $k=0$ or $k=n$. **Repeated shifting can take quadratic time; the reversal and block methods take linear time.** These comparisons concern the specified implementations, not a more general cycle-decomposition rotation using several disjoint cycles.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
