<h1 id="p/4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The claimed endpoint bounds with radius $\epsilon$ are **false for positive corner perturbations**. For example, take $n=3$, $\epsilon=1/1000$ and $\delta=9/10<1-\epsilon$. The characteristic [polynomial](../../../../../polynomial-split.md) is

$$
P(\lambda)=(\lambda-1)(\lambda-2)(\lambda-3)
-\frac1{4000}(2\lambda-4)-\frac9{160}.
$$

Throughout $|\lambda-1|\le1/1000$, the absolute value of the sum of its first two terms is below $0.003$, whereas $9/160=0.05625$. Hence this interval contains no root, contradicting the first requested bound. The actual [eigenvalues](../../../../../eigenvalue.md) are approximately $1.029144,1.943599,3.027257$, which also violate the last requested bound.

There is a valid real-eigenvalue conclusion with wider endpoint bounds. For $0<\epsilon<1/4$ and $\delta<(n-1)/2-\epsilon$, the [Gershgorin discs](../../../../../gershgorin-disc.md) from rows have one enlarged component on the left; the [Gershgorin discs](../../../../../gershgorin-disc.md) from columns have one enlarged component on the right. Each has an enlarged radius $r=\delta+\epsilon<(n-1)/2$. A small disc that meets the enlarged left disc has index $j$ satisfying $j-1\le r+q<n/2$. A small disc meeting the enlarged right disc satisfies $n-j<n/2$. Thus, when $n=2m$, every disc with index at most $m$ is isolated in the column family and every disc with index at least $m+1$ is isolated in the row family. Their counts give all $n$ [eigenvalues](../../../../../eigenvalue.md), one in each disjoint small disc, so all are real.

When $n=2m+1$, the same argument isolates the first $m$ discs in the column family and the last $m$ in the row family. It accounts for $2m$ real [eigenvalues](../../../../../eigenvalue.md). The one remaining [eigenvalue](../../../../../eigenvalue.md) is real by conjugation, and belongs to the central small disc: the enlarged left and right discs are disjoint, and their two components can intersect only within the disc centered at $m+1$. Therefore the valid uniform bounds are

$$
\boxed{|\lambda_1-1|\le\tfrac14,\quad
|\lambda_i-i|\le\tfrac14+\epsilon\ (2\le i<n),\quad
|\lambda_n-n|\le\tfrac14.}
$$

The sharper endpoint radii $\epsilon$ hold in part (d) when $\delta=0$, and cannot simply be carried over to the perturbed [matrix](../../../../../matrix.md).

## ↑ Ancestors (13)

1. [F](../f.md)
2. [4](../../4.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
