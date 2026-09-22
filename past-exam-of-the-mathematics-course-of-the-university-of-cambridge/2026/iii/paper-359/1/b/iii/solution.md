<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take the $L^2$ inner product of the temperature equation with $\theta_m$. The spectral projection disappears against $\theta_m\in\widetilde H_m$, and part (a)(iii) cancels transport. Thus

$$
\frac12\frac d{dt}\|\theta_m\|_2^2
+\kappa\|\nabla\theta_m\|_2^2
=\beta(u_m\mathbin\cdot e_3,\theta_m).
$$

The periodic [Poincaré inequality](../../../../../../../poincare-inequality.md), part (i), and the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) imply

$$
|(u_m\mathbin\cdot e_3,\theta_m)|
\leq |u_m|\|\theta_m\|_2
\leq C|Au_m|\|\theta_m\|_2
\leq C\frac{\alpha}{\nu}\|\theta_m\|_2^2.
$$

The [Gronwall inequality](../../../../../../../gronwall-inequality.md) therefore gives, for $0\leq t\leq T$,

$$
\|\theta_m(t)\|_2^2
\leq e^{C\alpha\beta T/\nu}\|\theta_0\|_2^2.
$$

This defines a bound $K_0(T)$ independent of $m$, and part (i) then gives

$$
\|Au_m\|_{L^\infty(0,T;H)}
\leq\frac{\alpha}{\nu}K_0(T)=:K_2(T).
$$

Integrating the energy identity and using the same bound on its right-hand side gives

$$
\|\theta_m\|_{L^2(0,T;H^1_{\rm per})}\leq K_1(T).
$$

It remains to estimate the time derivative. For $\varphi\in H^1_{\rm per}$, the Fourier projection $\Pi_m$ is a contraction in $H^1$, and the skew identity from part (a) gives

$$
|\langle\Pi_m((u_m\mathbin\cdot\nabla)\theta_m),\varphi\rangle|
=\left|\int_\Omega(u_m\mathbin\cdot\nabla\Pi_m\varphi)\theta_m\,dx\right|
\leq\|u_m\|_\infty\|\theta_m\|_2\|\varphi\|_{H^1}.
$$

The [sobolev embedding theorem](../../../../../../../sobolev-embedding-theorem.md) and the [periodic elliptic estimate](../../../../../../../periodic-elliptic-estimate.md) for the Stokes operator bound $\|u_m\|_\infty$ by $C|Au_m|$. Moreover,

$$
\|\Delta\theta_m\|_{H^{-1}}\leq\|\nabla\theta_m\|_2,
\qquad
\|\Pi_m(u_m\mathbin\cdot e_3)\|_{H^{-1}}\leq C|u_m|.
$$

The already obtained bounds therefore imply

$$
\boxed{\left\|\frac{d\theta_m}{dt}\right\|_{L^2(0,T;H^{-1}_{\rm per})}\leq K'_0(T)}
$$

with $K'_0(T)$ independent of $m$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
