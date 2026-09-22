<h1 id="10b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At infinity the [potential energy](../../../../../../potential-energy.md) tends to zero, so the conserved [mechanical energy](../../../../../../mechanical-energy.md) is $E=\tfrac12v_\infty^2$. The [impact parameter](../../../../../../impact-parameter.md) $b$ is the perpendicular distance from the origin to the incoming asymptotic line. Conservation of [angular momentum](../../../../../../angular-momentum.md) gives $|h|=bv_\infty$.

For $b>0$, a [turning point](../../../../../../turning-point.md) of the radial motion satisfies

$$
\frac12v_\infty^2=\frac{b^2v_\infty^2}{2r^2}-\frac Qr,
\qquad
v_\infty^2r^2+2Qr-b^2v_\infty^2=0.
$$

Only the positive root is physical, giving

$$
\boxed{r_{\min}=\frac{\sqrt{Q^2+b^2v_\infty^4}-Q}{v_\infty^2}.}
$$

For $Q=0$ this reduces to the straight-line closest distance $b$.

For nonzero $Q$, put $\eta=bv_\infty^2/|Q|\ll1$. If $Q<0$, the numerator is $|Q|(\sqrt{1+\eta^2}+1)$, so

$$
r_{\min}=\frac{2|Q|}{v_\infty^2}\left(1+\frac{\eta^2}{4}+O(\eta^4)\right).
$$

If $Q>0$, rationalize the numerator instead:

$$
r_{\min}=\frac{b^2v_\infty^2}{\sqrt{Q^2+b^2v_\infty^4}+Q}
=\frac{b^2v_\infty^2}{2Q}\left(1-\frac{\eta^2}{4}+O(\eta^4)\right).
$$

Thus the requested leading distances are

$$
\boxed{r_{\min}\sim\frac{2|Q|}{v_\infty^2}\quad(Q<0),\qquad
r_{\min}\sim\frac{b^2v_\infty^2}{2Q}\quad(Q>0).}
$$

Repulsion gives a finite barrier even for zero [impact parameter](../../../../../../impact-parameter.md); attraction allows much closer passage. At $b=0$, the attractive formula has the limiting closest distance zero, corresponding to collision with the singular centre rather than a positive [turning point](../../../../../../turning-point.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
