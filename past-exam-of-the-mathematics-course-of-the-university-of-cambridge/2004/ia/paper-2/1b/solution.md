<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

For a straight-line solution $y=mx$, substitution into the [differential equation](../../../../../differential-equation-split.md) gives $m=(1-2m)/(2+m)$. Thus $m^2+4m-1=0$, and the two possible slopes are

$$
\boxed{m_\pm=-2\pm\sqrt5.}
$$

These straight lines solve the [differential equation](../../../../../differential-equation-split.md) on either side of the origin. At the origin itself the right-hand side is undefined.

An [isocline](../../../../../isocline.md) of slope $k$ has equation $(1-2k)x-(2+k)y=0$. For $k\ne-2$ it is the straight line $y=(1-2k)x/(2+k)$; for $k=-2$ it is $x=0$, excluding the origin. In particular, $y=x/2$ is the zero-slope [isocline](../../../../../isocline.md). The line $y=-2x$ is excluded from the domain of the [differential equation](../../../../../differential-equation-split.md); slopes tend to infinity on approaching it. Draw the flow vectors proportional to $(1,(x-2y)/(2x+y))$, with positive horizontal component. This specifies orientation by increasing $x$, rather than by an auxiliary time variable.

To integrate, put $y=xu$ where $x\ne0$. Then

$$
xu'=\frac{1-4u-u^2}{2+u},\qquad
\int\frac{2+u}{1-4u-u^2}\,du=\int\frac{dx}{x}.
$$

The left-hand [integral](../../../../../integral.md) is $-\tfrac12\log|1-4u-u^2|$, so the nonconstant-$u$ solutions have the [first integral](../../../../../first-integral.md)

$$
\boxed{y^2+4xy-x^2=C.}
$$

The constant-$u$ solutions omitted by separation are exactly the two straight lines already found, corresponding to $C=0$. Alternatively, differentiating this [first integral](../../../../../first-integral.md) gives $(2y+4x)y'+4y-2x=0$, which recovers the original [differential equation](../../../../../differential-equation-split.md) wherever $2x+y\ne0$ and also verifies continuation through $x=0$ when $y\ne0$.

The [first integral](../../../../../first-integral.md) describes [hyperbolas](../../../../../hyperbola.md) with the two straight-line solutions as [asymptotes](../../../../../asymptote.md). For $C=1$, the upper branch crosses the vertical axis at $(0,1)$ and exists for every real $x$. For $C=-1$, each branch is confined to $|x|\geq1/\sqrt5$ and reaches a vertical tangent on the excluded line $y=-2x$; the corresponding classical solution intervals exclude those endpoints. These give the two distinct types of curves requested in the sketch.

The [initial condition](../../../../../initial-condition.md) selects $C=1$ and the upper branch, hence

$$
\boxed{y(x)=-2x+\sqrt{5x^2+1},\qquad -\infty<x<\infty.}
$$

Here $2x+y=\sqrt{5x^2+1}>0$, so this really is a global solution of the [initial value problem](../../../../../initial-value-problem.md), and $y'(0)=-2$ agrees with the right-hand side.

<a id="1b/image-isoclines-increasing-x-flow-vectors-and-the-two-types-of-solution-hyperbolas"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2-isoclines.png)

**[Figure 1](#1b/image-isoclines-increasing-x-flow-vectors-and-the-two-types-of-solution-hyperbolas). Isoclines, increasing-x flow vectors and the two types of solution hyperbolas**.

## ↑ Ancestors (11)

1. [1B](../1b.md)
2. [Section I](../section-i.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
