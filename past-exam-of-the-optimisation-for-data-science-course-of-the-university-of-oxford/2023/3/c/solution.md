<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For arbitrary $x,y$, write the [Bregman divergence](../../../../bregman-divergence.md)

$$
D_f(x,y)=f(x)-f(y)-\nabla f(y)^T(x-y)\geq0,
\qquad \delta_i=\partial_i f(x)-\partial_i f(y).
$$

Part (b), with its supporting [affine function](../../../../affine-function.md) constructed at this $y$, implies the [coordinate derivative bound by Bregman divergence](../../../../coordinate-derivative-bound-by-bregman-divergence.md)

$$
\delta_i^2\leq2L_iD_f(x,y).
$$

For a nonempty block $\mathcal B$, set $S_{\mathcal B}=\sum_{i\in\mathcal B}L_i$ and $\delta_{\mathcal B}=\nabla_{\mathcal B}f(x)-\nabla_{\mathcal B}f(y)$. Sum the coordinate inequalities:

$$
\|\delta_{\mathcal B}\|^2\leq2S_{\mathcal B}D_f(x,y).
$$

Since $y$ in part (b) was arbitrary, interchange $x$ and $y$ to obtain the same left side bounded by $2S_{\mathcal B}D_f(y,x)$. Adding the two inequalities and dividing by two gives

$$
\|\delta_{\mathcal B}\|^2\leq S_{\mathcal B}\big(D_f(x,y)+D_f(y,x)\big)
=S_{\mathcal B}(\nabla f(x)-\nabla f(y))^T(x-y).
$$

Now require that $x-y$ have zero coordinates outside $\mathcal B$. The last [dot product](../../../../dot-product.md) is then $\delta_{\mathcal B}^T(x-y)$. By the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md),

$$
\|\delta_{\mathcal B}\|^2\leq S_{\mathcal B}\|\delta_{\mathcal B}\|\,\|x-y\|.
$$

If $\delta_{\mathcal B}=0$, the desired estimate is immediate; otherwise divide by its [Euclidean norm](../../../../euclidean-norm.md). We have proved the stronger [block Lipschitz constant from coordinate smoothness](../../../../block-lipschitz-constant-from-coordinate-smoothness.md) estimate

$$
\boxed{\|\nabla_{\mathcal B}f(x)-\nabla_{\mathcal B}f(y)\|\leq\left(\sum_{i\in\mathcal B}L_i\right)\|x-y\|\quad\text{when }x-y\text{ is supported in }\mathcal B.}
$$

In particular, take $y=x-\alpha\nabla_{\mathcal B}f(x)$ for any real $\alpha$. This proves (6), with a valid choice

$$
\boxed{L_{\mathcal B}=\sum_{i\in\mathcal B}L_i\leq|\mathcal B|\max_{i\in\mathcal B}L_i.}
$$

The least admissible [Lipschitz constant](../../../../lipschitz-constant.md) is therefore no larger than this choice. For the empty block, the [block coordinate gradient](../../../../block-coordinate-gradient.md) vanishes identically and its least nonnegative [Lipschitz constant](../../../../lipschitz-constant.md) is zero. The proof uses only $C^1$ [differentiability](../../../../differentiability.md), [convexity](../../../../convex-function.md) and [coordinate Lipschitz continuity](../../../../coordinate-lipschitz-continuity.md), with no assumed [Hessian matrix](../../../../hessian-matrix.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the optimisation for data science course of the University of Oxford](../../../split.md)
5. [Optimisation for data science course of the University of Oxford](../../../../optimisation-for-data-science-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
