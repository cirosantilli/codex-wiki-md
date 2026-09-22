<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

For any [vector](../../../../../vector.md) $\mathbf a$, differentiating its components and the rotating basis gives the [rotating-frame derivative formula](../../../../../rotating-frame-derivative-formula.md)

$$
\left(\frac{d\mathbf a}{dt}\right)_S=\left(\frac{d\mathbf a}{dt}\right)_{S'}+\boldsymbol\omega\times\mathbf a.
$$

Apply it twice to the [position](../../../../../position.md) $\mathbf x$, with constant [angular velocity](../../../../../angular-velocity.md) $\boldsymbol\omega$. The inertial [acceleration](../../../../../acceleration.md) is

$$
\mathbf a_S=\ddot{\mathbf x}+2\boldsymbol\omega\times\dot{\mathbf x}+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x),
$$

where dots denote rotating-frame derivatives. [Newton's second law](../../../../../newton-s-second-law.md) therefore becomes

$$
\boxed{m\ddot{\mathbf x}=\mathbf F-2m\boldsymbol\omega\times\dot{\mathbf x}-m\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x).}
$$

The last terms are the [Coriolis force](../../../../../coriolis-force.md) and the force corresponding to [centrifugal acceleration](../../../../../centrifugal-acceleration.md).

For the [particle on a uniformly rotating inclined plane](../../../../../particle-on-a-uniformly-rotating-inclined-plane.md), choose orthonormal vectors $\mathbf e_1$ along the horizontal $\xi$ axis and $\mathbf e_2$ up the slope, and set $\mathbf e_3=\mathbf e_1\times\mathbf e_2$, the upward [normal vector](../../../../../normal-vector.md). Then $\mathbf e_z=\sin\theta\,\mathbf e_2+\cos\theta\,\mathbf e_3$ and

$$
\mathbf x=\xi\mathbf e_1+\eta\mathbf e_2,\qquad\boldsymbol\omega=\omega\mathbf e_z,\qquad\mathbf F=-mg\mathbf e_z+N\mathbf e_3.
$$

Here $N$ is the [normal reaction](../../../../../normal-force.md). The marble is modeled as the smooth sliding particle specified by the printed equations, without an additional rolling constraint. The rotating-frame [Coriolis acceleration](../../../../../coriolis-acceleration.md) and [centrifugal acceleration](../../../../../centrifugal-acceleration.md) are respectively

$$
-2\boldsymbol\omega\times\dot{\mathbf x}=2\omega\dot\eta\cos\theta\,\mathbf e_1-2\omega\dot\xi\cos\theta\,\mathbf e_2+2\omega\dot\xi\sin\theta\,\mathbf e_3,
$$



$$
-\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x)=\omega^2\xi\mathbf e_1+\omega^2\eta\cos^2\theta\,\mathbf e_2-\omega^2\eta\sin\theta\cos\theta\,\mathbf e_3.
$$

The normal rotating-frame [acceleration](../../../../../acceleration.md) is zero, so the [normal reaction](../../../../../normal-force.md) is not generally $mg\cos\theta$; it satisfies

$$
N=m\bigl(g\cos\theta-2\omega\dot\xi\sin\theta+\omega^2\eta\sin\theta\cos\theta\bigr).
$$

Projecting the same equation onto the two tangential axes gives exactly

$$
\boxed{\ddot\xi=\omega^2\xi+2\omega\dot\eta\cos\theta,\qquad\ddot\eta=\omega^2\eta\cos^2\theta-2\omega\dot\xi\cos\theta-g\sin\theta.}
$$

Multiply the equations by $\dot\xi$ and $\dot\eta$ and add. The [Coriolis force](../../../../../coriolis-force.md) terms cancel, as expected because this force does no work relative to the rotating frame. The [normal reaction](../../../../../normal-force.md) also does no work along the plane. The conserved quantity is **rotating-frame [kinetic energy](../../../../../kinetic-energy.md) plus gravitational and [centrifugal potential](../../../../../centrifugal-potential.md) energy**:

$$
\boxed{E'=\frac m2(\dot\xi^2+\dot\eta^2)+mg\eta\sin\theta-\frac{m\omega^2}{2}(\xi^2+\eta^2\cos^2\theta)=\text{constant}.}
$$

This need not be the conserved inertial [energy](../../../../../energy.md), since the externally driven rotating plane can exchange energy with the particle.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
