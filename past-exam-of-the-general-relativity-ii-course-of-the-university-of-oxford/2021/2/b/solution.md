<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the active sign convention for the [linearized coordinate gauge transformation](../../../../linearized-coordinate-gauge-transformation.md), $h_{\mu\nu}\mapsto h_{\mu\nu}+\partial_\mu\xi_\nu+\partial_\nu\xi_\mu$. The paper's prescribed generator has precisely this sign; using the passive convention would require its negative. Direct [partial differentiation](../../../../partial-derivative.md) gives

$$
\partial_\nu\xi_\mu=\frac14\left[
\tilde h''_{\kappa\sigma}x^\kappa x^\sigma n_\mu n_\nu
+2\tilde h'_{\nu\kappa}x^\kappa n_\mu
-2\tilde h'_{\mu\kappa}x^\kappa n_\nu-2\tilde h_{\mu\nu}\right].
$$

The middle terms cancel when the indices are symmetrized. Therefore

$$
\partial_\mu\xi_\nu+\partial_\nu\xi_\mu
=\frac12\tilde h''_{\kappa\sigma}x^\kappa x^\sigma n_\mu n_\nu-\tilde h_{\mu\nu},
\qquad
\boxed{\hat h_{\mu\nu}=\phi n_\mu n_\nu,\quad
\phi=\frac12\tilde h''_{\kappa\sigma}x^\kappa x^\sigma.}
$$

To test both equations (3), put $H(u)=\tilde h(u)=\eta^{\kappa\sigma}\tilde h_{\kappa\sigma}(u)$, the [trace](../../../../matrix-trace.md) of the original [metric perturbation](../../../../linearized-gravity-split.md). Since $n$ is a [null vector](../../../../null-vector.md), $\hat h=0$ and its [trace-reversed metric perturbation](../../../../trace-reversed-metric-perturbation.md) equals $\hat h$. Differentiating the result of part (a) gives

$$
n\cdot\partial\phi=n^\kappa\tilde h''_{\kappa\sigma}x^\sigma
=\frac12uH'',
\qquad
\Box\phi=H''+2n^\kappa\tilde h'''_{\kappa\sigma}x^\sigma
=H''+uH'''.
$$

In the second identity, the term with $n^2$ is zero. Thus

$$
\boxed{\partial^\mu\overline{\hat h}_{\mu\nu}=\frac12uH''n_\nu,\qquad
\Box\hat h_{\mu\nu}=(H''+uH''')n_\mu n_\nu.}
$$

**In general $\hat h$ does not satisfy (3).** On an open interval of $u$, both equations hold exactly when $H''=0$ there: the first equation forces this for $u\ne0$, and smoothness gives it at $u=0$ as well. A [linearized coordinate gauge transformation](../../../../linearized-coordinate-gauge-transformation.md) preserves the [linearized vacuum Einstein equations](../../../../linearized-vacuum-einstein-equations.md), but only a [residual gauge symmetry of linearized gravity](../../../../residual-gauge-symmetry-of-linearized-gravity.md) preserves the imposed [Lorenz gauge in linearized gravity](../../../../lorenz-gauge-in-linearized-gravity.md).

For an explicit failure, use the [null coordinates](../../../../null-coordinate.md) of part (c) and take only $\tilde h_{uv}=\tilde h_{vu}=u^2/4$ nonzero. Then $H=u^2$, the original field obeys (3), but $\phi=uv/2$ gives $\partial^\mu\overline{\hat h}_{\mu u}=u$ and $\Box\hat h_{uu}=2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
