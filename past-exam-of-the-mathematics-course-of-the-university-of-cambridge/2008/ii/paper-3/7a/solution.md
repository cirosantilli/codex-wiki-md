<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

The map [normal forms](../../../../../normal-form-dynamical-systems.md) at multiplier $+1$ are given in the numbered subparts below. For the multiplier $-1$ problem, the second iterate instead exposes the emerging period-two cycle.

For the multiplier $-1$ problem, write $x=X+\alpha/2$. To the required weighted order, with $X=O(\mu^{1/2})$, the shifted map is $X_{n+1}=-X_n+bX_n+\gamma X_n^2+\delta X_n^3$, where $b=\beta+\alpha\gamma$. Composing it with itself cancels the quadratic term. The cubic contribution is $-2\delta X^3-2\gamma^2X^3$, while the linear correction is $-2bX$. Consequently the [quadratic-cubic flip criticality](../../../../../quadratic-cubic-flip-criticality.md) calculation gives

$$
\boxed{\widehat\mu=-2(\beta+\alpha\gamma),\qquad A=2(\delta+\gamma^2).}
$$

Thus the second iterate has normal form $X_{n+2}=X_n+\widehat\mu X_n-AX_n^3$, up to terms of weighted order at least four. This is the asymptotic interpretation of the stated remainder under $X=O(\mu^{1/2})$; a uniformly valid local expansion about the exact [fixed point](../../../../../fixed-point.md) also retains mixed parameter remainders.

Assuming $\widehat\mu$ crosses zero transversely and $A\ne0$, the small nonzero fixed points of the second iterate satisfy $X^2\sim\widehat\mu/A$. They form a [period-two orbit](../../../../../period-two-orbit.md). For $A>0$ they exist on the side $\widehat\mu>0$, where the original fixed point has become unstable, and the second-iterate multiplier is $1-2\widehat\mu+o(\widehat\mu)$, so the cycle is stable. The [period-doubling bifurcation](../../../../../period-doubling-bifurcation.md) is therefore **supercritical precisely when $\delta+\gamma^2>0$**. Equality is a degenerate case requiring higher-order terms.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
