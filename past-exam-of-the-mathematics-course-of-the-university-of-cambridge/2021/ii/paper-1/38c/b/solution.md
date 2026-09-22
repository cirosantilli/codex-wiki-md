<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write

$$
H_{\alpha\beta}
=\partial_\alpha\partial_\beta\omega\big|_p,
\qquad
H=\eta^{\alpha\beta}H_{\alpha\beta}.
$$

The [Levi-Civita connection](../../../../../../levi-civita-connection.md) of

$$
g_{\alpha\beta}=e^{2\omega}\eta_{\alpha\beta}
$$

is

$$
\Gamma^\rho_{\alpha\beta}
=\delta^\rho_\alpha\partial_\beta\omega
+\delta^\rho_\beta\partial_\alpha\omega
-\eta_{\alpha\beta}\partial^\rho\omega.
$$

The assumed first-derivative condition makes $\Gamma^\rho_{\alpha\beta}(p)=0$. Differentiating once more gives, at $p$,

$$
\begin{aligned}
R_{\alpha\beta\gamma\delta}
=e^{2\omega}\bigl(
&\eta_{\alpha\delta}H_{\beta\gamma}
-\eta_{\alpha\gamma}H_{\beta\delta}\\
&-\eta_{\beta\delta}H_{\alpha\gamma}
+\eta_{\beta\gamma}H_{\alpha\delta}
\bigr).
\end{aligned}
$$

Its contractions are

$$
R_{\beta\delta}
=-2H_{\beta\delta}-\eta_{\beta\delta}H,
\qquad
R=-6e^{-2\omega}H.
$$

Substitution into the defining expression for $C_{\alpha\beta\gamma\delta}$ cancels every Hessian term, leaving

$$
\boxed{C_{\alpha\beta\gamma\delta}(p)=0}.
$$

Since $p$ was arbitrary, this is the [Weyl tensor of a conformally flat metric](../../../../../../weyl-tensor-of-a-conformally-flat-metric.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
