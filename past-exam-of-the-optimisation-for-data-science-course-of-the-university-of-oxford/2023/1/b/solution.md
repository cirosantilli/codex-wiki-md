<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Again write $z=x-\alpha\nabla f(x)$ and $\tau=\alpha\lambda$, and let $z_\ell$ denote its $\ell$th block of $k$ coordinates. The [block mixed norm](../../../../block-mixed-norm.md) in this part makes the [proximal operator](../../../../proximal-operator.md) separate over blocks. For a single block, its [minimiser](../../../../global-minimizer.md) solves

$$
\min_{u\in\mathbb R^k}\left\{\tau\|u\|+\frac12\|u-z_\ell\|^2\right\}.
$$

At a nonzero $u$, the [gradient](../../../../gradient.md) of the [Euclidean norm](../../../../euclidean-norm.md) is $u/\|u\|$. The [subgradient optimality condition](../../../../subgradient-optimality-condition.md) therefore becomes

$$
z_\ell=u+\tau\frac{u}{\|u\|}.
$$

Thus $u$ points in the direction of $z_\ell$ and $\|z_\ell\|=\|u\|+\tau$. This yields $u=(1-\tau/\|z_\ell\|)z_\ell$ when $\|z_\ell\|>\tau$.

At zero, the [subdifferential](../../../../subdifferential.md) of the [Euclidean norm](../../../../euclidean-norm.md) is the closed [Euclidean unit ball](../../../../euclidean-unit-ball.md): the [subgradient inequality](../../../../subgradient-inequality.md) is $q^Tw\leq\|w\|$ for every $w$, which is equivalent to $\|q\|\leq1$ by the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) and the choice $w=q$. Hence zero solves the [subgradient optimality condition](../../../../subgradient-optimality-condition.md) exactly when $\|z_\ell\|\leq\tau$. This also covers $z_\ell=0$ and avoids division by zero.

The resulting [radial soft thresholding](../../../../radial-soft-thresholding.md) is

$$
T_\tau(z_\ell)=
\begin{cases}
0,&\|z_\ell\|\leq\tau,\\
\left(1-\dfrac{\tau}{\|z_\ell\|}\right)z_\ell,&\|z_\ell\|>\tau.
\end{cases}
$$

If $y_\ell$ is the corresponding block of $x$, the required [proximal gradient mapping](../../../../proximal-gradient-mapping.md) is

$$
\boxed{[G_\alpha(x)]_\ell=\frac{y_\ell-T_{\alpha\lambda}(z_\ell)}{\alpha},\qquad z_\ell=y_\ell-\alpha[\nabla f(x)]_\ell.}
$$

**Whole blocks can become zero**, while nonzero blocks retain their direction after the [gradient](../../../../gradient.md) step. For a block of size one, [radial soft thresholding](../../../../radial-soft-thresholding.md) agrees with the [soft-thresholding operator](../../../../soft-thresholding.md) in part (a).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
