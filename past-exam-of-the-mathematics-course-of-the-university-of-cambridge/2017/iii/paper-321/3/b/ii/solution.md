<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For either scalar equation, the [complementary solution](../../../../../../../homogeneous-solution.md) is

$$
v'_{x,h}=e^{-\epsilon\Omega t}\bigl[A(x)\cos(\Omega t)+B(x)\sin(\Omega t)\bigr],
$$

so initial velocity transients decay when $t\gg(\epsilon\Omega)^{-1}$. In the exact corrected [forced dust epicycle with aerodynamic drag](../../../../../../../forced-dust-epicycle-with-aerodynamic-drag.md), $v'_{x,p}=u\cos\theta$ is a [particular solution](../../../../../../../particular-solution.md), and the original radial equation then gives $v'_{y,p}=u\sin\theta/2$. Consequently

$$
\boxed{\mathbf v'\longrightarrow\mathbf u'\quad\text{at late times}.}
$$

This is [resonant dust entrainment by an epicyclic gas wave](../../../../../../../resonant-dust-entrainment-by-an-epicyclic-gas-wave.md): in the adopted long-wavelength gas approximation, the forcing is a free epicycle of the dust too, so matching the gas makes the drag zero. The convergence holds for every $\epsilon>0$ in this linear model; at $\epsilon=0$ transients never decay, so the zero-drag and late-time limits do not commute.

If instead the printed scalar equation is treated literally for finite $\epsilon$, its particular solution is

$$
\boxed{v'_{x,p}=u\left[\frac4{4+\epsilon^2}\cos\theta+\frac{2\epsilon}{4+\epsilon^2}\sin\theta\right].}
$$

It has amplitude $|u|/\sqrt{1+\epsilon^2/4}$ and phase offset $\arctan(\epsilon/2)$, not exact phase/amplitude agreement. Agreement in that truncated equation means only leading order as $\epsilon\to0$. This distinguishes the intended approximation from a false exact reading of the printed assertion.

There is a further order-of-limits condition: a real finite-wavelength gas wave has $\omega-\Omega\ne0$. Leading resonant entrainment over the damping time requires $|\omega-\Omega|\ll\epsilon\Omega$, or $(kc_s/\Omega)^2\ll\epsilon$. Otherwise solve the dust transfer equations at the actual $\omega$; detuning can reduce the dust response even though $|k|c_s/\Omega\ll1$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
