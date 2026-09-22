<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $E=T-S$. Matching [interpolation](../../../../../interpolation-split.md) data and endpoint [derivatives](../../../../../derivative.md) gives

$$
E(x_i)=0\quad(0\leq i\leq n),\qquad E'(x_0)=E'(x_n)=0.
$$

The endpoint slope constraints make $S$ a [clamped cubic spline](../../../../../clamped-cubic-spline.md). The decisive step in its [minimum roughness property of a clamped cubic spline](../../../../../minimum-roughness-property-of-a-clamped-cubic-spline.md) is the [orthogonality](../../../../../orthogonal-vectors.md) identity

$$
\int_{x_0}^{x_n}S''(x)E''(x)\,dx=0.
$$

Prove it separately on each [interval](../../../../../interval-mathematics.md). Two applications of [integration by parts](../../../../../integration-by-parts.md), using the vanishing [fourth derivative](../../../../../fourth-derivative.md) of the cubic piece, give

$$
\int_{x_{i-1}}^{x_i}S''E''\,dx
=[S''E']_{x_{i-1}}^{x_i}-[S'''E]_{x_{i-1}}^{x_i}
=[S''E']_{x_{i-1}}^{x_i}.
$$

The second boundary term is zero because $E$ vanishes at both endpoints of this [interval](../../../../../interval-mathematics.md). Sum over $i$. At each interior [spline knot](../../../../../spline-knot.md), the two values of $S''E'$ agree because both factors are continuous, so the contributions cancel. The remaining outer boundary terms vanish because $E'$ is zero at both outer endpoints. This proves the identity.

Expanding the square now gives the stronger exact equality

$$
\boxed{\int_{x_0}^{x_n}(T'')^2\,dx
=\int_{x_0}^{x_n}(S'')^2\,dx
+\int_{x_0}^{x_n}(T''-S'')^2\,dx.}
$$

The last [integral](../../../../../integral-split.md) is nonnegative, proving the required inequality. It measures the excess [second derivative roughness penalty](../../../../../second-derivative-roughness-penalty.md) of $T$ over $S$.

The argument applies directly to twice continuously differentiable competitors. More generally it holds when $T'$ is an [absolutely continuous function](../../../../../absolutely-continuous-function.md) and $T''$ is [square-integrable](../../../../../square-integrable-function.md), the usual finite-energy class for this [second derivative roughness penalty](../../../../../second-derivative-roughness-penalty.md). Mere existence of pointwise [second derivatives](../../../../../second-derivative.md) does not by itself guarantee that all displayed [integrals](../../../../../integral-split.md) exist; the variational statement is understood for admissible competitors with this regularity.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
