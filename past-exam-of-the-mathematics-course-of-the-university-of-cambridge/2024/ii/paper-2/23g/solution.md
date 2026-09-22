<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) says that if $Y$ is a linear subspace of a real normed space $X$ and $g:Y\to\mathbb R$ is bounded and linear, then there is a bounded linear extension $G:X\to\mathbb R$ with $\|G\|=\|g\|$.

For $x\in X$, the map $\widehat x(f)=f(x)$ is linear on $X'$ and

$$
|\widehat x(f)|\leq\|f\|\,\|x\|,
$$

so $\widehat x\in X''$ and $\|\widehat x\|\leq\|x\|$. The assignment $Jx=\widehat x$ is visibly linear. If $x\ne0$, define $g$ on $\operatorname{span}\{x\}$ by

$$
g(\lambda x)=\lambda\|x\|.
$$

It has norm one, and Hahn--Banach extends it to an $f\in X'$ of norm one with $f(x)=\|x\|$. Therefore

$$
\|\widehat x\|\geq|\widehat x(f)|=\|x\|.
$$

Thus the [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md) is an isometry and

$$
\boxed{\|x\|=\sup_{\|f\|\leq1}|f(x)|}.
$$

On $C([0,1])$, point evaluation $\ell(f)=f(0)$ has norm one for the $L^\infty$ norm, because a [continuous function](../../../../../continuous-function.md)'s essential supremum equals its supremum. Hahn--Banach extends it to $\Lambda\in(L^\infty)'$. If $\Lambda$ were represented by some $g\in L^1$, then

$$
f(0)=\int_0^1f(t)g(t)\,dt
$$

for every continuous $f$. Choose continuous $0\leq f_n\leq1$ with $f_n(0)=1$ and support in $[0,1/n]$. Absolute continuity of the [integral](../../../../../integral.md) makes the right side tend to zero, while the left side is always one, a contradiction. This [singular functional on L infinity](../../../../../singular-functional-on-l-infinity.md) proves

$$
\boxed{(L^\infty)'\ne L^1(\mu).}
$$

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
