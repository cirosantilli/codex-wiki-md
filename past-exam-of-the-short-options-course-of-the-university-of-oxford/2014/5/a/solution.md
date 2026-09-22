<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a smooth [variation](../../../../variation.md) $y_\varepsilon=y+\varepsilon\eta$. Differentiating the [functional](../../../../functional.md) at zero gives the [first variation](../../../../first-variation.md)

$$
\delta I=\int_a^b(F_y\eta+F_{y'}\eta'+F_{y''}\eta'')\,dx.
$$

Integrate the second term once and the third term twice by [integration by parts](../../../../integration-by-parts.md):

$$
\delta I=\int_a^b\left(F_y-\frac d{dx}F_{y'}+\frac{d^2}{dx^2}F_{y''}\right)\eta\,dx
+\left[\left(F_{y'}-\frac d{dx}F_{y''}\right)\eta+F_{y''}\eta'\right]_a^b.
$$

Choose variations supported away from the endpoints. Stationarity and the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) force

$$
\boxed{F_y-\frac d{dx}F_{y'}+\frac{d^2}{dx^2}F_{y''}=0.}
$$

This is the [Euler-Lagrange equation for a second-derivative functional](../../../../euler-lagrange-equation-for-a-second-derivative-functional.md). With the interior equation imposed, the remaining boundary expression must vanish for every admissible [variation](../../../../variation.md).

At each endpoint, a freely varying value $y$ requires $\boxed{F_{y'}-(F_{y''})'=0}$, and a freely varying slope $y'$ requires $\boxed{F_{y''}=0}$. A fixed value or slope instead makes its corresponding variation zero and supplies no natural condition for that variable. These are the [natural boundary conditions for second-derivative functionals](../../../../natural-boundary-conditions-for-second-derivative-functionals.md), with the value and slope variations treated independently.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
