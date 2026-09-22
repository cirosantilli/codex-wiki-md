<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\alpha=\log_b a$. With a nonnegative toll bounded by $O(n^d)$, the [Master theorem](../../../../../master-theorem.md) gives the upper bounds

$$
\boxed{
T(n)=\begin{cases}
O(n^\alpha),&d<\alpha,\\
O(n^d\log n),&d=\alpha,\\
O(n^d),&d>\alpha.
\end{cases}}
$$

If the base cost is $\Theta(1)$ and the toll is $\Theta(n^d)$, these become the usual tight $\Theta$ bounds. The printed $O$ toll by itself does not imply those lower bounds; for example, the toll could vanish.

For the two requested proofs, let $n=b^k$ as permitted. Expanding the [recurrence relation](../../../../../recurrence-relation.md) through $k$ levels gives

$$
T(n)=a^kT(1)+\sum_{j=0}^{k-1}a^j O\!\left((n/b^j)^d\right)
=O(n^\alpha)+O\!\left(n^d\sum_{j=0}^{k-1}(a/b^d)^j\right).
$$

When $d=\alpha$, the ratio is one. The sum has $k=\log_b n$ terms, so $T(n)=O(n^d\log n)$. With matching positive lower bounds on each level's work, the same expansion gives $\Theta(n^d\log n)$.

When $d>\alpha$, the ratio $r=a/b^d$ is strictly below one. The [geometric series](../../../../../geometric-series.md) is at most $1/(1-r)$, so the internal work is $O(n^d)$; the leaf term $O(n^\alpha)$ is also $O(n^d)$. A $\Theta(n^d)$ root toll supplies the matching lower bound in the tight version. This proves both requested cases.

There is a small termination qualification in the printed generality: if $1<b<2$, the literal base case only at $n=1$ may leave `ceil(n/b) = n` at a small integer, for example $n=2,b=3/2$. The standard rounded [Master theorem](../../../../../master-theorem.md) assumes a sufficiently large fixed base-case cutoff so that recursive sizes decrease. The allowed unrounded powers-of-$b$ proof above does not use that problematic rounded step. Also, a literal number of recursive calls is integral, though the algebraic recurrence expansion remains meaningful for positive real $a$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
