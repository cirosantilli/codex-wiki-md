<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $z=x-\alpha\nabla f(x)$ and $\tau=\alpha\lambda$. The [proximal operator](../../../../proximal-operator.md) for the [L1 norm](../../../../l1-norm.md) separates into independent scalar [minimization problems](../../../../minimization-problem.md):

$$
p_i=\mathop{\arg\min}_{u\in\mathbb R}\left\{\tau|u|+\frac12(u-z_i)^2\right\}.
$$

The [subgradient optimality condition](../../../../subgradient-optimality-condition.md) is $0\in p_i-z_i+\tau\partial|p_i|$. By the [subgradient of the absolute value](../../../../subgradient-of-the-absolute-value.md), a positive solution must satisfy $p_i=z_i-\tau>0$, and a negative solution must satisfy $p_i=z_i+\tau<0$. At zero, the [subgradient optimality condition](../../../../subgradient-optimality-condition.md) holds exactly when $|z_i|\leq\tau$. The squared term makes the [objective function](../../../../objective-function.md) a [strictly convex function](../../../../strictly-convex-function.md), so these cases give its unique [minimiser](../../../../global-minimizer.md).

Thus the [proximal operator](../../../../proximal-operator.md) is the [soft-thresholding operator](../../../../soft-thresholding.md)

$$
S_\tau(t)=
\begin{cases}
t-\tau,&t>\tau,\\
0,&|t|\leq\tau,\\
t+\tau,&t<-\tau,
\end{cases}
\qquad p_i=S_\tau(z_i).
$$

Consequently the requested [proximal gradient mapping](../../../../proximal-gradient-mapping.md), rather than just the [proximal operator](../../../../proximal-operator.md), is

$$
\boxed{[G_\alpha(x)]_i=\frac{x_i-S_{\alpha\lambda}(x_i-\alpha\partial_i f(x))}{\alpha},\qquad i=1,\ldots,n.}
$$

The corresponding [proximal gradient method](../../../../proximal-gradient-method.md) update is $x_i^+=S_{\alpha\lambda}(x_i-\alpha\partial_i f(x))$. **Small [coordinates](../../../../coordinate-linear-algebra.md) are set exactly to zero.** When $\lambda=0$, the [soft-thresholding operator](../../../../soft-thresholding.md) is the identity and the [proximal gradient mapping](../../../../proximal-gradient-mapping.md) reduces to $\nabla f(x)$.

## ↑ Ancestors (12)

1. [A](../a.md)
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
