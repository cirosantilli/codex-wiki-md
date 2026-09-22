<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

On a connected [Riemann surface](../../../../../riemann-surfaces.md) $R$, a [Perron family of subharmonic functions](../../../../../perron-family-of-subharmonic-functions.md) is a nonempty family $\mathcal P$ of real continuous [subharmonic functions](../../../../../subharmonic-function.md) closed under pairwise maxima and under harmonic lifting on every relatively compact coordinate disk. A [harmonic lifting of a continuous subharmonic function](../../../../../harmonic-lifting-of-a-continuous-subharmonic-function.md) replaces its values inside such a disk by the harmonic [Poisson integral](../../../../../poisson-integral.md) of its boundary values, leaving the function unchanged outside. Harmonic comparison shows that the lift dominates the original function. The lift is continuous and remains subharmonic by harmonic comparison across the circle.

Write $U=\sup_{v\in\mathcal P}v$. Because the family is nonempty and its members are finite, $U$ cannot be minus infinity. Suppose first $U(p)<\infty$, and choose a relatively compact coordinate disk $V$ containing $p$. Choose $v_n\in\mathcal P$ approaching $U(p)$ at $p$. Lift $v_1$ on $V$ to get $h_1$, and recursively lift $\max(h_{n-1},v_n)$ to get $h_n$. These are members of the family, harmonic on $V$, and increasing. Also $h_n(p)\to U(p)$.

The nonnegative [harmonic functions](../../../../../harmonic-function.md) $h_n-h_1$ are bounded at $p$. The [Harnack inequality for harmonic functions](../../../../../harnack-inequality-for-harmonic-functions.md), on chains of compact subdisks, bounds them uniformly on every compact subset of $V$. The [Poisson integral](../../../../../poisson-integral.md) then bounds their derivatives on smaller subdisks. Compact convergence and the [mean value property](../../../../../mean-value-property-for-harmonic-functions.md) show that their increasing limit is finite and harmonic; denote the limit of $h_n$ by $h$.

Fix an arbitrary $v\in\mathcal P$, and let $k_n$ be the lift of $\max(v,h_n)$ on $V$. These functions increase, are harmonic on $V$, and satisfy $h_n\leq k_n\leq U$. They are bounded at $p$, so the same [Harnack inequality for harmonic functions](../../../../../harnack-inequality-for-harmonic-functions.md) argument gives a harmonic limit $k$. At $p$, $k(p)=h(p)=U(p)$, whereas $k\geq h$ on $V$. The nonnegative harmonic difference has an interior zero, so the [strong maximum principle for harmonic functions](../../../../../strong-maximum-principle-for-harmonic-functions.md) gives $k=h$. Since $v\leq k_n$, we have $v\leq h$. Taking the supremum over $v$ gives $U\leq h$, and $h_n\leq U$ gives the opposite inequality. Thus $U=h$ on $V$.

The finite locus of $U$ is open by this argument. It is also closed: if a point is a limit of finite points, choose a coordinate disk around it and a finite point in that disk; the preceding argument applied with that finite point shows that $U$ is finite on the entire disk. [Connectedness](../../../../../connected-space.md) now proves the dichotomy

$$
\boxed{U\equiv+\infty\quad\text{or}\quad U\text{ is finite and harmonic on }R.}
$$

Both occur. The family of all continuous [subharmonic functions](../../../../../subharmonic-function.md) bounded above by zero is a [Perron family of subharmonic functions](../../../../../perron-family-of-subharmonic-functions.md), since the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md) keeps every lift below zero; it contains zero, so its supremum is zero. The family of constant functions with positive integer values is also a [Perron family of subharmonic functions](../../../../../perron-family-of-subharmonic-functions.md), and its supremum is everywhere infinite.

For the final application, the radius must enclose the evaluation point. For $|z|<r<1$ set

$$
H_r(z)=\frac1{2\pi}\int_0^{2\pi}u(re^{i\theta})\frac{r^2-|z|^2}{|re^{i\theta}-z|^2}\,d\theta.
$$

This is the [harmonic lifting of a continuous subharmonic function](../../../../../harmonic-lifting-of-a-continuous-subharmonic-function.md) on the radius-$r$ disk. Hence $H_r\geq u$ there. If $|z|<r<s<1$, $H_s\geq u=H_r$ on the radius-$r$ boundary, so harmonic comparison gives $H_s\geq H_r$ throughout the smaller disk. The increasing limit is either everywhere infinite or finite and harmonic, by the preceding Harnack argument and propagation across overlapping disks. In the finite case it dominates $u$. Any [harmonic majorant](../../../../../harmonic-majorant.md) $h$ of $u$ dominates $H_r$ by boundary comparison and therefore dominates their limit. Thus the precise conclusion is

$$
\boxed{h_{\min}(z)=\lim_{r\uparrow1}H_r(z)=\sup_{|z|<r<1}H_r(z),}
$$

provided a finite [harmonic majorant](../../../../../harmonic-majorant.md) exists. This is the [least harmonic majorant by expanding disk lifts](../../../../../least-harmonic-majorant-by-expanding-disk-lifts.md).

There are two necessary qualifications to the printed formula. First, the supremum cannot include $r<|z|$. For example, if $u\equiv-1$ and $z\ne0$, the kernel has normalized integral $1$ for $r>|z|$ and $-1$ for $r<|z|$. The displayed integral is consequently $-1$ in the first case and $+1$ in the second. The unrestricted supremum would be $+1$, although the least [harmonic majorant](../../../../../harmonic-majorant.md) is $-1$; at $r=|z|$ the kernel is undefined. Second, a finite [harmonic majorant](../../../../../harmonic-majorant.md) need not exist. The continuous [subharmonic function](../../../../../subharmonic-function.md)

$$
u(z)=\frac1{1-|z|^2},\qquad \Delta u(z)=\frac{4(1+|z|^2)}{(1-|z|^2)^3}>0,
$$

has $H_r\equiv(1-r^2)^{-1}\to+\infty$. If $h\geq u$ were harmonic, its centered circular means would equal $h(0)$ and dominate $(1-r^2)^{-1}$ for every $r$, an impossibility. In this case the limit formula holds only in the extended sense, with value $+\infty$ and no finite least [harmonic majorant](../../../../../harmonic-majorant.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
