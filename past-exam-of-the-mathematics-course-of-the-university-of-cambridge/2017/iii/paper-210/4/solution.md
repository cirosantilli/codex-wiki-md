<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [natural cubic spline](../../../../../natural-cubic-spline.md) convention appropriate to the interior design knots: the spline is linear on $[a,x_1]$ and $[x_n,b]$. We also need $n\geq2$. These points will be important for uniqueness.

A [cubic spline](../../../../../cubic-spline.md) is a function in $C^2[a,b]$ whose restriction to each of $[a,x_1]$, $[x_1,x_2]$, through $[x_n,b]$ is a [polynomial](../../../../../polynomial-split.md) of degree at most three. A [spline knot](../../../../../spline-knot.md) is a junction between consecutive pieces. For a [natural cubic spline](../../../../../natural-cubic-spline.md), the two exterior pieces are [affine functions](../../../../../affine-function.md); equivalently, one uses the natural endpoint conditions $g''(x_1)=g''(x_n)=0$ on the spline over $[x_1,x_n]$ and then extends linearly with matching [derivatives](../../../../../derivative.md). Merely prescribing $g''(a)=g''(b)=0$ on otherwise arbitrary exterior cubic pieces is a different condition and does not provide the unique interpolant invoked in this question.

The [natural cubic spline interpolant](../../../../../natural-cubic-spline-interpolant.md) $N\mathbf v$ to values $\mathbf v=(v_1,\ldots,v_n)^T$ is the [natural cubic spline](../../../../../natural-cubic-spline.md) satisfying $(N\mathbf v)(x_i)=v_i$. Its existence and uniqueness for $n\geq2$ are the interpolant fact allowed in the PDF. The interpolation map $N$ is a [linear map](../../../../../linear-map.md): a [linear combination](../../../../../linear-combination.md) of interpolants satisfies the same spline, boundary and value conditions, so uniqueness identifies it with the interpolant to the corresponding [linear combination](../../../../../linear-combination.md) of value vectors.

Let $g=N\mathbf v$, let $\widetilde g\in C^2[a,b]$ have the same values, and put $r=\widetilde g-g$. Then $r(x_i)=0$. We prove the orthogonality

$$
\int_a^b g''r''\,dx=0.
$$

Apply [integration by parts](../../../../../integration-by-parts.md) twice on each [polynomial](../../../../../polynomial-split.md) interval. On an interior interval, $g''''=0$, and

$$
\int_{x_i}^{x_{i+1}}g''r''\,dx=[g''r'-g'''r]_{x_i}^{x_{i+1}}.
$$

The $g'''r$ terms vanish because $r$ vanishes at the knots. The $g''r'$ terms cancel at internal knots because $g''$ and $r'$ are [continuous](../../../../../continuous-function.md), and vanish at $x_1,x_n$ because $g''$ is zero there. On the exterior intervals, $g''=0$ identically. Summing therefore gives the claimed orthogonality without assuming that $g'''$ is [continuous](../../../../../continuous-function.md) across knots.

Expanding the square now gives the [minimum roughness property of the natural cubic spline interpolant](../../../../../minimum-roughness-property-of-the-natural-cubic-spline-interpolant.md)

$$
\boxed{\int_a^b(\widetilde g'')^2\,dx
=\int_a^b(g'')^2\,dx+\int_a^b(r'')^2\,dx
\geq\int_a^b(g'')^2\,dx.}
$$

Equality forces $r''=0$ everywhere, since $r''$ is [continuous](../../../../../continuous-function.md). Thus $r$ is an [affine function](../../../../../affine-function.md). It vanishes at two distinct design points, so $r=0$, proving equality if and only if $\widetilde g=g$.

For the penalized fit, take the allowed [spline roughness penalty matrix](../../../../../spline-roughness-penalty-matrix.md) $\Gamma$ to be a [symmetric matrix](../../../../../symmetric-matrix.md) with $\mathbf z^T\Gamma\mathbf z\geq0$; thus it is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md). If its supplied representative were not symmetric, its symmetric part defines the same [quadratic form](../../../../../quadratic-form.md) and is all that is needed. For any $\widetilde g$, let $\mathbf v=(\widetilde g(x_i))_{i=1}^n$. Replacing it by $N\mathbf v$ preserves every fitted value and can only decrease the [second derivative roughness penalty](../../../../../second-derivative-roughness-penalty.md). Therefore it is enough to minimize

$$
Q_\lambda(\mathbf v)=\|\mathbf Y-\mathbf v\|_2^2+\lambda\mathbf v^T\Gamma\mathbf v
$$

over $\mathbb R^n$. The [matrix](../../../../../matrix.md) $A_\lambda=I_n+\lambda\Gamma$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md), since

$$
\mathbf z^TA_\lambda\mathbf z
=\|\mathbf z\|_2^2+\lambda\mathbf z^T\Gamma\mathbf z>0
\qquad(\mathbf z\ne0).
$$

Completing the quadratic or differentiating gives the unique solution

$$
\boxed{\widehat{\mathbf v}_\lambda=(I_n+\lambda\Gamma)^{-1}\mathbf Y,\qquad
\widehat g_\lambda=N\widehat{\mathbf v}_\lambda.}
$$

This is the [cubic smoothing spline](../../../../../cubic-smoothing-spline.md). More explicitly, the normal equations are $(I_n+\lambda\Gamma)\widehat{\mathbf v}_\lambda=\mathbf Y$, and

$$
Q_\lambda(\mathbf v)-Q_\lambda(\widehat{\mathbf v}_\lambda)
=(\mathbf v-\widehat{\mathbf v}_\lambda)^TA_\lambda
(\mathbf v-\widehat{\mathbf v}_\lambda).
$$

For an arbitrary function with fitted vector $\mathbf v$, the earlier orthogonality also gives

$$
S_\lambda(\widetilde g)-S_\lambda(\widehat g_\lambda)
=(\mathbf v-\widehat{\mathbf v}_\lambda)^TA_\lambda
(\mathbf v-\widehat{\mathbf v}_\lambda)
+\lambda\int_a^b\bigl(\widetilde g''-(N\mathbf v)''\bigr)^2\,dx.
$$

Both terms are nonnegative. Equality forces $\mathbf v=\widehat{\mathbf v}_\lambda$ and, by the proved interpolation equality case, $\widetilde g=N\mathbf v=\widehat g_\lambda$. This proves both existence in $C^2[a,b]$ and uniqueness over the entire stated function class, not just over splines.

The argument is deterministic for each observed $\mathbf Y$. The [fixed-design nonparametric regression](../../../../../fixed-design-nonparametric-regression.md) and [homoscedasticity](../../../../../homoscedasticity.md) assumptions motivate the [squared-error loss](../../../../../squared-error-loss.md), but Gaussian errors are not required.

**At least two distinct design points are required for uniqueness.** Question 4 does not explicitly restate $n\geq2$, and this hypothesis is necessary. With one design point, every function $\widetilde g(x)=Y_1+c(x-x_1)$ has zero residual and zero [second derivative roughness penalty](../../../../../second-derivative-roughness-penalty.md), for any real $c$. Thus the printed unrestricted uniqueness conclusion would be false for $n=1$. The corrected theorem assumes at least two distinct knots and the stated linear-tail convention. At $\lambda=0$, uniqueness over all of $C^2[a,b]$ also fails; the stipulated $\lambda>0$ eliminates that degeneracy.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
