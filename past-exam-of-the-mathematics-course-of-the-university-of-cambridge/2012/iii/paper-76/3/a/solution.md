<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $\epsilon\downarrow0$ and fixed $A>0$. Away from the degenerate endpoint $x=0$, the reduced equation is $Ay_0'+y_0=0$. The positive drift makes the rapidly varying homogeneous mode decay as one moves away from the left boundary, so the [outer solution](../../../../../../outer-expansion.md) is selected by the right [boundary condition](../../../../../../boundary-condition.md):

$$
\boxed{y_{\rm out,0}(x)=e^{(1-x)/A}.}
$$

It does not satisfy the left value: its limit there is $L=e^{1/A}$.

If the layer width is $\delta$, diffusion is $O(\epsilon/\delta^2)$, while $Axy'$ is $O(A)$ because the drift vanishes linearly. Their [dominant balance](../../../../../../dominant-balance.md) gives the [square-root boundary layer at a vanishing drift](../../../../../../square-root-boundary-layer-at-a-vanishing-drift.md)

$$
\boxed{x=O(\sqrt{\epsilon/A}),\qquad\xi=x\sqrt{A/\epsilon}.}
$$

Writing $y=Y(\xi)$ gives $Y''+\xi Y'+[\sqrt\epsilon/A^{3/2}]\xi Y=0$. The first nonzero [inner expansion](../../../../../../inner-expansion.md) satisfies $Y_0''+\xi Y_0'=0$, hence $Y_0'=Be^{-\xi^2/2}$. Imposing $Y_0(0)=1$ and matching $Y_0(\infty)=L$ gives

$$
\boxed{Y_0(\xi)=1+(e^{1/A}-1)\operatorname{erf}(\xi/\sqrt2).}
$$

The [overlap region](../../../../../../overlap-region.md) is $\sqrt{\epsilon/A}\ll x\ll1$ for fixed $A$. The [additive composite expansion](../../../../../../additive-composite-expansion.md)

$$
y_{\rm comp,0}=e^{(1-x)/A}+(1-e^{1/A})\operatorname{erfc}\!\left(x\sqrt{\frac A{2\epsilon}}\right)
$$

combines the two leading approximations and satisfies the left value exactly and the right value up to an exponentially small term. Only the first nonzero terms were requested; higher matching terms need not be added.

For fixed $A<0$, the decaying fast mode is at the other endpoint. The [outer solution](../../../../../../outer-expansion.md) is now fixed by $y(0)=1$, giving $e^{-x/A}$. At $x=1$ the drift does not vanish, so the right layer has width $O(\epsilon/|A|)$, with leading transient proportional to $e^{-|A|(1-x)/\epsilon}$. In particular its leading inner profile is $e^{-1/A}+(1-e^{-1/A})e^{-\eta}$, where $\eta=|A|(1-x)/\epsilon$. The vanishing drift at the left endpoint does not require an order-one mismatch layer for these data.

For $A=0$, the reduced equation is $xy_0=0$, which cannot supply the nonzero endpoint values. The equation becomes an [Airy ordinary differential equation](../../../../../../airy-ordinary-differential-equation.md): $x=\epsilon^{1/3}\xi$ gives $Y''+\xi Y=0$. The exact solutions are combinations of $\operatorname{Ai}(-x/\epsilon^{1/3})$ and $\operatorname{Bi}(-x/\epsilon^{1/3})$. For $x>0$ they oscillate, with local wavelength of order $\sqrt{\epsilon/x}$, rather than forming a decaying exponential layer matched to a smooth nonzero outer profile. The $O(\epsilon^{1/3})$ region resolves the turning endpoint, but oscillations extend throughout the interval. Boundary-value resonances can occur at isolated parameter values. Thus setting $A=0$ is not a continuous substitution into either fixed-sign layer approximation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
