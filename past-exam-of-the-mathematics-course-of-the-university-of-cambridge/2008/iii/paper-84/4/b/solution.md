<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\xi=x/\delta_0$ and $n=2p-q$. The [eddy viscosity](../../../../../../eddy-viscosity.md) is $\nu_T=C_\mu\sqrt{k_0}\delta_0\xi^n$, since $\delta_0=k_0^{3/2}/\epsilon_0$. In the energy equation, advection scales as $\xi^{p-1}$, turbulent diffusion as $\xi^{n+p-2}$, and destruction as $\xi^q$. A leading advection–diffusion [K-epsilon turbulence front](../../../../../../k-epsilon-turbulence-front.md) requires $n=1$, hence

$$
\boxed{q=2p-1.}
$$

Comparing the leading coefficients then gives $U_0=C_\mu p\sqrt{k_0}/\sigma_k$. Similarly, the leading coefficients of the dissipation equation give $U_0=C_\mu q\sqrt{k_0}/\sigma_\epsilon$. Their equality implies $q=\sigma p$, where $\sigma=\sigma_\epsilon/\sigma_k$. Combining this with $q=2p-1$ yields

$$
\boxed{p=\frac1{2-\sigma},\qquad q=\frac{\sigma}{2-\sigma},
\qquad U_0=\frac{C_\mu(2p-1)\sqrt{k_0}}{\sigma_\epsilon}.}
$$

The assumed positive exponents require $0<\sigma<2$. Under these values, the omitted destruction terms are indeed higher order, as checked in part (d), so the leading balance is not circular.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
