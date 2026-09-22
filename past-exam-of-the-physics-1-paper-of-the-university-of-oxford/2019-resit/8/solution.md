<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

In the [laboratory frame](../../../laboratory-frame.md), the initial target is at rest and the outgoing directions are directly related to detector positions. The [centre-of-momentum frame](../../../center-of-momentum-frame.md) has zero total [momentum](../../../momentum-split.md), so the two outgoing [momenta](../../../momentum-split.md) are equal and opposite; it cleanly separates bulk motion from relative [kinetic energy](../../../kinetic-energy.md). Transforming back is needed to predict laboratory angles and [speeds](../../../speed.md). Neither [reference frame](../../../reference-frame.md) removes the need for an appropriate collision law.

Take the incident direction as $\widehat{\mathbf x}$ and put $S=M_1+M_2$. [Momentum conservation](../../../momentum-conservation.md) fixes the [centre-of-momentum frame](../../../center-of-momentum-frame.md) [velocity](../../../velocity.md), and a [Galilean transformation](../../../galilean-transformation.md) gives the initial [velocities](../../../velocity.md) in that frame:

$$
\boxed{\mathbf V=\frac{M_1u_1}{S}\widehat{\mathbf x},\qquad
\mathbf w_1=\frac{M_2u_1}{S}\widehat{\mathbf x},\qquad
\mathbf w_2=-\frac{M_1u_1}{S}\widehat{\mathbf x}.}
$$

After the [collision](../../../collision.md), $M_1\mathbf w'_1+M_2\mathbf w'_2=0$. Hence both particles have the same final-to-initial [speed](../../../speed.md) ratio,

$$
q=\frac{|\mathbf w'_1|}{|\mathbf w_1|}
=\frac{|\mathbf w'_2|}{|\mathbf w_2|}
=\frac{|\mathbf v'_1-\mathbf v'_2|}{u_1}.
$$

The relative [kinetic energy](../../../kinetic-energy.md) is multiplied by $q^2$. This common ratio exists independently of how the outgoing direction is selected.

**The meaning of restitution matters here.** The usual [coefficient of restitution](../../../coefficient-of-restitution.md) $e_n$ is a ratio of normal separation and approach [speeds](../../../speed.md), not total [speeds](../../../speed.md). In a smooth [oblique collision](../../../oblique-collision.md), the tangential relative [velocity](../../../velocity.md) is unchanged. If the incoming relative [velocity](../../../velocity.md) makes angle $\chi$ to the contact normal, then

$$
\boxed{q^2=e_n^2\cos^2\chi+\sin^2\chi.}
$$

For example, $e_n=1/2$ and $\chi=\pi/4$ give $q=\sqrt{5/8}\ne1/2$. Therefore the requested identification is not generally true with the standard normal definition. The printed equation is valid if its $e$ denotes the [relative speed retention in an oblique collision](../../../relative-speed-retention-in-an-oblique-collision.md), namely $e=q$, or if an additional collision model supplies that equality. The elastic cases have $q=e_n=1$ and are unaffected by this qualification.

To derive the scattering formula under that convention, write $\mathbf v'_1=\mathbf V+\mathbf w'_1$. Its components give the [laboratory scattering circle](../../../laboratory-scattering-circle.md)

$$
(v_1\cos\theta_1-V)^2+(v_1\sin\theta_1)^2
=q^2\left(\frac{M_2u_1}{S}\right)^2.
$$

Solving the resulting quadratic for the nonnegative [speed](../../../speed.md) yields

$$
\boxed{\frac{v_1}{u_1}=\frac{M_1}{S}\left[\cos\theta_1\pm
\sqrt{\cos^2\theta_1-1+q^2\left(\frac{M_2}{M_1}\right)^2}\right].}
$$

With $q=e$, this is the requested formula. A real square root and $v_1\ge0$ are both necessary: a negative algebraic root is not a second physical [speed](../../../speed.md), and $v_1=0$ does not define a [scattering angle](../../../scattering-angle.md). The subsequent limits are taken using this [laboratory scattering circle](../../../laboratory-scattering-circle.md).

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
