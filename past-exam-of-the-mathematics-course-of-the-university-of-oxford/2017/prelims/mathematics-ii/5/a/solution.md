<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [sequence](../../../../../../sequence.md) $(f_n)$ converges by [uniform convergence](../../../../../../uniform-convergence.md) to $f$ on $E$ if

$$
\forall\varepsilon>0\ \exists M\in\mathbb N\ \forall n\geq M\ \forall x\in E:\quad |f_n(x)-f(x)|<\varepsilon.
$$

The index $M$ must work simultaneously for every $x\in E$.

Given $\varepsilon>0$, choose $m\geq N$ so large that $|f_m(x)-f(x)|<\varepsilon/3$ for every $x\in E$. The [continuity](../../../../../../continuous-function.md) of this one fixed $f_m$ at $x_0$ gives $\delta>0$ such that $x\in E$ and $|x-x_0|<\delta$ imply $|f_m(x)-f_m(x_0)|<\varepsilon/3$. The [triangle inequality](../../../../../../triangle-inequality.md) then gives

$$
|f(x)-f(x_0)|\leq|f(x)-f_m(x)|+|f_m(x)-f_m(x_0)|+|f_m(x_0)-f(x_0)|<\varepsilon.
$$

Thus **$f$ is continuous at $x_0$**, with [continuity](../../../../../../continuous-function.md) understood relative to $E$. This is the pointwise form of the [uniform limit theorem](../../../../../../uniform-limit-theorem.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
