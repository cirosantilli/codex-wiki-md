<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [binomial branching process](../../../../../../binomial-branching-process.md), the offspring [probability generating function](../../../../../../probability-generating-function.md) is $f(s)=(1-p+ps)^n$. The [Galton-Watson extinction fixed point](../../../../../../galton-watson-extinction-fixed-point.md) gives $1-\rho=f(1-\rho)=(1-p\rho)^n$.

**The printed finite-binomial upper bound is false without an additional asymptotic qualification.** For $n=2$ and $p=(1+\varepsilon)/2$, solving the fixed-point equation exactly gives

$$
\rho=\frac{4\varepsilon}{(1+\varepsilon)^2}.
$$

For instance $\varepsilon=1/20$ gives $\rho=80/441>1/10=2\varepsilon$. More generally, at every fixed $n>1$ the [Taylor expansion](../../../../../../taylor-expansion.md) gives $\rho=2n\varepsilon/(n-1)+O_n(\varepsilon^2)$, again contradicting that upper bound for sufficiently small positive $\varepsilon$.

Here is the corrected [binomial branching survival correction](../../../../../../binomial-branching-survival-correction.md). The [Poisson branching process](../../../../../../poisson-branching-process.md) of mean $1+\varepsilon$ has [branching survival probability](../../../../../../survival-probability-of-a-branching-process.md) $r$ satisfying $-\log(1-r)=(1+\varepsilon)r$. Expanding the [logarithm](../../../../../../logarithm.md) gives

$$
\varepsilon=\sum_{j\geq1}\frac{r^j}{j+1},\qquad
\frac r2\leq\varepsilon\leq\frac r{2(1-r)}.
$$

Thus $2\varepsilon/(1+2\varepsilon)\leq r\leq2\varepsilon$, which implies the requested lower estimate $r\geq2\varepsilon-4\varepsilon^2$. Since $(1-p+ps)^n\leq e^{np(s-1)}$ on $[0,1]$, iteration of the two offspring [probability generating functions](../../../../../../probability-generating-function.md) gives $\rho\geq r$.

For the actual [binomial branching process](../../../../../../binomial-branching-process.md), expansion of its exact fixed-point equation gives

$$
\varepsilon=\sum_{j\geq1}\frac{1-np^{j+1}}{j+1}\rho^j.
$$

If $(1+\varepsilon)^2<n$, all coefficients are nonnegative. Keeping the first term proves

$$
\boxed{\frac{2\varepsilon}{1+2\varepsilon}\leq\rho\leq
\frac{2\varepsilon}{1-(1+\varepsilon)^2/n}.}
$$

In particular, for $n\to\infty$ and $\varepsilon=o(1)$ this gives $\rho=2\varepsilon+O(\varepsilon^2+\varepsilon/n)$. The printed bounds also hold for the [binomial branching process](../../../../../../binomial-branching-process.md) in an explicit large-$n$ regime: $0<\varepsilon\leq1/4$ and $n\varepsilon\geq2$. Indeed these conditions give $np^2\leq\varepsilon$ and $np^3\leq1/4$. In the preceding nonnegative series, evaluation at $x=2\varepsilon$ gives

$$
\sum_{j\geq1}\frac{1-np^{j+1}}{j+1}x^j
\geq\varepsilon(1-np^2)+\frac43\varepsilon^2(1-np^3)
\geq\varepsilon-\varepsilon^2+\varepsilon^2=\varepsilon.
$$

The series is increasing, and its value at the actual [branching survival probability](../../../../../../survival-probability-of-a-branching-process.md) $\rho$ is $\varepsilon$, so $\rho\leq2\varepsilon$. Together with the lower bound already proved, this recovers $2\varepsilon-4\varepsilon^2\leq\rho\leq2\varepsilon$ in that regime. In particular it applies eventually to part (ii). The counterexample shows why a regime condition is needed for a literal finite-$n$ statement.

<a id="4/i/image-finite-binomial-survival-exceeds-the-printed-upper-bound-while-poisson-survival-lies-between-the-corrected-comparison-bounds"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9-branching-survival.png)

**[Figure 1](#4/i/image-finite-binomial-survival-exceeds-the-printed-upper-bound-while-poisson-survival-lies-between-the-corrected-comparison-bounds). Finite-binomial survival exceeds the printed upper bound, while Poisson survival lies between the corrected comparison bounds**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
