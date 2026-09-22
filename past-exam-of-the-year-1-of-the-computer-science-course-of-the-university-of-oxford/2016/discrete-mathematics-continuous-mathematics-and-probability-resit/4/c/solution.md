<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On an interval avoiding $x=0$, divide by $x$ to obtain the first-order [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md)

$$
y'-\frac2x y=x^3\cos x.
$$

An [integrating factor](../../../../../integrating-factor.md) is $\mu(x)=\exp\!\left(\int-2/x\,dx\right)=x^{-2}$. Multiplying through and using the [product rule](../../../../../product-rule.md) gives

$$
\frac{d}{dx}(x^{-2}y)=x\cos x.
$$

By [integration by parts](../../../../../integration-by-parts.md), $\int x\cos x\,dx=x\sin x+\cos x+C$. Consequently

$$
\boxed{y(x)=x^2\bigl(x\sin x+\cos x+C\bigr)}.
$$

The formula differentiates back to the original equation. Although division excluded $x=0$, this formula has a smooth extension there with $y(0)=0$, satisfying the original equation at zero as well.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
