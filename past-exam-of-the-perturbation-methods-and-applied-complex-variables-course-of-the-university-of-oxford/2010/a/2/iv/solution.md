<h1 id="a/2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A fixed small-angle approximation alone is insufficient because its error is multiplied by $x$. Introduce the shrinking cutoff $\eta=x^{-1/3}$, which satisfies $\eta\ll\epsilon$ but $\sqrt x\,\eta\to\infty$.

On $[0,\eta]$, the [Taylor expansion](../../../../../taylor-expansion.md) $\sin^2t=t^2+O(t^4)$ gives $x(\sin^2t-t^2)=O(x\eta^4)=O(x^{-1/3})$ uniformly. Thus

$$
e^{-x\sin^2t}=e^{-xt^2}[1+O(x^{-1/3})]
$$

uniformly there, and the two central integrals are asymptotically equal. On $[\eta,\epsilon]$, choose a fixed $c>0$ with $\sin t\geq ct$ for $0\leq t\leq\epsilon$. The [sine](../../../../../sine.md)-integral tail is at most $\epsilon e^{-c^2x\eta^2}=\epsilon e^{-c^2x^{1/3}}$; the Gaussian tail has the same exponential bound with $c=1$. Both are $o(x^{-1/2})$, while the central [Gaussian integral](../../../../../gaussian-integral.md) is asymptotic to $\sqrt\pi/(2\sqrt x)$. Hence

$$
\boxed{\int_0^\epsilon e^{-x\sin^2t}dt\sim\int_0^\epsilon e^{-xt^2}dt.}
$$

This justifies the localized [Laplace method](../../../../../laplace-s-method.md) rather than interchanging a nonuniform approximation with integration.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
