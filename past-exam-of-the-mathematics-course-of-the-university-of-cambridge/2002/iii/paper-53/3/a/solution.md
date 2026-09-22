<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**With its material state fixed by a prescribed deformation history, the differential pom-pom model is a simple-fluid constitutive law.** The [stress](../../../../../../stress.md) depends on the local history of a material element through its molecular stretch and orientation, without gradients of that history between neighbouring elements. A differential representation does not prevent a material from being a [simple fluid](../../../../../../simple-fluid.md).

To see the history dependence explicitly, use the component-first [velocity gradient](../../../../../../velocity-gradient.md) $K$, so the tensor evolution is $D_tA=KA+AK^T-(A-I)/\tau_1$. Let $F(t,s)$ be the relative [deformation gradient](../../../../../../deformation-gradient.md), satisfying $\partial_tF=K(t)F$ and $F(s,s)=I$. Along a material trajectory, an [integrating factor](../../../../../../integrating-factor.md) gives

$$
A(t)=e^{-(t-t_0)/\tau_1}F(t,t_0)A(t_0)F(t,t_0)^T
+\frac1{\tau_1}\int_{t_0}^t e^{-(t-s)/\tau_1}F(t,s)F(t,s)^Tds.
$$

Thus $A$ is a functional of the local deformation history and its prepared initial state. If the initial $A$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), it retains that property, so $B=A/\operatorname{tr}A$ is well defined. Given this $B(t)$, the [scalar](../../../../../../scalar.md) stretch solves $\dot\lambda=r(t)\lambda+1/\tau_2$, where $r=B:K-1/\tau_2$. Its [variation of constants](../../../../../../variation-of-parameters.md) formula again depends only on that local history:

$$
\lambda(t)=\lambda(t_0)e^{\int_{t_0}^t r(q)dq}
+\frac1{\tau_2}\int_{t_0}^t e^{\int_s^t r(q)dq}ds.
$$

The [differential pom-pom model](../../../../../../differential-pom-pom-model.md) also satisfies [material frame indifference](../../../../../../material-frame-indifference.md). Under an observer rotation, $A$ and $B$ transform as objective tensors, while $\lambda$ is a scalar. The extra skew part of the transformed [velocity gradient](../../../../../../velocity-gradient.md) has zero contraction with symmetric $B$, so the stretch equation is unchanged. The tensor evolution uses an [upper-convected derivative](../../../../../../upper-convected-derivative.md), and the final [stress](../../../../../../stress.md) transforms objectively. Initial values cannot be independently forgotten when specifying a finite-past experiment: a fully specified prepared state, such as rest, is part of the history specification.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
