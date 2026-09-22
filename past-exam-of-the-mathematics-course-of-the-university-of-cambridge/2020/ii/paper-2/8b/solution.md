<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

If $\mathbf r$ is measured in the rotating frame, its inertial velocity is $\dot{\mathbf r}+\boldsymbol\omega\times\mathbf r$. The masses producing the gravitational field are stationary in this frame, so their [potential energy](../../../../../potential-energy.md) is a time-independent function $V(\mathbf r)$. Thus kinetic minus potential energy gives the stated [Lagrangian](../../../../../lagrangian.md)

$$
L=\frac m2(\dot{\mathbf r}+\boldsymbol\omega\times\mathbf r)^2-V(\mathbf r).
$$

Put $\mathbf v=\dot{\mathbf r}+\boldsymbol\omega\times\mathbf r$. Then

$$
\frac{\partial L}{\partial\dot{\mathbf r}}=m\mathbf v,
\qquad
\frac{\partial L}{\partial\mathbf r}=-m\boldsymbol\omega\times\mathbf v-\nabla V.
$$

Substitution in the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) yields

$$
\boxed{m\left(\ddot{\mathbf r}+2\boldsymbol\omega\times\dot{\mathbf r}
+\dot{\boldsymbol\omega}\times\mathbf r
+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r)\right)
=-\nabla V}.
$$

The extra terms are the [Coriolis acceleration](../../../../../coriolis-acceleration.md), [Euler acceleration](../../../../../euler-acceleration.md), and [centrifugal acceleration](../../../../../centrifugal-acceleration.md) of a [rotating reference frame](../../../../../rotating-reference-frame.md).

The [canonical momentum](../../../../../canonical-momentum.md) and [Hamiltonian](../../../../../hamiltonian.md) are

$$
\boxed{\mathbf p=m(\dot{\mathbf r}+\boldsymbol\omega\times\mathbf r)},
$$



$$
\boxed{H(\mathbf r,\mathbf p,t)
=\frac{\mathbf p^2}{2m}
-\boldsymbol\omega(t)\mathbin\cdot(\mathbf r\times\mathbf p)
+V(\mathbf r)}.
$$

Accordingly, [Hamilton's equations](../../../../../hamilton-s-equations.md) are

$$
\boxed{\dot{\mathbf r}=\frac{\mathbf p}{m}-\boldsymbol\omega\times\mathbf r,
\qquad
\dot{\mathbf p}=-\boldsymbol\omega\times\mathbf p-\nabla V}.
$$

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
