<h1 id="a/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $x=\delta X$ and write $y(x)=Y(X)$. The equation becomes

$$
\frac{\epsilon}{\delta^2}Y''+\delta^{\alpha-1}X^\alpha Y'+Y=0.
$$

A [dominant balance](../../../../../dominant-balance.md) must compare all three coefficients, rather than just the two derivative terms.

For $-1<\alpha<1$, balancing diffusion and drift gives $\delta=\epsilon^{1/(\alpha+1)}$. Their common coefficient tends to infinity, so the reaction term is smaller and the leading inner equation is

$$
Y''+X^\alpha Y'=0,\qquad
Y'=C\exp[-X^{\alpha+1}/(\alpha+1)].
$$

This derivative is integrable at infinity, allowing an ordinary localized endpoint adjustment. Thus **the thickness is $\epsilon^{1/(\alpha+1)}$** in this range.

For $\alpha=1$, $\delta=\sqrt\epsilon$ makes all three terms comparable. Keep all of them:

$$
Y''+XY'+Y=0.
$$

One decaying solution is $e^{-X^2/2}$, and reduction of order gives the other. This is a **square-root-thickness layer with all terms retained**.

For $\alpha>1$, the first variation scale is $\delta=\sqrt\epsilon$. Keep diffusion and reaction, and drop drift at this scale:

$$
Y''+Y=0.
$$

This leading motion is oscillatory, not a monotone decaying boundary-layer profile. To describe localization one must also resolve the slower damping envelope. Removing the first derivative in the original equation by

$$
y=\exp\left[-\frac{x^{\alpha+1}}{2\epsilon(\alpha+1)}\right]v
$$

gives

$$
v''+\left[\frac1\epsilon-\frac{\alpha x^{\alpha-1}}{2\epsilon}
-\frac{x^{2\alpha}}{4\epsilon^2}\right]v=0.
$$

Near the endpoint the wavelength is $O(\sqrt\epsilon)$, while the envelope changes on $x=O(\epsilon^{1/(\alpha+1)})$. Hence an oscillatory endpoint region is possible, but **it has distinct wavelength and envelope scales**; calling the diffusion-drift balance alone its leading equation would incorrectly discard the reaction term. This generalizes the [oscillatory endpoint with a quadratically vanishing drift](../../../../../oscillatory-endpoint-with-a-quadratically-vanishing-drift.md).

For $\alpha\leq-1$, the diffusion-drift balance would require $\delta^{\alpha+1}=\epsilon$, which gives no shrinking positive power scale. At every shrinking scale the singular drift dominates diffusion, so no regular finite-amplitude diffusion boundary layer of the preceding kind occurs. The coefficient itself is singular at zero; singular endpoint solutions are a different issue from a bounded boundary-layer correction.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
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
