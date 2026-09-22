<h1 id="question-2/a/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

On the unit [sphere](../../../../../../../sphere.md), the outward [unit normal vector](../../../../../../../unit-normal.md) is $\mathbf n=\mathbf r$ and $\mathbf u=\mathbf r$. Hence the outward [flux integral](../../../../../../../flux-integral.md) is

$$
\iint_{r=1}\mathbf u\cdot\mathbf n\,dS
=\iint_{r=1}1\,dS=4\pi.
$$

Using [spherical polar coordinates](../../../../../../../spherical-coordinate-system.md) and the [divergence](../../../../../../../divergence.md) from [ii](../ii.md), the [volume integral](../../../../../../../volume-integral.md) over the unit [ball](../../../../../../../ball-mathematics.md) is

$$
\begin{aligned}
\iiint_{r\leq1}\nabla\cdot\mathbf u\,dV
&=4\pi(3-\alpha)\int_0^1r^{2-\alpha}\,dr\\
&=4\pi(3-\alpha)\left[\frac{r^{3-\alpha}}{3-\alpha}\right]_0^1
=\boxed{4\pi}\qquad(\alpha<3).
\end{aligned}
$$

This [improper integral](../../../../../../../improper-integral.md) converges precisely because $2-\alpha>-1$. When the [vector field](../../../../../../../vector-field.md) is singular or fails to be continuously differentiable at the origin, justify the equality by applying the [divergence theorem](../../../../../../../divergence-theorem.md) on $\varepsilon<r<1$. The outward [flux](../../../../../../../flux.md) through its inner [sphere](../../../../../../../sphere.md) is $-4\pi\varepsilon^{3-\alpha}$, so

$$
\iiint_{\varepsilon<r<1}\nabla\cdot\mathbf u\,dV
=4\pi\bigl(1-\varepsilon^{3-\alpha}\bigr)\longrightarrow4\pi.
$$

Thus **the two integrals agree for every $\alpha<3$**, with the limiting interpretation where needed; the classical smoothness hypothesis does not hold for every such $\alpha$.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [a](../../a.md)
3. [Question 2](../../../question-2.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
