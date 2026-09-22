# Butcher tableau

↑ **Parent:** [Runge-Kutta method](runge-kutta-method-split.md)

A Butcher tableau records a [Runge-Kutta method](runge-kutta-method-split.md)'s stage [matrix](matrix.md) $A$, time nodes $c$, and output weights $b$ in the block array

$$
\begin{array}{c|c}c&A\\\hline&b^T\end{array}.
$$

Read row $i$ above the line as the recipe for [Runge-Kutta stage](runge-kutta-stage.md) $i$: the left entry gives $t_n+c_i h$, and the right entries give the coefficients in $Y_i=y_n+h\sum_ja_{ij}k_j$. Below the line, $b_i$ weights slope $k_i$ in the final update. Zeros on and above the diagonal identify an [Explicit Runge-Kutta method](explicit-runge-kutta-method.md). For the internally consistent convention, row sums of $A$ equal $c$; first-order [consistency of a numerical method](consistency-of-a-numerical-method.md) also requires $\sum_i b_i=1$. An [embedded Runge-Kutta pair](embedded-runge-kutta-pair.md) adds another weight row while retaining $A,c$.

## ↑ Ancestors (6)

1. [Runge-Kutta method](runge-kutta-method-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Euler-Heun embedded pair](euler-heun-embedded-pair.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-341/5/b/3/solution.md)
- [Runge-Kutta method](runge-kutta-method-split.md)
