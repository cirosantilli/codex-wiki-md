<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here the drift vanishes at the left endpoint. The outer equation is $xy_0'+y_0=0$, giving $y_0=1/x$ after applying the right boundary value. The ordinary $x=O(\epsilon)$ layer does not balance diffusion and drift: their balance selects $x=O(\sqrt\epsilon)$ instead.

For the [square-root boundary layer at a vanishing drift](../../../../../../../square-root-boundary-layer-at-a-vanishing-drift.md), put $X=x/\sqrt\epsilon$. The inner equation is

$$
Y''+XY'+Y=0,\qquad (Y'+XY)'=0.
$$

Matching $1/x$ requires a leading inner [amplitude](../../../../../../../wave-amplitude.md) of order $\epsilon^{-1/2}$, so an inner expansion with an everywhere order-one leading term would be incorrect. This can be seen directly by integrating the original equation once:

$$
\epsilon y'+xy=C,\qquad
y(x)=e^{-x^2/(2\epsilon)}\left[1+\frac C\epsilon\int_0^x e^{s^2/(2\epsilon)}\,ds\right].
$$

The right boundary value determines

$$
C=\frac{\epsilon(e^{1/(2\epsilon)}-1)}{\int_0^1e^{s^2/(2\epsilon)}ds}=1+O(\epsilon).
$$

In the inner variable the exact representation becomes

$$
Y(X)=e^{-X^2/2}+\frac C{\sqrt\epsilon}e^{-X^2/2}\int_0^X e^{s^2/2}\,ds.
$$

The first term enforces $Y(0)=1$, while the second is zero there and matches $C/(\sqrt\epsilon X)=C/x$ for large $X$. One would expand this integral in the overlap region, determine successive outer terms from the right boundary, and subtract their common expansion. **The endpoint layer has width $\sqrt\epsilon$ and an $O(\epsilon^{-1/2})$ interior peak**, while its value at the endpoint remains one. This distinguishes it from the ordinary exponential layers in the two preceding cases.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 74](../../../../paper-74-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
