# Uniform limit theorem

↑ **Parent:** [Uniform convergence](uniform-convergence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_limit_theorem)

A [uniform limit](uniform-limit.md) of [continuous functions](continuous-function.md) is a [continuous function](continuous-function.md). No [compactness](compact-space.md) assumption on the [domain of a function](domain-of-a-function.md) is required.[Basic Analysis: Introduction to Real Analysis, Volume I by Jiří Lebl, §6.2.1, Theorem 6.2.2](basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl/6-2-interchange-of-limits.md)

For a proof, fix an input $x$ and tolerance $\varepsilon>0$. [Uniform convergence](uniform-convergence.md) supplies one $f_N$ with $\|f_N-f\|_\infty<\varepsilon/3$. Its [continuity](continuous-function.md) at $x$ supplies $\delta>0$ with $|f_N(y)-f_N(x)|<\varepsilon/3$ for allowed inputs satisfying $|y-x|<\delta$. The [triangle inequality](triangle-inequality.md) gives

$$
|f(y)-f(x)|\leq|f(y)-f_N(y)|+|f_N(y)-f_N(x)|+|f_N(x)-f(x)|<\varepsilon.
$$

One approximating [function](function-split.md) controls both endpoints of this estimate. Under [pointwise convergence](pointwise-convergence.md), selecting an index for $x$ supplies no common control at nearby $y$. This explains why the [polynomial functions](polynomial-function.md) $x^n$ can have a discontinuous [pointwise limit](pointwise-limit.md) on $[0,1]$.

## ↑ Ancestors (7)

1. [Uniform convergence](uniform-convergence.md)
2. [Sequence and series](sequence-and-series-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4/4e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/11b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-8/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/11e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-61/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/3g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-136/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/3e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/3e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/2h/solution.md)
- [Space of continuous functions on a compact space](space-of-continuous-functions-on-a-compact-space.md)
- [Summable absolute-value cusp series](summable-absolute-value-cusp-series.md)
- [Uniform convergence](uniform-convergence.md)
- [Uniform convergence at moving evaluation points](uniform-convergence-at-moving-evaluation-points.md)
- [Uniform derivative convergence with an anchored value](uniform-derivative-convergence-with-an-anchored-value.md)
