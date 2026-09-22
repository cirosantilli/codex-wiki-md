<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

Use units $c=1$, consistent with comparing $B$ directly to $E$, and metric signature $(+---)$. For an arbitrary [worldline](../../../../../world-line.md) parameter $s$, an action for a charged [relativistic particle](../../../../../relativistic-particle.md) is

$$
\boxed{\mathcal S=-m\int\sqrt{\dot x^\mu\dot x_\mu}\,ds-q\int A_\mu(x)\dot x^\mu\,ds.}
$$

The first term has variation $-m\dot x_\mu/\sqrt{\dot x^2}$ in its momentum, and the coupling gives $-qA_\mu$. The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) therefore read

$$
m\frac d{ds}\left(\frac{\dot x_\mu}{\sqrt{\dot x^2}}\right)
=q(\partial_\mu A_\nu-\partial_\nu A_\mu)\dot x^\nu.
$$

When $s$ is [proper time](../../../../../proper-time.md), $u^\mu=\dot x^\mu$ has $u^\mu u_\mu=1$, giving the covariant [Lorentz force](../../../../../lorentz-force.md)

$$
\boxed{m\frac{du^\mu}{ds}=qF^{\mu\nu}u_\nu.}
$$

With $F^{i0}=E_i$ and $F^{ij}=-\epsilon_{ijk}B_k$, put $e=qE/m$, $b=qB/m$, $\omega=\sqrt{b^2-e^2}$ for nonzero charge. The velocity equations become

$$
\dot u^0=e u^z,\qquad\dot u^x=-b u^z,\qquad\dot u^z=e u^0+b u^x,\qquad u^y=0.
$$

Thus $\ddot u^z=-\omega^2u^z$, with $u^z(0)=0$, $\dot u^z(0)=e$. Integrating with $u^0(0)=1$, $u^x(0)=0$ gives $u^z=(e/\omega)\sin\omega s$, $u^0=1+(e^2/\omega^2)(1-\cos\omega s)$ and $u^x=-(be/\omega^2)(1-\cos\omega s)$. Integrate once more from the origin:

$$
\boxed{\begin{aligned}
x^0(s)&=s+\frac{e^2}{\omega^2}\left(s-\frac{\sin\omega s}{\omega}\right),\\
x^1(s)&=-\frac{be}{\omega^2}\left(s-\frac{\sin\omega s}{\omega}\right),\\
x^2(s)&=0,\\
x^3(s)&=\frac e{\omega^2}(1-\cos\omega s).
\end{aligned}}
$$

For zero charge the trajectory is simply rest, $x^0=s$, with all spatial coordinates zero. The charged trajectory oscillates in $z$ while drifting in the negative $x$ direction, the direction of $\mathbf E\times\mathbf B$. Its displacement-to-time ratio over a proper-time period is $-E/B$. A boost at that drift velocity removes the [electric field](../../../../../electric-field.md) and leaves circular magnetic motion; in the original frame the orbit has repeating cycloidal cusps where the particle is momentarily at rest. Energy oscillates rather than growing indefinitely because $B>E$. In SI units the corresponding magnetic-dominated condition is $cB>E$.

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
