<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose $D_\mu=\partial_\mu-igA_\mu^at^a$ on the [Dirac field](../../../../dirac-field.md), $t^a=\sigma^a/2$ in the [fundamental representation](../../../../fundamental-representation.md) of [SU(2)](../../../../su-2-group.md), and $[t^a,t^b]=i\epsilon^{abc}t^c$. Define the [gauge field strength](../../../../gauge-field-strength.md) and the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md) [gauge covariant derivative](../../../../gauge-covariant-derivative.md) by

$$
F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a
+g\epsilon^{abc}A_\mu^bA_\nu^c,\qquad
(D_\mu c)^a=\partial_\mu c^a+g\epsilon^{abc}A_\mu^bc^c.
$$

The required [gauge-fixed Yang-Mills Lagrangian in a covariant gauge](../../../../gauge-fixed-yang-mills-lagrangian-in-a-covariant-gauge.md), including the matter term, is

$$
\boxed{\mathcal L=-\frac14F_{\mu\nu}^aF^{a\mu\nu}
+\bar\psi(i\gamma^\mu D_\mu-m)\psi
-\frac1{2\xi}(\partial^\mu A_\mu^a)^2
-\bar c^a\partial^\mu(D_\mu c)^a.}
$$

Here $c^a$ and $\bar c^a$ are independent [Grassmann fields](../../../../grassmann-field.md) in the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md): the [Faddeev-Popov ghost fields](../../../../faddeev-popov-ghost.md) and [antighost fields](../../../../faddeev-popov-antighost-field.md). Under an infinitesimal [gauge transformation](../../../../gauge-transformation.md), $\delta A_\mu^a=(D_\mu\omega)^a$; hence the [Lorenz gauge](../../../../lorenz-gauge-condition.md) function $G^a=\partial^\mu A_\mu^a$ varies by $\partial^\mu D_\mu^{ab}\omega^b$. Its [Faddeev-Popov determinant](../../../../faddeev-popov-determinant.md) is represented by the ghost term, with an irrelevant field-independent determinant sign absorbed into normalization. [Integration by parts](../../../../integration-by-parts.md) gives $\mathcal L_{\rm gh}=(\partial^\mu\bar c^a)(D_\mu c)^a$, explicitly showing the [ghost-gluon vertex](../../../../ghost-gluon-vertex.md).

There is no scalar vacuum expectation value here, so [R-xi gauge](../../../../r-xi-gauge.md) reduces to the linear [covariant gauge](../../../../covariant-gauge.md) displayed above, with no [Goldstone boson](../../../../goldstone-boson.md) term. At $\xi=1$ the [Feynman gauge](../../../../feynman-gauge.md) [gauge boson](../../../../gauge-boson.md) [propagator](../../../../propagator.md) is $-i\delta^{ab}g_{\mu\nu}/(k^2+i0)$. With Fourier convention $e^{-ikx}$ and all three boson [four-momenta](../../../../four-momentum.md) incoming, this choice gives exactly the source's $+g\epsilon^{abc}$ three-boson [Feynman rule](../../../../feynman-rule.md), and the matter [interaction vertex](../../../../interaction-vertex.md) is $+ig\gamma^\mu t^a$. The sign of $D_\mu$ has been explicitly chosen here; the QED convention in question 2 instead has vertex $-ie\gamma^\mu$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
