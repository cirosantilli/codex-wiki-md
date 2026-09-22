<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [chain rule](../../../../../../chain-rule.md) and

$$
\theta_x=\Theta_X=k,
\qquad
\theta_t=\Theta_T=-\omega,
\qquad
X_x=T_t=\varepsilon
$$

give

$$
\phi_x=k\Phi_\theta+\varepsilon\Phi_X,
\qquad
\phi_t=-\omega\Phi_\theta+\varepsilon\Phi_T.
$$

Applying the same rule to $L_1$ and $L_2$ in the [Euler-Lagrange field equation](../../../../../../euler-lagrange-field-equation.md) yields the exact modulated equation

$$
\boxed{
k(L_1)_\theta+\varepsilon(L_1)_X
-\omega(L_2)_\theta+\varepsilon(L_2)_T-L_3=0.}
$$

Multiply this equation by $\Phi_\theta$. Since $k$ and $\omega$ are independent of the fast phase,

$$
L_\theta
=L_1(k\Phi_{\theta\theta}+\varepsilon\Phi_{X\theta})
+L_2(-\omega\Phi_{\theta\theta}+\varepsilon\Phi_{T\theta})
+L_3\Phi_\theta.
$$

The [product rule](../../../../../../product-rule.md) then rearranges the field equation into the exact [modulated-wave first integral](../../../../../../modulated-wave-first-integral.md)

$$
\boxed{
\partial_\theta\left[(kL_1-\omega L_2)\Phi_\theta-L\right]
+\varepsilon\partial_X(\Phi_\theta L_1)
+\varepsilon\partial_T(\Phi_\theta L_2)=0.}
$$

Average this identity over one $2\pi$ period in $\theta$. [Periodicity](../../../../../../periodic-function.md) kills the first term, while differentiation of the [averaged Lagrangian](../../../../../../averaged-lagrangian.md) gives

$$
\frac{\partial\overline L}{\partial k}
=\left\langle\Phi_\theta L_1\right\rangle,
\qquad
\frac{\partial\overline L}{\partial\omega}
=-\left\langle\Phi_\theta L_2\right\rangle.
$$

Consequently

$$
\boxed{
\partial_X\frac{\partial\overline L}{\partial k}
-\partial_T\frac{\partial\overline L}{\partial\omega}=0.}
$$

The same two equations follow directly from the modulated [variational principle](../../../../../../principle-of-stationary-action.md). Varying $\Phi$ gives

$$
\partial_\theta(kL_1-\omega L_2)
+\varepsilon\partial_XL_1
+\varepsilon\partial_TL_2-L_3=0,
$$

which is the exact field equation above. For a variation of $Θ$, use $\delta k=\partial_X\delta\Theta$ and $\delta\omega=-\partial_T\delta\Theta$. [Integration by parts](../../../../../../integration-by-parts.md) in $X$ and $T$ gives the averaged equation. Thus variation with respect to the periodic profile reproduces the local wave equation, whereas variation with respect to its slow phase gives the [Whitham modulation equation](../../../../../../whitham-modulation-equation.md) for wave action.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
