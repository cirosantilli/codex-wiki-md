<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Let $V=f(U)$, the right half-disc from part (i). Write $w=re^{it}$ with $0<r<1$ and $-\pi/2<t<\pi/2$. Squaring doubles the angle and squares the radius, giving a [holomorphic](../../../../../holomorphic-function-split.md) bijection

$$
w\longmapsto w^2:\ V\longrightarrow W=\mathbb D\setminus(-1,0].
$$

Its inverse is the unique square root with positive real part, and its derivative $2w$ is nonzero on $V$. The cut includes zero, because $0\notin V$.

Next, the [Möbius transformation](../../../../../mobius-transformation.md) $T(s)=i(1-s)/(1+s)$ is a [conformal](../../../../../conformal-map.md) bijection from $\mathbb D$ onto $\mathbb H$: it is the inverse [Cayley transform between the half-plane and disk](../../../../../cayley-transform-between-the-half-plane-and-disk.md) composed with $s\mapsto-s$. For $s=-t$, $0\leq t<1$, it gives

$$
T(-t)=i\frac{1+t}{1-t}.
$$

Consequently $T((-1,0])=\{iy:y\geq1\}$. Since $T$ is a bijection on the whole disc, deleting this interval deletes exactly that ray in the image.

The required [function composition](../../../../../function-composition.md) is therefore

$$
\boxed{g(z)=i\frac{1-f(z)^2}{1+f(z)^2}=\frac{2z}{1-z^2}}.
$$

Each component is a [conformal](../../../../../conformal-map.md) bijection between the indicated domains. The only possible denominator zeros of the simplified expression are $z=\pm1$, outside $U$, and

$$
g'(z)=\frac{2(1+z^2)}{(1-z^2)^2}\ne0\quad(z\in U),
$$

since $i$ is on the excluded semicircle and $-i$ is outside the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md). This also checks the local [conformality](../../../../../conformality.md) of the [conformal map from the exterior half-disc to a slit half-plane](../../../../../conformal-map-from-the-exterior-half-disc-to-a-slit-half-plane.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [6](../../../6.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
