<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In centre-of-mass and relative coordinates, the kinetic energy separates into centre-of-mass motion plus $\mu v^2/2$, while the mutual potential is $-GM_1M_2/r=-GM\mu/r$. In the centre-of-mass frame the orbital energy is therefore

$$
\boxed{E=\mu\left(\frac12v^2-\frac{GM}{r}\right)}.
$$

The force is central, so the specific relative angular momentum $h=r^2\dot\theta$ is conserved. With $u=1/r$, the radial equation becomes the [Binet equation](../../../../../binet-equation.md)

$$
u''+u=\frac{GM}{h^2},
$$

whose solution is

$$
\boxed{r=\frac{l}{1+e\cos\theta},
\qquad l=\frac{h^2}{GM}}.
$$

Here $\theta$ is the [true anomaly](../../../../../true-anomaly.md) measured from periapsis and $e$ is the [orbital eccentricity](../../../../../orbital-eccentricity.md). Substitution into the energy, or evaluation at an apsis, gives

$$
\frac E\mu=-\frac{GM}{2a},
\qquad
l=a(1-e^2),
$$

and hence

$$
\boxed{E=-\frac{GM\mu}{2a}}.
$$

Immediately before the supernova the circular relative speed obeys $v^2=GM/a$. The impulsive [supernova kick in a binary star](../../../../../supernova-kick-in-a-binary-star.md) changes it to

$$
v'^2=v^2(1+2\alpha\cos\psi+\alpha^2).
$$

Applying the energy formula just after the explosion at the unchanged separation $r=a$ gives

$$
-\frac{GM'}{2a'}
=\frac12v'^2-\frac{GM'}a.
$$

Using the original circular-speed relation,

$$
\boxed{\frac{M'}{a'}
=\frac{2M'}a-\frac Ma(1+2\alpha\cos\psi+\alpha^2)}.
$$

The post-explosion system is bound exactly when $1+2\alpha\cos\psi+\alpha^2<2M'/M$. The left side ranges from $(1-\alpha)^2$ to $(1+\alpha)^2$, so every kick direction remains bound if

$$
\boxed{M'>\frac12(1+\alpha)^2M},
$$

whereas every direction unbinds the stars if

$$
\boxed{M'<\frac12(1-\alpha)^2M}.
$$

For an unbound orbit, conservation of relative specific energy at infinity gives $V^2/2=v'^2/2-GM'/a$. Therefore

$$
\boxed{V=\left[(1+2\alpha\cos\psi+\alpha^2)
-\frac{2M'}M\right]^{1/2}v}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
