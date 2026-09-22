<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the [center of mass](../../../../../../center-of-mass.md) frame, put the two positions at $(0,0,z(t))$ and $(0,0,-z(t))$, with $z>0$ during infall. Their separation is $2z$, so [Newtonian gravity](../../../../../../gravitational-acceleration.md) gives

$$
\boxed{\ddot z=-\frac{m}{4z^2},\qquad z(0)=z_0,\quad\dot z(0)=0.}
$$

Multiplying by $\dot z$ and integrating gives

$$
\frac12\dot z^2=\frac m4\left(\frac1z-\frac1{z_0}\right),\qquad
\boxed{\dot z=-\sqrt{\frac m2}\sqrt{\frac1z-\frac1{z_0}}.}
$$

The negative square root is essential for the falling branch. All [second mass moment tensor](../../../../../../second-mass-moment-tensor.md) components except $I_{zz}=2mz^2$ vanish. Differentiating three times,

$$
\dddot I_{zz}=4m(3\dot z\ddot z+z\dddot z),\qquad
\dddot z=\frac{m\dot z}{2z^3}.
$$

Substitution yields $\dddot I_{zz}=-m^2\dot z/z^2$, hence

$$
\boxed{\dddot I_{zz}=\frac{m^2}{z^2}\sqrt{\frac m2}\sqrt{\frac1z-\frac1{z_0}},}
$$

with every other component of $\dddot I_{ij}$ zero. **The distance entering each acceleration is $2z$**, which accounts for the factor one quarter in the equation of motion.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
