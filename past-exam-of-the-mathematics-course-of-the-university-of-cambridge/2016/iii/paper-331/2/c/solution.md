<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $k>0$, without loss for this symmetric real base state, and write $s=1+J$, $e=e^{-2\alpha}$, and $y=\widetilde c^{\,2}$. The given quartic becomes a real quadratic $y^2+Ay+B=0$. Its constant term factors as

$$
B=\frac{[2\alpha-s(1+e)][2\alpha-s(1-e)]}{4\alpha^2}.
$$

Therefore $B<0$ exactly when

$$
\frac{2\alpha}{1+e^{-2\alpha}}<1+J<\frac{2\alpha}{1-e^{-2\alpha}}.
$$

A negative product means the two quadratic roots are real and of opposite sign: the [discriminant](../../../../../../discriminant.md) is $A^2-4B>0$. The negative root gives a pair $\widetilde c=\pm i\sqrt{-y_-}$. One sign has positive [temporal growth rate](../../../../../../growth-rate.md) $kc_i$ and is unstable. Using the definitions of the hyperbolic functions gives **the required unstable band**:

$$
\boxed{\frac{\alpha e^\alpha}{\cosh\alpha}<1+J<\frac{\alpha e^\alpha}{\sinh\alpha}.}
$$

This proves the [unstable band of a three-layer stratified shear flow](../../../../../../unstable-band-of-a-three-layer-stratified-shear-flow.md) directly, without needing to solve all four quartic roots.

For the wave interpretation, consider either interface in isolation with decaying [normal modes](../../../../../../normal-mode.md) $\widehat w=w_0e^{-k|z-z_i|}$. Put $S=\Delta U/h$, $U_i=\overline U(z_i)$, and $v=c-U_i$, the intrinsic [phase velocity](../../../../../../phase-velocity.md). At either interface $[\overline\rho]=-\Delta\rho/2$, while $[\overline U']=-S$ at the upper interface and $+S$ at the lower one. The [jump conditions for stratified inviscid shear flow](../../../../../../jump-conditions-for-stratified-inviscid-shear-flow.md) give the [gravity-vorticity interface wave](../../../../../../gravity-vorticity-interface-wave.md) relation

$$
2kv^2-[\overline U']v-\frac{g\Delta\rho}{2\rho_0}=0.
$$

For stable density jumps, $J\geq0$, both intrinsic branches are real. In units $C=2c/\Delta U$, the isolated wave speeds are

$$
C_u=1+\frac{-1\pm\sqrt{1+8\alpha J}}{4\alpha},\qquad
C_l=-1+\frac{1\pm\sqrt{1+8\alpha J}}{4\alpha}.
$$

The upper wave travelling against its positive background current has $C_u=1-[1+\sqrt{1+8\alpha J}]/(4\alpha)$. The lower wave travelling against its negative background current has the opposite speed, $C_l=-C_u$. Their [counterpropagating wave resonance in a three-layer shear flow](../../../../../../counterpropagating-wave-resonance-in-a-three-layer-shear-flow.md) occurs at $C_u=C_l=0$, which gives

$$
\boxed{1+J=2\alpha\quad\text{for the isolated-wave resonance}.}
$$

At large [wavenumber](../../../../../../wavenumber.md), coupling across the separation $h$ is exponentially weak, of order $e^{-kh}=e^{-2\alpha}$. The unstable band becomes

$$
1+J=2\alpha+O(\alpha e^{-2\alpha}),
$$

with full width $4\alpha e^{-2\alpha}+O(\alpha e^{-6\alpha})$. It is a [counterpropagating wave instability](../../../../../../counterpropagating-wave-instability.md): the two waves propagate oppositely relative to their local currents but have almost equal laboratory [phase velocities](../../../../../../phase-velocity.md), allowing weak coupling to lock their phases and extract mean-flow energy. The [unstable band of a three-layer stratified shear flow](../../../../../../unstable-band-of-a-three-layer-stratified-shear-flow.md) thus becomes narrowly concentrated around this resonance. For fixed $J$, arbitrarily large $k$ lies outside that band; large-$k$ resonance requires $J$ to grow with $\alpha$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
