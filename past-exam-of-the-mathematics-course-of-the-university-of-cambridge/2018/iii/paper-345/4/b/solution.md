<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use locally bed-tangent [drag force](../../../../../../drag-physics.md), consistent with interpreting $\tau$ as bed [shear stress](../../../../../../shear-stress.md). Let the bed rise downstream at angle $\alpha$ and retain the same effective [drag coefficient](../../../../../../drag-coefficient.md). The normal reaction is $R=G\cos\alpha$, while the opposing downslope component of [submerged weight](../../../../../../submerged-weight.md) is $G\sin\alpha$. At impending upslope motion,

$$
F_D=G\sin\alpha+\mu_sG\cos\alpha.
$$

Thus the [inclined-bed sediment threshold](../../../../../../inclined-bed-sediment-threshold.md) is

$$
\boxed{\Theta_{\mathrm{th},0}(\alpha)=\frac4{3C_D}(\mu_s\cos\alpha+\sin\alpha)
=\Theta_{\mathrm{th},0}\left(\cos\alpha+\frac{\sin\alpha}{\mu_s}\right)}.
$$

For $|\alpha|\ll1$,

$$
\boxed{\tau_{\mathrm{th}}(\alpha)=\tau_{\mathrm{th},0}\left(1+\frac\alpha{\mu_s}\right)+O(\alpha^2)}.
$$

An uphill slope increases the [sediment entrainment threshold](../../../../../../sediment-entrainment-threshold.md); a downhill slope lowers it, until spontaneous gravity-driven motion invalidates the resting-bed model.

There is a geometric convention to specify: if the [drag force](../../../../../../drag-physics.md) remains horizontal while the bed tilts, then $R=G\cos\alpha+F_D\sin\alpha$. The corresponding [force balance](../../../../../../force-balance.md) gives instead

$$
\Theta_{\mathrm{th}}^{\mathrm{horizontal\ drag}}
=\frac4{3C_D}\frac{\mu_s\cos\alpha+\sin\alpha}{\cos\alpha-\mu_s\sin\alpha}
=\Theta_{\mathrm{th},0}\left[1+(\mu_s+\mu_s^{-1})\alpha+O(\alpha^2)\right].
$$

The subsequent bed [shear stress](../../../../../../shear-stress.md) analysis uses the first, locally tangent convention. The two interpretations should not be mixed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
