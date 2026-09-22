# Factorial estimate for Picard iteration

↑ **Parent:** [Picard iteration](picard-iteration.md)

For [Picard iteration](picard-iteration.md) $y_{n+1}(x)=b+\int_a^x f(s,y_n(s))\,ds$, $y_0=b$, assume $|f|\leq M$ and a [Lipschitz constant](lipschitz-constant.md) $L$ on a rectangle containing every iterate. The first difference is at most $M|x-a|$. Integrating the preceding bound multiplied by $L$ proves the displayed estimate by [mathematical induction](mathematical-induction.md). Its uniform bounds sum to a convergent [exponential series](exponential-series.md) for every finite $Lh$, so the [Weierstrass M-test](weierstrass-m-test.md) gives [uniform convergence](uniform-convergence.md) without requiring $Lh<1$.

For two arbitrary initial functions $y,z$ in a function set preserved by the [Picard iteration](picard-iteration.md) operator $T$, the same induction gives

$$
\|T^ny-T^nz\|_\infty\leq\frac{(Lh)^n}{n!}\|y-z\|_\infty.
$$

Thus some iterate is a [contraction mapping](contraction-mapping.md) on any fixed finite interval for which every iterate stays in that set. The [iterated contraction](iterated-contraction.md) argument gives a unique fixed point of $T$ on a nonempty [complete metric space](complete-metric-space.md), without requiring $Lh<1$. For a rectangle with field bound $M$ and vertical radius $k$, $Mh\leq k$ supplies the required self-mapping property.

## ↑ Ancestors (8)

1. [Picard iteration](picard-iteration.md)
2. [Picard-Lindelöf theorem](picard-lindelof-theorem.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-differential-equations-1-course-of-the-university-of-oxford/2017/2/a/iii/solution.md)
- [Solution](past-exam-of-the-differential-equations-1-course-of-the-university-of-oxford/2021/2/a/1/solution.md)
