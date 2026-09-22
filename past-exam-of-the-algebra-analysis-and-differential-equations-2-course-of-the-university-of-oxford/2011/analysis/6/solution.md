<h1 id="analysis/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [conformal map](../../../../conformal-map.md) preserves angles between intersecting regular curves, including their orientation. If $f$ is holomorphic with $f'(a)\neq0$, the image tangent vectors are $f'(a)$ times the original tangent vectors. Multiplication by this nonzero complex number gives a common positive scaling and rotation, so their oriented angle is unchanged. This proves conformality throughout the stated domain.

At a zero [derivative](../../../../derivative.md) this can fail: $f(z)=z^2$ at zero sends rays of arguments $0$ and $\pi/4$ to rays of arguments $0$ and $\pi/2$. The angle is doubled, so this [holomorphic function](../../../../holomorphic-function-split.md) is not conformal there.

For the disk map $C(z)=i(1+z)/(1-z)$, compute

$$
\operatorname{Im}C(z)=\frac{1-|z|^2}{|1-z|^2}>0,
\qquad C'(z)=\frac{2i}{(1-z)^2}\neq0.
$$

Its inverse is $z=(w-i)/(w+i)$; for $\operatorname{Im}w>0$, the inequality $|w-i|<|w+i|$ puts this inverse in the unit disk. Both rational maps are holomorphic on their respective domains. Thus

$$
\boxed{C:D\to\mathbb H\text{ is a conformal bijection}.}
$$

For the final region, writing $z=x+iy$ gives $|e^z|=e^x\in(0,1)$ and $\arg(e^z)=y\in(0,\pi)$. Hence its exponential image is exactly the upper half of the unit disk,

$$
V=\{w:|w|<1,\ \operatorname{Im}w>0\}.
$$

The exponential is [injective](../../../../injective-function.md) on this strip, since two equal exponential values differ by $2\pi i$ times an integer while the imaginary parts here differ by less than $\pi$. Its [derivative](../../../../derivative.md) never vanishes and its inverse on $V$ is the logarithm with argument in $(0,\pi)$.

Now $L(w)=(1+w)/(1-w)$ maps $V$ conformally onto the first quadrant. Indeed

$$
\operatorname{Re}L(w)=\frac{1-|w|^2}{|1-w|^2}>0,\qquad
\operatorname{Im}L(w)=\frac{2\operatorname{Im}w}{|1-w|^2}>0,
$$

and the inverse $(s-1)/(s+1)$ has modulus below one and positive imaginary part for every first-quadrant $s$. Squaring maps that quadrant bijectively onto $\mathbb H$, with nonzero [derivative](../../../../derivative.md). Therefore a required composition is

$$
\boxed{F(z)=\left(\frac{1+e^z}{1-e^z}\right)^2.}
$$

Every component is a conformal bijection between the stated domains, so the composition is one as well.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Analysis](../../analysis.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
