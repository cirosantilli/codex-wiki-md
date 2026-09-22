<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $e_n=y(x_n)-y_n$. Subtracting the numerical update from the exact update with its [local truncation error](../../../../../local-truncation-error.md) gives

$$
e_{n+1}=e_n+h\theta[f(x_{n+1},y(x_{n+1}))-f(x_{n+1},y_{n+1})]+h(1-\theta)[f(x_n,y(x_n))-f(x_n,y_n)]+hT_n.
$$

The [Lipschitz condition](../../../../../lipschitz-continuity.md) in the solution variable and the [triangle inequality](../../../../../triangle-inequality.md) imply

$$
\boxed{(1-L\theta h)|e_{n+1}|\leq[1+L(1-\theta)h]|e_n|+h|T_n|.}
$$

The assumed positive denominator permits division. With $K=[1+L(1-\theta)h]/(1-L\theta h)$ and $e_0=0$, repeated substitution of this [Lipschitz one-step error bound](../../../../../lipschitz-one-step-error-bound.md) yields

$$
|e_n|\leq\frac h{1-L\theta h}\sum_{j=0}^{n-1}K^{n-1-j}|T_j|
\leq\boxed{\frac h{1-L\theta h}\frac{K^n-1}{K-1}\max_{0\leq j<n}|T_j|.}
$$

Here $K>1$ because $L,h>0$, so the displayed [geometric series](../../../../../geometric-series.md) quotient is well defined. For implicit steps, the same condition makes the scalar update map a [contraction mapping](../../../../../contraction-mapping.md), ensuring a unique numerical next value.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
