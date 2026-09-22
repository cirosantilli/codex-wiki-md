<h1 id="27j/solution">Solution</h1>

↑ **Parent:** [27J](../27j.md)

A [complete statistic](../../../../../complete-statistic.md) $T$ for a family $(P_\theta)$ if every measurable $g$ with $\mathbb E_\theta|g(T)|<\infty$ and $\mathbb E_\theta g(T)=0$ for all $\theta$ satisfies $g(T)=0$ almost surely under every $P_\theta$. It is [boundedly complete](../../../../../boundedly-complete-statistic.md) if the same implication is required only for bounded measurable $g$. Completeness therefore implies bounded completeness.

The vector $X$ is multivariate normal with mean zero and covariance

$$
\Sigma_\theta=(1-\theta)I+\theta J.
$$

Its [determinant](../../../../../determinant.md) is $(1-\theta)^2(1+2\theta)$ and its inverse is $(1-\theta)^{-1}I-\theta[(1-\theta)(1+2\theta)]^{-1}J$. Hence the joint density is

$$
\boxed{p_\theta(x)=
\frac{\exp\!\left[-\frac{T_1}{2(1-\theta)}
+\frac{\theta T_2}{2(1-\theta)(1+2\theta)}\right]}
{(2\pi)^{3/2}(1-\theta)\sqrt{1+2\theta}}.}
$$

The [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md) gives sufficiency. For minimality use the [likelihood-ratio criterion for minimal sufficiency](../../../../../likelihood-ratio-criterion-for-minimal-sufficiency.md). The density ratio for $x,x'$ is independent of $\theta$ precisely when

$$
-\frac{\Delta T_1}{2(1-\theta)}
+\frac{\theta\Delta T_2}{2(1-\theta)(1+2\theta)}
$$

is constant. Multiplying by $2(1-\theta)(1+2\theta)$ shows that its constant would produce a quadratic term on the right whereas the left is linear, so that constant is zero. The remaining coefficients give $\Delta T_1=\Delta T_2=0$. Thus $T$ is [minimal sufficient statistic](../../../../../minimal-sufficient-statistic.md).

Each $X_i$ is standard normal, so $\mathbb E_\theta T_1=3$. The integrable, nonzero function $T_1-3$ has zero expectation for every parameter, proving that $T$ is **not complete**.

By sufficiency, choose a version $S(T)=\mathbb P_\theta(X_1^2\le1\mid T)$ common to all parameters. The tower property gives

$$
\mathbb E_\theta S=\mathbb P_\theta(|X_1|\le1)
=2\Phi(1)-1=:c,\qquad0<c<1.
$$

On the event $T_1<1$ we necessarily have $X_1^2<1$, so $S=1$ there almost surely. This event has positive probability under every parameter because the joint normal density is strictly positive on a ball about the origin. Thus $S$ is not identically $c$. The bounded function $S-c$ has zero expectation for every parameter but is not almost surely zero. Consequently

$$
\boxed{T\text{ is neither complete nor boundedly complete}.}
$$

## ↑ Ancestors (10)

1. [27J](../27j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
