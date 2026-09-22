<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each lower index contributes a minus connection term to the [covariant derivative](../../../../covariant-derivative.md) of the [metric tensor](../../../../metric-tensor.md):

$$
\nabla_\lambda g_{\mu\nu}
=\partial_\lambda g_{\mu\nu}
-\Gamma^\rho_{\mu\lambda}g_{\rho\nu}
-\Gamma^\rho_{\nu\lambda}g_{\mu\rho}.
$$

Substitute the [Christoffel symbols](../../../../christoffel-symbol.md) of the [Levi-Civita connection](../../../../levi-civita-connection.md) and use the [inverse metric](../../../../inverse-metric.md) identity $g_{\rho\nu}g^{\rho\sigma}=\delta^\sigma_\nu$:

$$
\begin{aligned}
g_{\rho\nu}\Gamma^\rho_{\mu\lambda}
&=\tfrac12(\partial_\mu g_{\nu\lambda}
+\partial_\lambda g_{\nu\mu}-\partial_\nu g_{\mu\lambda}),\\
g_{\mu\rho}\Gamma^\rho_{\nu\lambda}
&=\tfrac12(\partial_\nu g_{\mu\lambda}
+\partial_\lambda g_{\mu\nu}-\partial_\mu g_{\nu\lambda}).
\end{aligned}
$$

Adding cancels the first and third terms and leaves exactly $\partial_\lambda g_{\mu\nu}$. Hence

$$
\boxed{\nabla_\lambda g_{\mu\nu}=0.}
$$

This is [metric compatibility](../../../../metric-compatibility.md): the [Levi-Civita connection](../../../../levi-civita-connection.md) preserves the [inner product](../../../../inner-product-split.md) under [parallel transport](../../../../parallel-transport.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
