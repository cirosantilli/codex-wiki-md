<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Away from the line source, insert a leading [wavefront](../../../../../../wavefront.md) form $u\sim a(\mathbf x)W(t-T(\mathbf x))$ into the [shear-horizontal wave](../../../../../../shear-horizontal-wave.md) equation and match the two most singular orders. The first gives the [eikonal equation](../../../../../../eikonal-equation.md) $|\nabla T|=1/\beta$. The next gives

$$
2\nabla T\cdot\nabla a+a\Delta T=0,
\qquad\nabla\cdot(a^2\nabla T)=0.
$$

Equivalently, [SH ray-tube amplitude transport](../../../../../../sh-ray-tube-amplitude-transport.md) conserves $\rho\beta a^2J$, where $J$ is the transverse width of a two-dimensional ray tube. A line source has straight radial [elastic rays](../../../../../../elastic-ray.md) and $J=r\,d\theta$ for fixed angular width, so

$$
\boxed{a(r)=C r^{-1/2}}.
$$

The same geometrical spreading applies to the first nonzero derivative discontinuity or leading [wavefront](../../../../../../wavefront.md) singularity; the source history determines which waveform $W$ and normalization $C$ occur. In three dimensions a point source instead has $J\propto r^2$ and amplitude proportional to $r^{-1}$.

This does not contradict the [SH line-source near-field singularity](../../../../../../sh-line-source-near-field-singularity.md). Ray transport describes an arrival-front limit with $t-r/\beta$ small, or the high-[frequency](../../../../../../frequency.md) field outside the immediate source neighborhood. The logarithm describes $r\downarrow0$ at fixed elapsed time and includes the tail behind the two-dimensional [wavefront](../../../../../../wavefront.md). For example, a causal step force $F_0H(t)$ has the exact radial displacement

$$
u(r,t)=\frac{F_0}{2\pi\mu}\operatorname{arcosh}\frac{\beta t}{r}\ H(t-r/\beta).
$$

For $r\ll\beta t$, this is $F_0\log(2\beta t/r)/(2\pi\mu)$, the near-source logarithm. For $t=r/\beta+\tau$ with $0<\tau\ll r/\beta$, it is

$$
\boxed{u\sim\frac{F_0\sqrt{2\beta}}{2\pi\mu}\,r^{-1/2}\sqrt\tau}.
$$

The coefficient of the leading arrival singularity therefore has exactly the ray-theory dependence. A force impulse gives the corresponding $r^{-1/2}H(\tau)/\sqrt\tau$ leading field. **The limits describe different regions of one causal solution; neither is a uniform approximation to the other**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
