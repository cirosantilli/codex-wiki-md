<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At $x^k$, choose $a=f(x^k)$, $g=\nabla f(x^k)$, $H=\nabla^2f(x^k)$, and the current radius $\Delta=\Delta_k>0$. A bounded [symmetric matrix](../../../../../symmetric-matrix.md) approximation to the [Hessian matrix](../../../../../hessian-matrix.md) can also be used. Stop if the [gradient](../../../../../gradient.md) is sufficiently small; otherwise approximately solve the [trust-region subproblem](../../../../../trust-region-subproblem.md) to obtain $s_k$ with $\|s_k\|\leq\Delta_k$ and at least a fixed [fraction of Cauchy decrease](../../../../../fraction-of-cauchy-decrease.md). Its predicted decrease is then positive, so calculate the [trust-region acceptance ratio](../../../../../trust-region-acceptance-ratio.md)

$$
\rho_k=\frac{f(x^k)-f(x^k+s_k)}{m_k(0)-m_k(s_k)}.
$$

Fix $0<\eta_1<\eta_2<1$, $0<\gamma_d<1<\gamma_u$, and a maximum radius $\Delta_{\max}$. One valid update is:
- If $\rho_k<\eta_1$, reject the trial: $x^{k+1}=x^k$ and $\Delta_{k+1}=\gamma_d\Delta_k$.
- Otherwise accept $x^{k+1}=x^k+s_k$. If additionally $\rho_k>\eta_2$ and the step reaches the boundary, enlarge the radius to $\min\{\gamma_u\Delta_k,\Delta_{\max}\}$; otherwise keep it unchanged.

The [trust region](../../../../../trust-region.md) controls the reliability of the model; the ratio decides whether that reliability was borne out by the actual [objective function](../../../../../objective-function.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Continuous optimisation course of the University of Oxford](../../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
