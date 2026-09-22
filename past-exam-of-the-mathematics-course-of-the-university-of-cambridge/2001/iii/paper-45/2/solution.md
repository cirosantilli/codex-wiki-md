<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose an explicit orientation convention, since the supplied PDF does not display the referenced diagram. Let $\mathbf e_z$ point upward and $\mathbf e_2$ complete a right-handed frame with the horizontal flow direction $\mathbf e_1$. Use

$$
\mathbf i=\sin\theta\,\mathbf e_1+\cos\theta\,\mathbf e_z,\qquad
\mathbf j=-\cos\theta\,\mathbf e_1+\sin\theta\,\mathbf e_z,
$$

where $\mathbf i$ points from the head towards the tail. A tail point has position $\mathbf r=(a+s)\mathbf i$. Its rotational [velocity](../../../../../velocity.md) is $\Omega(a+s)\mathbf j$, where the scalar $\Omega$ is about $-\mathbf e_2$ and therefore $\dot\theta=-\Omega$. Keeping that sign is essential for stability.

The point lies at height $z=(a+s)\cos\theta$, so the local imposed fluid [velocity](../../../../../velocity.md) is $\alpha(a+s)\cos\theta\,\mathbf e_1$. Its [velocity](../../../../../velocity.md) relative to that fluid has components

$$
\boxed{v_j=U_j+(\Omega+\alpha\cos^2\theta)(a+s),\qquad
v_i=U_i-\alpha\sin\theta\cos\theta(a+s),}
$$

where $U_i=\mathbf U\cdot\mathbf i$ and $U_j=\mathbf U\cdot\mathbf j$. These follow by projection; rigid rotation has no tangential component.

Write $P=m'g$, $H=6\pi\mu a$, $\mathcal T=8\pi\mu a^3/3$, $K=K_NL$, and

$$
I_1=\int_0^L(a+s)ds=aL+\frac{L^2}{2},\qquad
I_2=\int_0^L(a+s)^2ds=a^2L+aL^2+\frac{L^3}{3}.
$$

Let $q=\Omega+\alpha\cos^2\theta$. The [resistive-force theory](../../../../../resistive-force-theory.md) [force](../../../../../force.md) per length on the tail is $-K_Nv_j\mathbf j-\gamma K_Nv_i\mathbf i$. Head drag and excess weight give

$$
(H+K)U_j=-P\sin\theta-K_NI_1q,\qquad
(H+\gamma K)U_i=-P\cos\theta+\gamma K_NI_1\alpha\sin\theta\cos\theta.
$$

The fluid [vorticity](../../../../../vorticity.md) is $\alpha\mathbf e_2$, so its local [angular velocity](../../../../../angular-velocity.md) has scalar component $-\alpha/2$ about our axis. Sphere rotation resistance therefore contributes $-\mathcal T(\Omega+\alpha/2)$. Torque balance about $C$, including gravity acting at $h\mathbf i$, is

$$
0=-Ph\sin\theta-K_N(I_1U_j+I_2q)-\mathcal T(\Omega+\alpha/2).
$$

Eliminating $U_j$ gives the unapproximated local-resistance relation

$$
\left[K_NI_2-\frac{K_N^2I_1^2}{H+K}+\mathcal T\right]q
=P\left[\frac{K_NI_1}{H+K}-h\right]\sin\theta
-\mathcal T\alpha\left(\frac12-\cos^2\theta\right).
$$

Now retain head and tail translation resistance at the same order, as intended by $\sigma=O(L/a)$, but use $a/L\ll1$ in the lever-arm integrals. Thus $I_1\simeq L^2/2$, $I_2\simeq L^3/3$. Sphere rotation resistance is smaller than tail rotation resistance by order $(a/L)^2$, so omit $\mathcal T$ at fixed scaled shear. Also neglect $h$ relative to the tail's hydrodynamic force-centre distance $K_NI_1/(H+K)=O(L)$. Uniform [density](../../../../../density.md) gives

$$
\frac hL=\frac{\pi b^2L(a+L/2)}{L(4\pi a^3/3+\pi b^2L)};
$$

hence this step requires $b^2L/a^3\ll1$, or head-dominated volume. It is consistent with the distinguished logarithmic ordering, but $b\ll a\ll L$ by itself would not ensure it. The model further neglects hydrodynamic interaction between head and tail, and uses low-Reynolds-number local drag.

Under these approximations,

$$
q=\frac{(L^2/2)P\sin\theta}
{(H+K)L^3/3-K_NL^4/4}
=\frac{6P}{L(K+4H)}\sin\theta=2\beta\sin\theta,
$$

so

$$
\boxed{\Omega\simeq2\beta\sin\theta-\alpha\cos^2\theta,\qquad
\beta=\frac{P}{K_NL^2/3+8\pi\mu aL}=\frac{3P}{L(K+4H)}.}
$$

Because $\dot\theta=-\Omega$, its equilibria satisfy $\alpha(1-\sin^2\theta)=2\beta\sin\theta$. Define

$$
s_*=\frac{\alpha}{\beta+\sqrt{\beta^2+\alpha^2}},
$$

with $s_*=0$ at zero shear. The two orientations modulo $2\pi$ are $\theta_s=\arcsin s_*$ and $\theta_u=\pi-\theta_s$. The [derivative](../../../../../derivative.md) of $\dot\theta=\alpha\cos^2\theta-2\beta\sin\theta$ at an equilibrium is

$$
-2\cos\theta(\beta+\alpha\sin\theta).
$$

The second factor is positive, so the branch $\cos\theta_s>0$ is stable and the other is unstable. On the stable branch the tail tip is above $C$: **the head is lower than the far tail end**.

The corresponding leading translation velocities are

$$
\boxed{U_i\simeq\frac{-P\cos\theta+\frac12\gamma K_NL^2\alpha\sin\theta\cos\theta}{H+\gamma K},\qquad
U_j\simeq-\frac{4P}{K+4H}\sin\theta.}
$$

The second formula uses $q=2\beta\sin\theta$ in the normal [force](../../../../../force.md) balance. In the equilibrium orientation $\alpha\cos^2\theta=2\beta\sin\theta$, and $U_z=U_i\cos\theta+U_j\sin\theta$ simplifies to

$$
\boxed{U_z=-\frac{P}{H+\gamma K}
+\frac{PK(1-\gamma)}{(H+\gamma K)(K+4H)}s_*^2.}
$$

This is [shear-dependent settling of a sphere-and-tail body](../../../../../shear-dependent-settling-of-a-sphere-and-tail-body.md). Since $0<\gamma<1$ for a slender filament, $s_*^2$ increases with the magnitude of shear and the signed upward-coordinate [velocity](../../../../../velocity.md) $U_z$ increases towards zero. Equivalently, **increasing shear decreases the downward sedimentation speed**. The formula remains negative throughout this leading model. If $\gamma=1$ there is no shear dependence; reversing the drag [anisotropy](../../../../../anisotropy.md) would reverse the trend. At very large shear, the omitted sphere rotation term proportional to $\mathcal T\alpha$ can become important, so the approximation is not uniform in arbitrarily large $\alpha$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
