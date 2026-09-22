<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For small $\varepsilon$, the [conserved quantity](../../../../../../conserved-quantity.md) from part (b) instead obeys $H'=-\varepsilon(\lambda+u)v^2$. The [Melnikov energy-balance method](../../../../../../melnikov-energy-balance-method.md) evaluates the first-order net change along the unperturbed [homoclinic orbit](../../../../../../homoclinic-orbit.md):

$$
\Delta H=-\varepsilon\left(\lambda I_0+I_1\right)+O(\varepsilon^2),\qquad
I_0=\int_{-\infty}^{\infty}v^2\,d\widetilde t>0,\quad
I_1=\int_{-\infty}^{\infty}uv^2\,d\widetilde t.
$$

Using the homoclinic curve $v^2=\frac23(s-u)^2(u+2s)$, these are integrals of $v\,du$ on its two halves. Their weighted mean is $I_1/I_0=-5s/7$. Thus the first-order splitting vanishes at $\lambda=5s/7$. Since its derivative with respect to $\lambda$ is $-I_0\ne0$, the implicit function theorem gives a nearby curve where the stable and unstable saddle separatrices reconnect. This is the [homoclinic balance for a quadratic-force oscillator](../../../../../../homoclinic-balance-for-a-quadratic-force-oscillator.md) and therefore a global, rather than local, bifurcation.

Returning to the original parameters, $q=\varepsilon^2\lambda$ and $\sqrt p=\varepsilon^2\sqrt\kappa$. With fixed positive $\kappa$ and $\varepsilon\to0$, **the homoclinic bifurcation curve has leading form**

$$
\boxed{q=\frac57\sqrt p+o(\sqrt p).}
$$

The energy integral locates the leading curve; the perturbed orbit itself is no longer a constant-$H$ curve.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
