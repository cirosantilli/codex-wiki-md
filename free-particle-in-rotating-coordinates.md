# Free particle in rotating coordinates

↑ **Parent:** [Coriolis acceleration](coriolis-acceleration.md)

Consider a ball moving horizontally with no net horizontal [force](force-split.md) in the laboratory. Treat its horizontal motion as that of a free particle: $\mathbf r_{\rm lab}=(ut,0)$ with constant $u>0$. Axes rotating counterclockwise at constant [angular velocity](angular-velocity.md) $\boldsymbol\Omega=\Omega\mathbf e_z$ about the launch point assign it the [position](position.md)

$$
\mathbf r_{\rm rot}=
\begin{pmatrix}\cos\Omega t&\sin\Omega t\\-\sin\Omega t&\cos\Omega t\end{pmatrix}
\begin{pmatrix}ut\\0\end{pmatrix}
=\begin{pmatrix}ut\cos\Omega t\\-ut\sin\Omega t\end{pmatrix}.
$$

This is an exact [rotation matrix](rotation-matrix.md) transformation, with the axes coinciding at $t=0$. Taking $u=0.25\ \mathrm{m\,s^{-1}}$, $\Omega=0.8\ \mathrm{rad\,s^{-1}}$, and $0\leq t\leq3\ \mathrm s$ gives the two views below. At $t=3\ \mathrm s$, the laboratory [position](position.md) is $(0.75,0)\ \mathrm m$, but the rotating [position](position.md) is approximately $(-0.5530,-0.5066)\ \mathrm m$. Both assign the same distance $0.75\ \mathrm m$ from the origin.

<a id="image-one-free-ball-straight-laboratory-trajectory-and-curved-rotating-coordinate-trajectory"></a>
![](coriolis-free-ball-two-frames.png)

**[Figure 9](#image-one-free-ball-straight-laboratory-trajectory-and-curved-rotating-coordinate-trajectory). One free ball: straight laboratory trajectory and curved rotating-coordinate trajectory**.

The entire rotating [acceleration](acceleration.md) must include the [centrifugal acceleration](centrifugal-acceleration.md) as well as the [Coriolis acceleration](coriolis-acceleration.md). To see the balance explicitly, write $c=\cos\Omega t$ and $s=\sin\Omega t$. Direct [differentiation](differentiation.md) gives

$$
\mathbf v_{\rm rot}=u(c-\Omega ts,-s-\Omega tc),
\qquad
\ddot{\mathbf r}_{\rm rot}=u(-2\Omega s-\Omega^2tc,-2\Omega c+\Omega^2ts).
$$

The two apparent contributions are

$$
\begin{aligned}
\mathbf a_{\rm cor}&=u(-2\Omega s-2\Omega^2tc,-2\Omega c+2\Omega^2ts),\\
\mathbf a_{\rm cf}&=u\Omega^2t(c,-s),\\
\ddot{\mathbf r}_{\rm rot}&=\mathbf a_{\rm cor}+\mathbf a_{\rm cf}.
\end{aligned}
$$

At launch $\mathbf r=0$, so only the [Coriolis acceleration](coriolis-acceleration.md) contributes to the initial bending. Later the [centrifugal acceleration](centrifugal-acceleration.md) also contributes; the full curved [trajectory](trajectory.md) cannot be explained by keeping only the [Coriolis force](coriolis-force.md). In particular, $|\mathbf v_{\rm rot}|^2=u^2(1+\Omega^2t^2)$ grows even though the [Coriolis force does no work](coriolis-force-does-no-work.md): the rotating-frame [kinetic energy](kinetic-energy.md) increase is supplied by [work](work.md) from the [centrifugal force](centrifugal-force.md). The laboratory [kinetic energy](kinetic-energy.md) remains $mu^2/2$.

## ↑ Ancestors (7)

1. [Coriolis acceleration](coriolis-acceleration.md)
2. [Coriolis force](coriolis-force.md)
3. [Rotating reference frame](rotating-reference-frame.md)
4. [Reference frame](reference-frame.md)
5. [Mathematical physics](mathematical-physics-split.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Coriolis force](coriolis-force.md)
- [Coriolis force does no work](coriolis-force-does-no-work.md)
- [Rotating-table demonstration of Coriolis deflection](rotating-table-demonstration-of-coriolis-deflection.md)
