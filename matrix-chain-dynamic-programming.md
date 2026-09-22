# Matrix-chain dynamic programming

↑ **Parent:** [Matrix-chain multiplication](matrix-chain-multiplication.md)

Let $A_i$ have [matrix dimensions](matrix-dimensions.md) $p_{i-1}\times p_i$, where $p_0,\ldots,p_n$ are positive [integers](integer-split.md). For $1\leq i\leq j\leq n$, define $m[i,j]$ as the minimum [scalar multiplication](scalar-multiplication.md) cost of the contiguous [matrix product](matrix-product.md) $A_i\cdots A_j$. The endpoints $(i,j)$ of an [integer interval](integer-interval.md) identify a [dynamic programming state](dynamic-programming-state.md). A single [matrix](matrix.md) needs no [matrix multiplication](matrix-multiplication.md), giving the [base case](base-case.md) $m[i,i]=0$. At the final [matrix multiplication](matrix-multiplication.md), split after $A_k$:

$$
m[i,j]=\min_{i\leq k<j}\bigl(m[i,k]+m[k+1,j]+p_{i-1}p_kp_j\bigr),\qquad i<j.
$$

The two subproducts have [matrix dimensions](matrix-dimensions.md) $p_{i-1}\times p_k$ and $p_k\times p_j$, regardless of their internal grouping. The [recurrence relation](recurrence-relation.md) adds their optimal costs and the final [scalar multiplication](scalar-multiplication.md) cost.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; Lecture 21: Dynamic Programming III, printed p. 2, Parenthesization: final split, recurrence and zero one-matrix base case; notes use half-open indices](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-21-dynamic-programming-iii.md)

Why is this [optimal substructure](optimal-substructure.md)? For a chosen final split $k$, replacing either subproduct's grouping by a cheaper one leaves its [matrix dimensions](matrix-dimensions.md) and exact [matrix product](matrix-product.md) unchanged, so it decreases the whole cost by the same amount. Therefore an optimal grouping can use optimal groupings on both sides. Conversely, each candidate in the [recurrence relation](recurrence-relation.md) joins two achievable groupings. [Mathematical induction](mathematical-induction.md) on $j-i+1$, starting with the single-[matrix](matrix.md) [base case](base-case.md), proves that the minimum is achievable and no grouping is cheaper.

There are also [overlapping subproblems](overlapping-subproblems.md): while evaluating the different final splits of $ABCD$, the cases $A(BCD)$ and $(ABC)D$ both request the cost of $BC$. [Recursion](recursion-computer-science.md) without reuse recomputes this answer; [memoization](memoization.md) or a [dynamic programming](dynamic-programming.md) table stores it once. Fill the table by increasing length $j-i+1$, so both dependencies are ready. Record an attaining split $s[i,j]$ alongside each cost.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; Lecture 21: Dynamic Programming III, printed p. 2, Parenthesization: increasing substring size, cubic time and parent pointers](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-21-dynamic-programming-iii.md)

The [dynamic programming](dynamic-programming.md) table has $n(n+1)/2$ cost entries. For length $\ell$, there are $n-\ell+1$ entries and $\ell-1$ possible splits, so the exact number of candidate evaluations is

$$
\sum_{\ell=2}^{n}(n-\ell+1)(\ell-1)=\frac{n(n-1)(n+1)}{6}.
$$

Under the unit-cost assumption that [arithmetic operations](arithmetic-operation.md), comparisons and access to stored costs each take constant time, this gives [time complexity](time-complexity.md) $O(n^3)$ and [space complexity](space-complexity.md) $O(n^2)$, using [Big O notation](big-o-notation.md). These bounds concern choosing a grouping from the [matrix dimensions](matrix-dimensions.md); they exclude the subsequent [matrix multiplication](matrix-multiplication.md) work. If the dimensions or costs require arbitrarily long [integers](integer-split.md), their arithmetic and storage costs must also be counted.

## ↑ Ancestors (4)

1. [Matrix-chain multiplication](matrix-chain-multiplication.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
