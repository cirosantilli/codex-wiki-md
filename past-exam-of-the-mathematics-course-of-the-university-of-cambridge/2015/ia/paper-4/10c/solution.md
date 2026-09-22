<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

The [Lorentz force](../../../../../lorentz-force.md) in the uniform [magnetic field](../../../../../magnetic-field.md) gives

$$
\dot{\mathbf L}=\mathbf r\times m\dot{\mathbf v}=q\mathbf r\times(\mathbf v\times\mathbf B)=q[(\mathbf r\cdot\mathbf B)\mathbf v-(\mathbf r\cdot\mathbf v)\mathbf B],
$$

where the last step is the [vector triple product identity](../../../../../vector-triple-product.md). Hence

$$
\frac d{dt}(\mathbf L\cdot\mathbf B)=q[(\mathbf r\cdot\mathbf B)(\mathbf v\cdot\mathbf B)-B^2(\mathbf r\cdot\mathbf v)].
$$

On the other hand, $|\mathbf r\times\mathbf B|^2=B^2r^2-(\mathbf r\cdot\mathbf B)^2$, so

$$
\frac d{dt}\left(\frac q2|\mathbf r\times\mathbf B|^2\right)=q[B^2(\mathbf r\cdot\mathbf v)- (\mathbf r\cdot\mathbf B)(\mathbf v\cdot\mathbf B)].
$$

The derivatives cancel, proving the [magnetic angular-momentum invariant](../../../../../magnetic-angular-momentum-invariant.md)

$$
\boxed{\mathbf L\cdot\mathbf B+\frac q2|\mathbf r\times\mathbf B|^2=\text{constant}.}
$$

The magnetic [Lorentz force](../../../../../lorentz-force.md) is perpendicular to velocity, so its power is zero:

$$
\dot T=m\mathbf v\cdot\dot{\mathbf v}=q\mathbf v\cdot(\mathbf v\times\mathbf B)=0.
$$

Thus **the kinetic energy is constant**.

For the alternative [kinetic energy](../../../../../kinetic-energy.md) expression, work on an interval where $r>0$ so that the radial [unit vector](../../../../../unit-vector.md) $\mathbf u=\mathbf r/r$ is defined. Differentiating $\mathbf u\cdot\mathbf u=1$ once and twice gives

$$
\mathbf u\cdot\dot{\mathbf u}=0,\qquad \mathbf u\cdot\ddot{\mathbf u}=-|\dot{\mathbf u}|^2.
$$

Since $\mathbf v=\dot r\mathbf u+r\dot{\mathbf u}$, it follows that $\mathbf u\cdot\mathbf v=\dot r$ and $v^2=\dot r^2+r^2|\dot{\mathbf u}|^2$. Therefore the [unit-direction kinetic-energy identity](../../../../../unit-direction-kinetic-energy-identity.md) is

$$
\boxed{T=\frac m2\mathbf u\cdot\left[(\mathbf u\cdot\mathbf v)\mathbf v-r^2\ddot{\mathbf u}\right]=\frac m2v^2.}
$$

This identity holds for any twice differentiable trajectory away from the origin, not only for motion in a [magnetic field](../../../../../magnetic-field.md).

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
