<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal V=HL_0$ be the layer volume per unit transverse width. The [gravity-current box model](../../../../../../gravity-current-box-model.md) imposes $hL=\mathcal V$; it approximates the front and scalar balances, rather than an exactly uniform solution of the local [momentum](../../../../../../momentum.md) equation. For a specified constant front [Froude number](../../../../../../froude-number.md) $\operatorname{Fr}$, the [heated particle-laden gravity current](../../../../../../heated-particle-laden-gravity-current.md) satisfies

$$
\boxed{h=\frac{\mathcal V}{L},\qquad
\dot L=\operatorname{Fr}\sqrt{\frac{g\mathcal V(\gamma\phi-\theta)}{L}},\qquad
\dot\phi=-\frac{W_sL}{\mathcal V}\phi,\qquad
\dot\theta=\beta\phi}.
$$

The initial data are $L=L_0$, $\phi=\phi_0$, and $\theta=0$. The [gravity-current front condition](../../../../../../gravity-current-front-condition.md) applies only while $\gamma\phi-\theta\geq0$.

For heating without settling, $\phi=\phi_0$ and $\theta=\beta\phi_0t$. Integration of the front equation gives

$$
\boxed{L(t)=\left[L_0^{3/2}+\frac{\operatorname{Fr}\sqrt{g\mathcal V\phi_0}}{\beta}
\left\{\gamma^{3/2}-(\gamma-\beta t)^{3/2}\right\}\right]^{2/3}},\qquad
0\leq t\leq\frac\gamma\beta.
$$

Hence the [heated gravity-current runout](../../../../../../heated-gravity-current-runout.md) is

$$
\boxed{L_{\max}=\left[L_0^{3/2}+\frac{\operatorname{Fr}\sqrt{g\mathcal V\phi_0}\,\gamma^{3/2}}{\beta}\right]^{2/3}}.
$$

It is reached at the neutral-buoyancy time $\gamma/\beta$ within this front model. A finite-[momentum](../../../../../../momentum.md) current could subsequently coast or lift off: the formula is the maximum predicted by the prescribed [gravity-current front condition](../../../../../../gravity-current-front-condition.md), which contains no independent front inertia.

For settling without heating, $\theta=0$. Set $K=\operatorname{Fr}\sqrt{g\gamma\mathcal V}$, so $\dot L=K\sqrt\phi\,L^{-1/2}$. Eliminating time yields

$$
\frac{d\sqrt\phi}{dL}=-\frac{W_sL^{3/2}}{2\mathcal V K},\qquad
\sqrt\phi=\sqrt{\phi_0}-\frac{W_s}{5\mathcal V K}(L^{5/2}-L_0^{5/2}).
$$

Thus the [runout length of a gravity current](../../../../../../runout-length-of-a-gravity-current.md) is

$$
\boxed{L_{\max}=\left[L_0^{5/2}+
\frac{5\operatorname{Fr}\mathcal V^{3/2}\sqrt{g\gamma\phi_0}}{W_s}\right]^{2/5}}.
$$

This length is approached as $t\to\infty$, because positive concentration cannot disappear at a finite time under the settling law. If distance means displacement from the removed barrier, the answer is $L_{\max}-L_0$ in either case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
