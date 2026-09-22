<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\Delta_M$ be the free real-scalar [Feynman propagator](../../../../feynman-propagator.md) and $D_m(x-y)=\langle0|T\varphi(x)\varphi^\dagger(y)|0\rangle_0$ the free complex-scalar one. Expanding the interaction exponential once and applying [Wick's theorem](../../../../wick-s-theorem.md) gives the connected decay [Green's function](../../../../green-s-function-split.md)

$$
\boxed{\langle T\phi(x)\varphi(y)\varphi^\dagger(z)\rangle_c
=-ig\int d^4w\,\Delta_M(x-w)D_m(y-w)D_m(w-z)+O(g^3).}
$$

There is one allowed contraction of each external [field](../../../../field.md) with the appropriate [vertex](../../../../vertex-graph-theory.md) field, so no factorial remains. Fourier transformation gives the momentum-conserving delta factor times $(-ig)\widetilde\Delta_M(p)\widetilde D_m(q_1)\widetilde D_m(q_2)$, and [amputation of external propagators](../../../../amputation-of-external-propagators.md) gives the decay vertex $-ig$. An on-shell physical decay additionally requires $M>2m$.

If one literally asks for the full three-point [correlation function](../../../../correlation-function.md) without a connected restriction or a tadpole condition, it also contains

$$
-ig\int d^4w\,\Delta_M(x-w)D_m(0)D_m(y-z),
$$

the product of the induced heavy-field one-point function and the free light-field two-point function. This disconnected [tadpole diagram](../../../../tadpole-diagram.md) does not describe a three-particle decay and drops out of its connected amputated amplitude.

For two equally charged daughters the corresponding [Green's function](../../../../green-s-function-split.md) vanishes to every perturbative order:

$$
\boxed{\langle T\phi(x)\varphi^\dagger(y)\varphi^\dagger(z)\rangle=0.}
$$

Every interaction contains equal numbers of $\varphi$ and $\varphi^\dagger$, so the two excess conjugate fields can never be paired. Equivalently the exact global [U(1)](../../../../circle-group.md) symmetry $\varphi\mapsto e^{i\alpha}\varphi$, $\varphi^\dagger\mapsto e^{-i\alpha}\varphi^\dagger$ leaves the [vacuum](../../../../vacuum.md) and action invariant, whereas this insertion has charge $-2$. Charge conservation forbids the decay of a neutral [particle](../../../../particle-physics.md) into two particles of the same nonzero charge.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
