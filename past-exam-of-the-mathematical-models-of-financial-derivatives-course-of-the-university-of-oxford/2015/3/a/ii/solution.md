<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Differentiate the [Black-Scholes formula](../../../../../black-scholes-formula.md) for the [European put option](../../../../../european-put-option.md) with respect to its strike. The [chain rule](../../../../../chain-rule.md) gives

$$
\frac{\partial P}{\partial K}
=e^{-r\tau}\Phi(-d_-)
-Ke^{-r\tau}\phi(d_-)\frac{\partial d_-}{\partial K}
+S\phi(d_+)\frac{\partial d_+}{\partial K}.
$$

The final two terms cancel by both identities in part [i](../i.md). Hence the [put-price strike derivative](../../../../../put-price-strike-derivative.md) is

$$
\boxed{\frac{\partial P}{\partial K}=e^{-r\tau}\operatorname N(-d_-).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../../split.md)
6. [Mathematical models of financial derivatives course of the University of Oxford](../../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
