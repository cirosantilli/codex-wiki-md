# Picard iteration for a simple-pole linear differential equation

↑ **Parent:** [Picard iteration](picard-iteration.md)

For real constants $a,c$, apply [Picard iteration](picard-iteration.md) to the [initial value problem](initial-value-problem.md) $y'=ay/(1-x)$, $y(0)=c$, starting with $y_0(x)=c$. The recurrence is

$$
y_{n+1}(x)=c+\int_0^x\frac{a\,y_n(t)}{1-t}\,dt.
$$

Since $\int_0^x\log^k(1-t)/(1-t)\,dt=-\log^{k+1}(1-x)/(k+1)$, [mathematical induction](mathematical-induction.md) gives the displayed partial sums. The [exponential series](exponential-series.md) converges at every finite argument, so $y_n(x)\to c(1-x)^{-a}$ for every real $x<1$, uniformly on each [compact interval](compact-interval.md) in that range. This is not a [Taylor series](taylor-series.md) in $x$, so its convergence is not restricted to $|x|<1$. The differential equation's coefficient is singular at $x=1$ even when a special solution has a removable singularity there.

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

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2008/7/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2012/7/solution.md)
