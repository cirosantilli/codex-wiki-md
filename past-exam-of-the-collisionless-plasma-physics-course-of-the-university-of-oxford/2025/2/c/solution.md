<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use positive real local [wavenumbers](../../../../wavenumber.md)

$$
k_1(x)=\frac{\omega_{pe0}}{cL}\sqrt{x^2-x_T^2}\quad(x<a),\qquad
k_2(x)=\kappa(x)=\frac{\omega_{pe0}}{cL}\sqrt{x_T^2-x^2}\quad(a<x<b),\qquad
k_3(x)=\frac{\omega_{pe0}}{cL}\sqrt{x^2-x_T^2}\quad(x>b),
$$

within $|x|\le L$. If the exterior is [vacuum](../../../../vacuum.md), continue $k_1,k_3$ as $\omega/c$ outside the column. Define the positive [phase integrals](../../../../phase-integral.md) and barrier integral

$$
\Phi(x)=\int_x^a k_1(s)\,ds,\qquad
I(x)=\int_a^x\kappa(s)\,ds,\qquad
\Psi(x)=\int_b^x k_3(s)\,ds.
$$

The three [WKB approximations](../../../../wkb-approximation.md), with the common $e^{-i\omega t}$ suppressed, are

$$
\boxed{\begin{aligned}
E_{\rm I}&=\frac{A_{\rm in}e^{-i(\Phi-\pi/4)}+A_{\rm r}e^{i(\Phi-\pi/4)}}{\sqrt{k_1}},\\
E_{\rm II}&=\frac{D e^{-I}+G e^{I}}{\sqrt\kappa},\\
E_{\rm III}&=\frac{A_{\rm t}e^{i(\Psi-\pi/4)}+A_{\rm back}e^{-i(\Psi-\pi/4)}}{\sqrt{k_3}}.
\end{aligned}}
$$

The [flux-normalized WKB amplitudes](../../../../flux-normalized-wkb-amplitude.md) make squared travelling-wave coefficients proportional to directed [Poynting flux](../../../../poynting-flux.md). Since $\Phi'=-k_1$ and $\Psi'=k_3$, $A_{\rm in}$ and $A_{\rm t}$ travel to the right, while $A_{\rm r}$ and $A_{\rm back}$ travel to the left. The constants $\pi/4$ are a convenient [Airy turning-point connection formula](../../../../airy-turning-point-connection-formula.md) convention.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the collisionless plasma physics course of the University of Oxford](../../../split.md)
5. [Collisionless plasma physics course of the University of Oxford](../../../../collisionless-plasma-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
