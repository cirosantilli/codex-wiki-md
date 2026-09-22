<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [coefficients](../../../../../../coefficient.md) of the formal series must be [smooth functions](../../../../../../smooth-function.md) $H_n\in C^\infty(M)$, rather than points of $M$. Interpret complex parameter values in the complexified [function](../../../../../../function-split.md) algebra. The [Casimir function](../../../../../../casimir-function-of-a-poisson-manifold.md) condition for the [Poisson pencil](../../../../../../poisson-pencil.md) is a coefficientwise formal identity:

$$
0=\{H,f\}_\lambda
=\{H_0,f\}_1+\sum_{n\geq1}\lambda^n
\left(\{H_n,f\}_1+\{H_{n-1},f\}_2\right).
$$

Equality of the formal [coefficients](../../../../../../coefficient.md) proves

$$
\boxed{\{H_0,f\}_1=0,\qquad
\{H_n,f\}_1=-\{H_{n-1},f\}_2\quad(n\geq1).}
$$

These are the [Lenard-Magri recursion](../../../../../../lenard-magri-recursion.md) relations, valid for every [smooth function](../../../../../../smooth-function.md) $f$.

For $i\geq1$ and $j\geq0$, use the recursion in the first argument, then antisymmetry and the recursion in the second:

$$
\{H_i,H_j\}_1=-\{H_{i-1},H_j\}_2
=\{H_{i-1},H_{j+1}\}_1.
$$

Each step lowers the first index while raising the second. Iterating $i$ times gives

$$
\{H_i,H_j\}_1=\{H_0,H_{i+j}\}_1=0,
$$

because $H_0$ is a [Casimir function](../../../../../../casimir-function-of-a-poisson-manifold.md) of the first [Poisson structure](../../../../../../poisson-structure.md). This includes $i=0$ directly. The recursion one step higher then gives

$$
\{H_i,H_j\}_2=-\{H_{i+1},H_j\}_1=0.
$$

Thus the [commuting coefficients of a Poisson pencil Casimir](../../../../../../commuting-coefficients-of-a-poisson-pencil-casimir.md) satisfy

$$
\boxed{\{H_i,H_j\}_1=\{H_i,H_j\}_2=0\qquad(i,j\geq0).}
$$

They are therefore [Poisson-commuting functions](../../../../../../poisson-commuting-functions.md) for every member of the [Poisson pencil](../../../../../../poisson-pencil.md). The argument proves involution, not [functional independence](../../../../../../functionally-independent-functions.md); an infinite sequence can contain repetitions or zero [coefficients](../../../../../../coefficient.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
