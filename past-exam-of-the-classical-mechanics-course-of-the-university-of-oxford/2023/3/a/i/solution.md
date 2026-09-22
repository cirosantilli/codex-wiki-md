<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define the [canonical momenta](../../../../../canonical-momentum.md) by

$$
\boxed{p_i=\frac{\partial L}{\partial\dot q_i}(\mathbf q,\dot{\mathbf q},t),\qquad i=1,\ldots,n.}
$$

To obtain an ordinary unconstrained [Hamiltonian](../../../../../hamiltonian.md), assume a [regular Lagrangian](../../../../../regular-lagrangian.md): the velocity [Hessian matrix](../../../../../hessian-matrix.md) $\bigl(\partial^2L/\partial\dot q_i\partial\dot q_j\bigr)$ is invertible. The [inverse function theorem](../../../../../inverse-function-theorem.md) then lets us solve locally for $\dot{\mathbf q}=\mathbf v(\mathbf q,\mathbf p,t)$. The [phase space](../../../../../phase-space.md) is the [cotangent bundle](../../../../../cotangent-bundle.md) $T^*\mathcal Q$, with local [canonical coordinates](../../../../../canonical-variables.md) $(\mathbf q,\mathbf p)$ and dimension $2n$. The [Legendre transform in mechanics](../../../../../legendre-transform-in-mechanics.md) defines

$$
\boxed{H(\mathbf q,\mathbf p,t)=\sum_{i=1}^np_iv_i(\mathbf q,\mathbf p,t)
-L\bigl(\mathbf q,\mathbf v(\mathbf q,\mathbf p,t),t\bigr).}
$$

The velocities in this formula have been eliminated in favour of [phase space](../../../../../phase-space.md) variables. A [hyperregular Lagrangian](../../../../../hyperregular-lagrangian.md) makes this construction global; regularity alone guarantees it locally. [Hamilton's equations](../../../../../hamilton-s-equations.md) are

$$
\boxed{\dot q_i=\frac{\partial H}{\partial p_i},\qquad
\dot p_i=-\frac{\partial H}{\partial q_i},\qquad i=1,\ldots,n.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the classical mechanics course of the University of Oxford](../../../../split.md)
6. [Classical mechanics course of the University of Oxford](../../../../../classical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
