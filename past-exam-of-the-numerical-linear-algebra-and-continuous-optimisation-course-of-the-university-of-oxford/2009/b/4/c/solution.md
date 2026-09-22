<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $x_0$, fixed $\bar\alpha>0$, $\sigma,\beta\in(0,1)$, and repeat for every $n\geq0$: compute $g_n=\nabla f(x_n)$, choose $\alpha_n$ by the [backtracking line search](../../../../../backtracking-line-search.md) in part (b) with $s_n=-g_n$, and set $x_{n+1}=x_n-\alpha_ng_n$. At a stationary point keep the sequence constant.

Assume $f\in C^1$ has a globally [Lipschitz gradient](../../../../../lipschitz-gradient.md) and is bounded below on its initial [sublevel set](../../../../../sublevel-set.md) $\{x:f(x)\leq f(x_0)\}$. Then the [steepest descent method](../../../../../gradient-descent-split.md) satisfies $\boxed{\nabla f(x_n)\to0}$. Indeed, the [Armijo condition](../../../../../armijo-condition.md) and the uniform lower step bound give

$$
f(x_n)-f(x_{n+1})\geq\sigma\alpha_n\|g_n\|_2^2\geq\sigma c\|g_n\|_2^2.
$$

The objective values decrease and stay in the stated sublevel set. Summing the inequality and using its lower bound $f_{\inf}$ yields

$$
\sum_{n=0}^\infty\|g_n\|_2^2\leq\frac{f(x_0)-f_{\inf}}{\sigma c}<\infty,
$$

which proves the limit. Every cluster point is a [stationary point](../../../../../stationary-point.md) by continuity of the [gradient](../../../../../gradient.md). If the initial sublevel set is compact, cluster points exist. This global convergence result guarantees stationarity from arbitrary initial points under these assumptions; it does not, for a general nonconvex objective, guarantee convergence of the whole iterate sequence or a global minimum.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
