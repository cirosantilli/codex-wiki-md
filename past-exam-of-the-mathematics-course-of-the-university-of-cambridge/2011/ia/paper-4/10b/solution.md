<h1 id="10b/solution">Solution</h1>

↑ **Parent:** [10B](../10b.md)

Apply the [rotating-frame derivative formula](../../../../../rotating-frame-derivative-formula.md) first to position and then to its inertial [velocity](../../../../../velocity.md):

$$
\left(\frac{d\mathbf r}{dt}\right)_I=\dot{\mathbf r}+\boldsymbol\omega\times\mathbf r,
$$



$$
\left(\frac{d^2\mathbf r}{dt^2}\right)_I
=\ddot{\mathbf r}+2\boldsymbol\omega\times\dot{\mathbf r}
+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r).
$$

The angular velocity is constant, so there is no term involving $\dot{\boldsymbol\omega}$. By [Newton's second law](../../../../../newton-s-second-law.md) in the [inertial frame](../../../../../inertial-frame.md), the inertial acceleration is $\mathbf F/m$. Rearrangement gives the [equation of motion in a rotating frame](../../../../../equation-of-motion-in-a-rotating-frame.md):

$$
\boxed{m\ddot{\mathbf r}=\mathbf F-2m\boldsymbol\omega\times\dot{\mathbf r}
-m\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r).}
$$

The two additional accelerations are the [Coriolis acceleration](../../../../../coriolis-acceleration.md) and [centrifugal acceleration](../../../../../centrifugal-acceleration.md).

## ↑ Ancestors (10)

1. [10B](../10b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
