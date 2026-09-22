<h1 id="9/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [stationary point](../../../../../stationary-point.md) is a point where the function is differentiable and its first [derivative](../../../../../derivative.md) vanishes. Interpret the cube root as the real [cube root](../../../../../cube-root.md), and put $q(x)=x^2-8x+7$. Then $f(x)=15+(x-3)\sqrt[3]{q(x)}$. For $x\ne1,7$, the [product rule](../../../../../product-rule.md) and [chain rule](../../../../../chain-rule.md) give

$$
f'(x)=\frac{3q(x)+(x-3)q'(x)}{3\big(\sqrt[3]{q(x)}\big)^2}
=\frac{5x^2-38x+45}{3\big(\sqrt[3]{q(x)}\big)^2}.
$$

The denominator is positive wherever it is defined. Consequently the two stationary abscissae are

$$
\boxed{x_\pm=\frac{19\pm2\sqrt{34}}5.}
$$

Using the stationary equation to simplify the value of $q$ gives $q(x_\pm)=-2(x_\pm+5)/5$. Thus the complete stationary points are

$$
\boxed{\left(x_\pm,\ 15-(x_\pm-3)\sqrt[3]{\frac{2(x_\pm+5)}5}\right).}
$$

Numerically they are approximately $(1.46762,17.10362)$ and $(6.13238,9.84664)$. The numerator of $f'$ is positive outside $[x_-,x_+]$ and negative inside, so the first is a local maximum and the second a local minimum.

At $x=1,7$, the real function is continuous but has a vertical tangent; the factor $x-3$ does not cancel either cube-root singularity. Those points are not stationary points. This is the distinction required when finding [stationary points with real cube-root factors](../../../../../stationary-points-with-real-cube-root-factors.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [2019 resit](../../../../2019-resit-split.md)
5. [Past exam of the mathematical methods II course of the University of Oxford](../../../../split.md)
6. [Mathematical methods II course of the University of Oxford](../../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
