<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an initially zero [binary counter](../../../../../binary-counter.md), [bit](../../../../../bit.md) $i$ changes precisely on increments whose indices are divisible by $2^i$. Weighting each such change by $2^i$ gives the exact total

$$
\boxed{C(n,k)=\sum_{i=0}^{k-1}2^i\left\lfloor\frac{n}{2^i}\right\rfloor.}
$$

For $n\geq1$ and $k\geq1$, put $r=\min\{k,1+\lfloor\log_2 n\rfloor\}$. All summands with $i\geq r$ vanish; each of the other summands is at most $n$. Therefore

$$
\boxed{C(n,k)\leq nr=O\!\left(n\min\{k,1+\log_2 n\}\right).}
$$

This is sharper than simply charging $n$ for each of all $k$ positions when $n$ is small. To show that the order is best possible, use $\lfloor x\rfloor\geq x/2$ for $x\geq1$. For every $0\leq i<r$,

$$
2^i\left\lfloor\frac{n}{2^i}\right\rfloor\geq\frac n2,
\qquad
\frac{nr}{2}\leq C(n,k)\leq nr.
$$

Thus the [asymptotic analysis](../../../../../asymptotic-analysis.md) gives a tight bound. If wraparound is excluded, $n<2^k$, and this becomes $\Theta(n(1+\log_2 n))$, often written $\Theta(n\log n)$ for $n\geq2$. If wraparound is allowed and $n\geq2^k$, it becomes $\Theta(nk)$. For $n=0$, the cost is zero.

For completeness, the same conclusion cannot be asserted uniformly over arbitrary initial [binary counter](../../../../../binary-counter.md) states. An initial value $2^k-1$ makes the first increment change every [bit](../../../../../bit.md), costing $2^k-1$. A general upper bound follows by replacing each [floor function](../../../../../floor-function.md) in the count by a [ceiling function](../../../../../ceiling-function.md):

$$
C_{\mathrm{arbitrary}}(n,k)
\leq\sum_{i=0}^{k-1}2^i\left\lceil\frac n{2^i}\right\rceil
\leq nr+2^k-1.
$$

To see the second inequality, split at $r$: for $i<r$, use $\lceil n/2^i\rceil\leq n/2^i+1$, and for $i\geq r$, use $\lceil n/2^i\rceil=1$. For $n\geq1$ the worst initial-state cost is consequently $\Theta(nr+2^k)$. This qualification separates initialization from the usual [amortized analysis](../../../../../amortized-analysis.md) starting at zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
