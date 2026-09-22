<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $M=\|\,|e_0|+|e_1|\,\|_\infty$. Since both [linear functionals](../../../../../linear-functional.md) have [operator norm](../../../../../operator-norm.md) one, for every $f\in X$ the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
|(Tf)(x)|\leq|\ell_0(f)||e_0(x)|+|\ell_1(f)||e_1(x)|
\leq\|f\|_\infty\bigl(|e_0(x)|+|e_1(x)|\bigr).
$$

Taking the [essential supremum](../../../../../essential-supremum.md) proves $\|T\|\leq M$.

For the reverse bound, [continuity](../../../../../continuous-function.md) and the [extreme value theorem](../../../../../extreme-value-theorem.md) give $x_*\in[0,1]$ with $|e_0(x_*)|+|e_1(x_*)|=M$. Choose complex $a_0,a_1$ of modulus one so that $a_je_j(x_*)=|e_j(x_*)|$, taking $a_j=1$ if $e_j(x_*)=0$. The [continuous function](../../../../../continuous-function.md)

$$
f_*(x)=(1-x)a_0+xa_1
$$

has [supremum norm](../../../../../supremum-norm.md) one by the [triangle inequality](../../../../../triangle-inequality.md) and its endpoint values. Since $\ell_j(f_*)=a_j$,

$$
(Tf_*)(x_*)=a_0e_0(x_*)+a_1e_1(x_*)=M.
$$

The output is continuous, so its [L-infinity norm](../../../../../l-infinity-norm.md) equals its [supremum norm](../../../../../supremum-norm.md), including when $x_*$ is an endpoint. Therefore $\|T\|\geq M$, and the exact [operator norm](../../../../../operator-norm.md) is

$$
\boxed{\|T\|=\|\,|e_0|+|e_1|\,\|_\infty.}
$$

This is the [norm of a two-endpoint interpolation projection](../../../../../norm-of-a-two-endpoint-interpolation-projection.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis I course of the University of Oxford](../../../../split.md)
6. [Functional analysis I course of the University of Oxford](../../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
