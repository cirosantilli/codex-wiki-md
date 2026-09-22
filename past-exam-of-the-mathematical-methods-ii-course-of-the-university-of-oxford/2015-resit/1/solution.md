<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Start with the [Maclaurin series](../../../maclaurin-series.md) $\cos x=1-x^2/2+x^4/24+O(x^6)$. Put $z=-x^2/2+x^4/24+O(x^6)$ into the [binomial series](../../../binomial-series.md) $(1+z)^{-2}=1-2z+3z^2+O(z^3)$. Keeping terms through $x^4$ gives

$$
(\cos x)^{-2}=1-2\left(-\frac{x^2}{2}+\frac{x^4}{24}\right)+3\left(\frac{x^4}{4}\right)+O(x^6),
$$

so

$$
\boxed{\sec^2x=1+x^2+\frac23x^4+O(x^6)}.
$$

Since $d(\tan x)/dx=\sec^2x$ and $\tan0=0$, term-by-term [integration](../../../integral-split.md) supplies the [constant of integration](../../../constant-of-integration.md) and gives

$$
\boxed{\tan x=x+\frac{x^3}{3}+\frac{2x^5}{15}+O(x^7)}.
$$

The expansions hold near zero; the nearest real poles at $\pm\pi/2$ limit their [radius of convergence](../../../radius-of-convergence.md) to $\pi/2$. The derivative relation also independently checks all three displayed coefficients of the [tangent function](../../../tangent-function.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
