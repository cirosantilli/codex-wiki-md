<h1 id="11b/solution">Solution</h1>

↑ **Parent:** [11B](../11b.md)

Fix $x_0\in E$ and $\varepsilon>0$. By [uniform convergence](../../../../../uniform-convergence.md), choose $N$ so that $|f_N(x)-f(x)|<\varepsilon/3$ for every $x\in E$. By [continuity](../../../../../continuous-function.md) of $f_N$ relative to $E$, there is $\delta>0$ such that $x\in E$ and $|x-x_0|<\delta$ imply $|f_N(x)-f_N(x_0)|<\varepsilon/3$. The [triangle inequality](../../../../../triangle-inequality.md) gives

$$
|f(x)-f(x_0)|
\le |f(x)-f_N(x)|+|f_N(x)-f_N(x_0)|+|f_N(x_0)-f(x_0)|
<\varepsilon.
$$

This proves the [uniform limit theorem](../../../../../uniform-limit-theorem.md) without requiring $E$ to be open or closed.

For the series, fix an arbitrary $x_0\in(0,1]$ and put $a=x_0/2>0$. On $[a,1]$ each summand $n^{-1-x}$ is [continuous](../../../../../continuous-function.md) and

$$
0<n^{-1-x}\le n^{-1-a},\qquad
\sum_{n=1}^\infty n^{-1-a}<\infty.
$$

The [Weierstrass M-test](../../../../../weierstrass-m-test.md) gives [uniform convergence](../../../../../uniform-convergence.md) of the series on $[a,1]$. Its partial sums are [continuous](../../../../../continuous-function.md), so the [uniform limit theorem](../../../../../uniform-limit-theorem.md) makes its sum [continuous](../../../../../continuous-function.md) on that interval, in particular at $x_0$ with the appropriate relative topology if $x_0=1$. Since $x_0$ was arbitrary, **the sum is continuous on $(0,1]$**.

This is local [uniform convergence](../../../../../uniform-convergence.md), not [uniform convergence](../../../../../uniform-convergence.md) on the entire half-open interval. Indeed, for any finite partial sum length $N$, its tail as $x\downarrow0$ is bounded below by arbitrarily long tails of the divergent harmonic series. There is no continuity claim at the excluded endpoint $0$.

## ↑ Ancestors (10)

1. [11B](../11b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
