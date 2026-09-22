<h1 id="b/4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The quadratic model has gradient $g(x_k)+B_kp$ and positive-definite [Hessian matrix](../../../../../hessian-matrix.md) $B_k$. Its unique minimizer is therefore

$$
\boxed{p_k=-B_k^{-1}g(x_k).}
$$

If $g(x_k)\ne0$, then $p_k\ne0$ and $g(x_k)^Tp_k=-p_k^TB_kp_k<0$, proving that it is a [descent direction](../../../../../descent-direction.md).

[Backtracking line search](../../../../../backtracking-line-search.md) starts with a trial step and repeatedly reduces it until the [Armijo condition](../../../../../armijo-condition.md) holds. Part (ii) guarantees finite termination because sufficiently small steps are acceptable. The test guarantees a specified positive fraction of the decrease predicted by the linear model, namely $f(x_k+\alpha p_k)\leq f(x_k)+\alpha\beta g(x_k)^Tp_k<f(x_k)$ for an accepted positive step. It does not require solving the line-minimization problem exactly.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
