<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here the [singular perturbation](../../../../../../singular-perturbation.md) has an exact conservative structure:

$$
(\epsilon y'+xy)'=0,\qquad \epsilon y'+xy=C.
$$

The [integrating factor](../../../../../../integrating-factor.md) for this [first-order linear differential equation](../../../../../../first-order-linear-differential-equation.md) gives

$$
y(x)=e^{-x^2/(2\epsilon)}\left[D+\frac C\epsilon\int_0^x e^{s^2/(2\epsilon)}ds\right].
$$

At $x=1$ and $x=-1$ the integral terms have opposite signs while the exponential factors agree. Equal boundary data therefore force $C=0$, and normalization gives the unique exact solution

$$
\boxed{y(x)=\exp\left(\frac{1-x^2}{2\epsilon}\right)}.
$$

This exposes the [Gaussian interior layer of a conservative drift equation](../../../../../../gaussian-interior-layer-of-a-conservative-drift-equation.md). Its central scale is **$x=O(\sqrt\epsilon)$**, where $x=\sqrt\epsilon\,\xi$ gives $Y''+\xi Y'+Y=0$. The central [Gaussian function](../../../../../../gaussian-function.md) profile is $e^{-\xi^2/2}$ with [amplitude](../../../../../../wave-amplitude.md) $e^{1/(2\epsilon)}$.

Away from the center, $|x|\gg\sqrt\epsilon$, use exponential [WKB approximation](../../../../../../wkb-approximation.md) branches rather than an assumed bounded algebraic outer solution. The reduced [ordinary differential equation](../../../../../../ordinary-differential-equation.md) $xy_0'+y_0=0$ would give $C/x$; matching both equal positive endpoint values with that algebraic branch is impossible. The exact solution selects its zero coefficient and the exponentially large branch with a [Gaussian function](../../../../../../gaussian-function.md) profile instead. Near either endpoint, a distance $O(\epsilon)$ changes $y$ by order one relative to its endpoint value: with $r=(1-|x|)/\epsilon$, $y=e^{r-\epsilon r^2/2}$. These endpoint scales describe normalization of the same global exponential solution.

Thus a central $O(\sqrt\epsilon)$ turning region, exponential outer regions on both sides, and $O(\epsilon)$ endpoint normalization scales give the complete regional description. **The peak is exponentially large**, so no uniformly bounded regular [outer expansion](../../../../../../outer-expansion.md) should be presumed. The exact expression already provides a uniform solution without further matching calculations.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
