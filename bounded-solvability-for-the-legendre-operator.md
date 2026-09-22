# Bounded solvability for the Legendre operator

↑ **Parent:** [Sturm-Liouville problem](sturm-liouville-problem.md)

For $f\in C([-1,1])$, the equation $((1-x^2)y')'=f$ has a bounded solution on $(-1,1)$ if and only if $\int_{-1}^1f=0$. All bounded solutions differ by a constant. To prove necessity, integrate the equation once. The quantity $(1-x^2)y'$ has finite endpoint limits, and any nonzero endpoint limit would force logarithmic growth in $y$. Both limits must therefore vanish, yielding the zero-mean condition. For sufficiency set $F(x)=\int_{-1}^xf(t)dt$ and $y(x)=C+\int_0^x F(s)/(1-s^2)ds$. Zero mean implies $|F(s)|\leq\|f\|_\infty\min(1+s,1-s)$, so $y'$ is bounded and $y$ extends continuously to the endpoints. The homogeneous solutions are a constant and $\tfrac12\log((1+x)/(1-x))$, proving uniqueness up to a constant. This is the [Fredholm alternative](fredholm-alternative.md) for the zero [eigenvalue](eigenvalue.md) of this singular [Sturm-Liouville problem](sturm-liouville-problem.md).

The [eigenfunction expansion](eigenfunction-expansion.md) in [Legendre polynomials](legendre-polynomial.md) is $y=C-\sum_{k\geq1}P_k\int_{-1}^1fP_k/[k(k+1)\int_{-1}^1P_k^2]$. It follows by projecting onto the [eigenfunctions](eigenfunction.md) with [eigenvalues](eigenvalue.md) $-k(k+1)$. Completeness follows because the [Legendre polynomials](legendre-polynomial.md) span the [polynomials](polynomial-split.md), which are dense by the [Weierstrass approximation theorem](weierstrass-approximation-theorem.md).

Continuity only in the open interval requires more care. Even if $f$ is integrable and has zero mean, the primitive of $F/(1-x^2)$ must still be bounded at both ends. For example, $F(x)=1/\log(e/(1-x^2))$ has zero endpoint limits and absolutely integrable derivative $f=F'$, but $F/(1-x^2)$ has a divergent primitive. Thus zero mean alone is insufficient without endpoint control.

## ↑ Ancestors (6)

1. [Sturm-Liouville problem](sturm-liouville-problem.md)
2. [Sturm-Liouville theory](sturm-liouville-theory-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2023/2/b/ii/solution.md)
