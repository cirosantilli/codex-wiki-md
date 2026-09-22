<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work consistently to first order in the [metric perturbation](../../../../linearized-gravity-split.md), with $\partial_\mu\xi^\nu$ of the same small order. Under the passive change $x'^\mu=x^\mu+\xi^\mu(x)$,

$$
\frac{\partial x^\alpha}{\partial x'^\mu}
=\delta^\alpha_\mu-\partial_\mu\xi^\alpha+O(h^2).
$$

Applying this to the full [metric tensor](../../../../metric-tensor.md) and writing $g'_{\mu\nu}=\eta_{\mu\nu}+h'_{\mu\nu}$ with the same fixed numerical [Minkowski metric](../../../../minkowski-metric.md) gives

$$
\boxed{
h'_{\mu\nu}(x')=h_{\mu\nu}(x)
-\partial_\mu\xi_\nu-\partial_\nu\xi_\mu+O(h^2).
}
$$

Indices on $\xi$ are lowered with $\eta$. This is the gauge transformation of the perturbation relative to a fixed background. If the background were transformed as a tensor as well, the difference of those two fully transformed metrics would instead obey the homogeneous tensor transformation law. The inhomogeneous terms arise from retaining the fixed-background identification used in [linearized gravity](../../../../linearized-gravity-split.md).

The trace changes by $h'=h-2\partial_\alpha\xi^\alpha$, so the [trace-reversed metric perturbation](../../../../trace-reversed-metric-perturbation.md) changes as

$$
\bar h'_{\mu\nu}
=\bar h_{\mu\nu}
-\partial_\mu\xi_\nu-\partial_\nu\xi_\mu
+\eta_{\mu\nu}\partial_\alpha\xi^\alpha.
$$

Let $F_\nu=\partial^\mu\bar h_{\mu\nu}$. Commuting [partial derivatives](../../../../partial-derivative.md) gives

$$
\partial^\mu\bar h'_{\mu\nu}
=F_\nu-\Box\xi_\nu,\qquad
\Box=\eta^{\alpha\beta}\partial_\alpha\partial_\beta.
$$

Thus choose a solution of the inhomogeneous [wave equation](../../../../wave-equation-split.md)

$$
\boxed{\Box\xi_\nu=F_\nu.}
$$

Such a solution exists locally with suitable initial data, and can be selected with appropriate wave-equation [boundary conditions](../../../../boundary-condition.md). This imposes the [Lorenz gauge in linearized gravity](../../../../lorenz-gauge-in-linearized-gravity.md), $\partial^\mu\bar h'_{\mu\nu}=0$. All the divergence terms in the supplied vacuum equation then vanish, leaving

$$
\boxed{\Box\bar h'_{\mu\nu}=0.}
$$

The remaining freedom $\Box\xi_\nu=0$ is the [residual gauge symmetry of linearized gravity](../../../../residual-gauge-symmetry-of-linearized-gravity.md).

Using the old coordinates in these derivatives is consistent at the retained order. Indeed

$$
\partial'_\mu
=\partial_\mu-(\partial_\mu\xi^\alpha)\partial_\alpha+O(h^2).
$$

Acting on a first-order perturbation, the correction is a product of two first-order quantities and is discarded. Similarly replacing the argument $x'$ by $x$ changes $h'$ by $O(h^2)$ under the same perturbative ordering. This does not assert an exact equality of the two coordinate differential operators; it is the linear approximation about the fixed flat background.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
