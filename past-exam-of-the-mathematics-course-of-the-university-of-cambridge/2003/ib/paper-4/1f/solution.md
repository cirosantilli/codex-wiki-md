<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

[Uniform convergence](../../../../../uniform-convergence.md) on an interval $I$ means that for every $\epsilon>0$ there is $N$ such that $|f_n(x)-f(x)|<\epsilon$ for every $x\in I$ and every $n\ge N$. Equivalently, the supremum of this difference tends to zero. A [uniform limit](../../../../../uniform-limit.md) of [continuous functions](../../../../../continuous-function.md) is continuous: at a point $x_0$, choose one $f_N$ uniformly within $\epsilon/3$ of $f$, then use [continuity](../../../../../continuous-function.md) of $f_N$ to make $|f_N(x)-f_N(x_0)|<\epsilon/3$. The [triangle inequality](../../../../../triangle-inequality.md) gives $|f(x)-f(x_0)|<\epsilon$. Thus $f$ is integrable on the compact interval, and

$$
\left|\int_a^b f_n-\int_a^b f\right|\le (b-a)\sup_{[a,b]}|f_n-f|\longrightarrow0.
$$

For the half-line example, differentiating gives $f_n'(x)=n^{-2}e^{-x/n}(1-x/n)$. The maximum is attained at $x=n$, where $f_n(n)=1/(en)$. Therefore **$f_n\to0$ uniformly on $[0,\infty)$**. Nevertheless, the substitution $x=ny$ gives

$$
\boxed{\int_0^\infty f_n(x)\,dx=\int_0^\infty y e^{-y}\,dy=1}.
$$

The integral does not tend to zero. This is the phenomenon that [uniformly vanishing functions can retain a nonzero integral](../../../../../uniformly-vanishing-functions-can-retain-a-nonzero-integral.md): the finite-length estimate above has no finite analogue for the entire half-line.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
