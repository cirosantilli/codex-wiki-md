<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The first-order [multivariable Taylor expansion](../../../multivariable-taylor-expansion.md) is

$$
f(x,y)=e^{y_0}\bigl[x_0^2+2x_0(x-x_0)+x_0^2(y-y_0)\bigr]+O\bigl((x-x_0)^2+(y-y_0)^2\bigr).
$$

Taking $(x_0,y_0)=(2,0)$ gives the [linear approximation](../../../linear-approximation.md)

$$
\boxed{f(2.03,-0.01)\simeq4+4(0.03)+4(-0.01)=4.08.}
$$

To assess its [significant figures](../../../significant-figures.md), the quadratic [Taylor polynomial](../../../taylor-polynomial.md) supplies the correction $h^2+4hk+2k^2=-0.0001$ for $h=0.03$, $k=-0.01$. Direct evaluation gives $2.03^2e^{-0.01}=4.0798963599\ldots$. Thus the estimate is **correct to four significant figures**: both round to $4.080$, whereas to five significant figures the exact value is $4.0799$ and the approximation is $4.0800$. The unexpectedly small quadratic correction results partly from cancellation of its mixed and unmixed terms.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2016](../../2016-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
