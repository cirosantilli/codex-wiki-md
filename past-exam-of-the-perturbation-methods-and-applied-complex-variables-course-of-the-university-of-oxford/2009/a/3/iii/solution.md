<h1 id="a/3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In the [overlap region](../../../../../overlap-region.md) $\epsilon^{1/3}\ll x\ll1$, write $X=x/\epsilon^{1/3}$. The supplied [Airy function](../../../../../airy-function.md) asymptotics give

$$
Y\sim\frac{\alpha\epsilon^{1/12}}{2\sqrt\pi}x^{-1/4}
e^{-2x^{3/2}/(3\sqrt\epsilon)}
+\frac{\beta\epsilon^{1/12}}{\sqrt\pi}x^{-1/4}
e^{2x^{3/2}/(3\sqrt\epsilon)}.
$$

The outer prefactor $e^{-x^2/4+x/2}$ tends to one in this overlap. Therefore

$$
c_1=\frac{\alpha\epsilon^{1/12}}{2\sqrt\pi},\qquad
c_2=\frac{\beta\epsilon^{1/12}}{\sqrt\pi}.
$$

The recessive condition $c_2=0$ gives $\beta=0$ and $\alpha=1/a_0=3^{2/3}\Gamma(2/3)$. Hence the leading inner answer is

$$
\boxed{y_{\rm in}(x)=\frac{\operatorname{Ai}(x/\epsilon^{1/3})}{\operatorname{Ai}(0)}.}
$$

Away from the turning point, the matched [WKB approximation](../../../../../wkb-approximation.md) is

$$
\boxed{y(x)\sim
\frac{\epsilon^{1/12}}{2\sqrt\pi\,\operatorname{Ai}(0)}
x^{-1/4}\exp\left[-\frac{2x^{3/2}}{3\sqrt\epsilon}-\frac{x^2}4+\frac x2\right].}
$$

A useful [multiplicative composite expansion](../../../../../multiplicative-composite-expansion.md) through the turning region is $e^{-x^2/4+x/2}\operatorname{Ai}(x/\epsilon^{1/3})/\operatorname{Ai}(0)$: it is finite and normalized at zero and matches the displayed outer expression for fixed positive $x$. It is a small-$\epsilon$ approximation across the turning point, not a claim of relative uniform accuracy out to arbitrarily large $x$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
