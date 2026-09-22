<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Take $+y$ upwards in the source diagram. Write $w$ for $B$'s incoming [speed](../../../speed.md), so the initial [velocities](../../../velocity.md) are

$$
\mathbf u_A=(-u,0),\qquad
\mathbf u_B=\left(\frac{\sqrt3}{2}w,\frac12w\right).
$$

**A contact-direction assumption is needed for a unique answer.** The diagram specifies the incoming [velocities](../../../velocity.md) but does not specify the contact normal or an outgoing [angle](../../../angle.md). First adopt the usual intended model: the [impulse](../../../impulse.md) is horizontal, so neither particle changes its $y$ component of [velocity](../../../velocity.md). This is the smooth [oblique collision](../../../oblique-collision.md) model with a horizontal line of centres at impact. Bringing $A$ to rest in the $x$ direction then brings it entirely to rest.

Let $b$ be $B$'s outgoing $x$ component of [velocity](../../../velocity.md). [Conservation of momentum](../../../momentum-conservation.md) and conservation of [kinetic energy](../../../kinetic-energy.md) give

$$
-3u+\frac{\sqrt3}{2}w=b,
\qquad
3u^2+w^2=b^2+\frac14w^2.
$$

Put $q=(\sqrt3/2)w$. The second equation becomes $3u^2+q^2=(q-3u)^2$, so $q=u$. Therefore

$$
\boxed{w=\frac{2u}{\sqrt3},\qquad
\mathbf v_A=(0,0),\qquad
\mathbf v_B=\left(-2u,\frac{u}{\sqrt3}\right).}
$$

The outgoing [kinetic energies](../../../kinetic-energy.md) are

$$
\boxed{K_A=0,\qquad K_B=\frac12m\left(4u^2+\frac{u^2}{3}\right)=\frac{13}{6}mu^2.}
$$

The outgoing [speed](../../../speed.md) of $B$ is $u\sqrt{13/3}$, directed above the negative $x$ axis at [angle](../../../angle.md) $\tan^{-1}[1/(2\sqrt3)]\simeq16.1^\circ$. The initial [kinetic energy](../../../kinetic-energy.md) is also $(3/2+2/3)mu^2=13mu^2/6$, as required for an [elastic collision](../../../elastic-collision.md).

For the [perfectly inelastic collision](../../../perfectly-inelastic-collision.md) with these same incoming [velocities](../../../velocity.md), both particles share a common outgoing [velocity](../../../velocity.md). [Conservation of momentum](../../../momentum-conservation.md) gives

$$
\boxed{\mathbf V=\frac{3m\mathbf u_A+m\mathbf u_B}{4m}
=\left(-\frac u2,\frac{u}{4\sqrt3}\right),\qquad
|\mathbf V|=\frac{\sqrt{13}}{4\sqrt3}u.}
$$

Its direction is again $16.1^\circ$ above the negative $x$ axis. The separate translational [kinetic energies](../../../kinetic-energy.md) of the constituents and their total are

$$
\boxed{K_A=\frac{13}{32}mu^2,\qquad K_B=\frac{13}{96}mu^2,\qquad
K_{\rm final}=\frac{13}{24}mu^2.}
$$

The loss of translational [kinetic energy](../../../kinetic-energy.md) is

$$
\boxed{K_{\rm initial}-K_{\rm final}=\frac{13}{8}mu^2.}
$$

This becomes internal [energy](../../../energy-split.md), for example deformation and heating; total [energy](../../../energy-split.md) is conserved. In the [elastic collision](../../../elastic-collision.md) no [kinetic energy](../../../kinetic-energy.md) is lost and the particles separate with different [velocities](../../../velocity.md). In the [perfectly inelastic collision](../../../perfectly-inelastic-collision.md) relative motion disappears and the common [velocity](../../../velocity.md) is the original [centre of mass](../../../center-of-mass.md) [velocity](../../../velocity.md).

The limitation of the printed data can be made explicit. Without the horizontal-[impulse](../../../impulse.md) assumption, write the final [velocity](../../../velocity.md) of $A$ as $(0,h)$. Then [conservation of momentum](../../../momentum-conservation.md) determines

$$
\mathbf v_B=\left(\frac{\sqrt3}{2}w-3u,\frac12w-3h\right),
$$

and conservation of [kinetic energy](../../../kinetic-energy.md) gives only

$$
\boxed{w(\sqrt3u+h)=2u^2+4h^2.}
$$

There is a family of possibilities. For a concrete second solution, $h=u/\sqrt3$ gives

$$
w=\frac{5\sqrt3}{6}u,\qquad
\mathbf v_A=\left(0,\frac{u}{\sqrt3}\right),\qquad
\mathbf v_B=\left(-\frac74u,-\frac{7\sqrt3}{12}u\right).
$$

These [velocities](../../../velocity.md) conserve both components of [momentum](../../../momentum-split.md) and conserve [kinetic energy](../../../kinetic-energy.md), and they satisfy the specified vanishing $x$ component for $A$, while requiring a different incoming [speed](../../../speed.md). They can arise from a smooth contact normal proportional to $(1,1/\sqrt3)$. Thus the horizontal-[impulse](../../../impulse.md) result is conditional, rather than uniquely implied by the printed statement. For any member of this family the corresponding sticking result remains well determined once $w$ is chosen:

$$
\mathbf V=\frac14\left(-3u+\frac{\sqrt3}{2}w,\frac12w\right),\qquad
K_{\rm final}=2m|\mathbf V|^2,\qquad
\Delta K=\frac{3m}{8}\left(\left[u+\frac{\sqrt3}{2}w\right]^2+\frac{w^2}{4}\right).
$$

The last expression is the lost relative [kinetic energy](../../../kinetic-energy.md) in a [perfectly inelastic collision](../../../perfectly-inelastic-collision.md) of these two [point masses](../../../point-mass.md).

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2021](../../2021-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
