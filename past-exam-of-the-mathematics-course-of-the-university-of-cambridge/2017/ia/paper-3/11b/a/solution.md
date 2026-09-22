<h1 id="11b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an [arc-length parametrization](../../../../../../arc-length-parametrization.md), the [unit tangent vector](../../../../../../unit-tangent-vector.md) is $t=r'(s)$, with $|t|=1$. Its derivative is perpendicular to $t$. The [curvature of a space curve](../../../../../../curvature-of-a-space-curve.md) is $\kappa=|t'|$; where $\kappa>0$, its [principal normal vector](../../../../../../principal-normal-vector.md) is $n=t'/\kappa$, so $t'=\kappa n$. The [binormal vector](../../../../../../binormal-vector.md) $b=t\times n$ completes the positively oriented [Frenet frame](../../../../../../frenet-frame.md).

Differentiate $b\cdot b=1$ to get $b'\cdot b=0$. Also

$$
\frac d{ds}(b\cdot t)=0
\quad\Longrightarrow\quad b'\cdot t=-b\cdot t'=-\kappa b\cdot n=0.
$$

Thus $b'$ has only an $n$ component. Define the [torsion of a space curve](../../../../../../torsion-of-a-curve.md) by $\tau=-b'\cdot n$, giving $b'=-\tau n$.

Next, $n'\cdot n=0$, and differentiating the other inner products gives $n'\cdot t=-\kappa$ and $n'\cdot b=\tau$. Hence the [Frenet-Serret formulas](../../../../../../frenet-serret-formulas.md) are

$$
\boxed{t'=\kappa n,\qquad b'=-\tau n,\qquad n'=-\kappa t+\tau b.}
$$

These statements require enough smoothness, for example a $C^3$ [curve](../../../../../../curve.md) with positive curvature on the interval under discussion. If $\kappa=0$, the [unit tangent vector](../../../../../../unit-tangent-vector.md) is still defined, but the standard [principal normal vector](../../../../../../principal-normal-vector.md), [binormal vector](../../../../../../binormal-vector.md) and [torsion of a space curve](../../../../../../torsion-of-a-curve.md) need not be; their existence cannot be inferred just from smoothness of the [curve](../../../../../../curve.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11B](../../11b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
