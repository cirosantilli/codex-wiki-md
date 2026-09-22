<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $s=x+1\in[0,2]$. The drift now vanishes quadratically at the left endpoint, and the [outer expansion](../../../../../../outer-expansion.md) selected from $s=2$ is proportional to $e^{1/s}$, which becomes singular as $s\downarrow0$. The [oscillatory endpoint with a quadratically vanishing drift](../../../../../../oscillatory-endpoint-with-a-quadratically-vanishing-drift.md) is not an ordinary monotone layer of width $\epsilon^{1/3}$: balancing just diffusion and drift on that scale neglects the zeroth-order $y$ term.

The formal local exponential rates obey $\epsilon\lambda^2+s^2\lambda+1=0$. For $s\gg\epsilon^{1/4}$ their slow and fast branches are approximately $-s^{-2}$ and $-s^2/\epsilon$. They coalesce when $s^4\sim4\epsilon$. This locates the main transition a distance $O(\epsilon^{1/4})$ from the left endpoint.

A reliable procedure removes the first [derivative](../../../../../../derivative.md) exactly:

$$
y(s)=e^{-s^3/(6\epsilon)}v(s),\qquad
\epsilon^2v''=P(s)v,\qquad P(s)=\frac{s^4}4+\epsilon s-\epsilon.
$$

Use [WKB approximation](../../../../../../wkb-approximation.md) for this transformed equation on each side of its unique positive zero $s_t=\sqrt2\epsilon^{1/4}+O(\epsilon^{1/2})$. For $s>s_t$ the transformed modes are exponential; for $0<s<s_t$ they are oscillatory. Their physical [amplitudes](../../../../../../wave-amplitude.md) include the displayed exponential prefactor.

At $s_t$, $P'(s_t)=O(\epsilon^{3/4})$, so the [Airy turning-point connection formula](../../../../../../airy-turning-point-connection-formula.md) uses

$$
\boxed{s-s_t=O\!\left((\epsilon^2/P'(s_t))^{1/3}\right)=O(\epsilon^{5/12})}.
$$

This layer connects the oscillatory and exponential [WKB approximation](../../../../../../wkb-approximation.md) branches. On the transition scale $s=\epsilon^{1/4}S$, the exact equation is $\epsilon^{1/2}v_{SS}=(S^4/4-1+\epsilon^{1/4}S)v$, displaying a small effective [WKB approximation](../../../../../../wkb-approximation.md) parameter $\epsilon^{1/4}$.

Close to $s=0$, the local wavelength is $O(\sqrt\epsilon)$: setting $s=\sqrt\epsilon\,\xi$ gives $Y_{\xi\xi}+Y+\sqrt\epsilon\,\xi^2Y_\xi=0$, whose leading solutions are sine and cosine. This endpoint form imposes $y(-1)=1$. Within the oscillatory region, the prefactor changes by order one over the additional envelope scale $s=O(\epsilon^{1/3})$. The $\sqrt\epsilon$ wavelength and $\epsilon^{1/3}$ envelope are subscales of the same oscillatory region, not additional omitted ordinary layers.

Use the outer exponential/regular branches for $s\gg\epsilon^{1/4}$, oscillatory [WKB approximation](../../../../../../wkb-approximation.md) inside the $O(\epsilon^{1/4})$ transition region, an $O(\epsilon^{5/12})$ Airy neighborhood of $s_t$, and the $O(\sqrt\epsilon)$ local endpoint form to apply the left boundary data. Match their constants and enforce the right boundary data at $s=2$; there is no separate right endpoint layer required. Matching [amplitudes](../../../../../../wave-amplitude.md) need not remain $O(1)$, and parameter values admitting a homogeneous Dirichlet solution require a separate solvability check rather than an assumed uniform algebraic expansion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
