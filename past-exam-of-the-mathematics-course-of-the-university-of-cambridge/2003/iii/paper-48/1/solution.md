<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) as $\widehat H=\widehat p^2/(2m)+V(\widehat q)$, with $[\widehat q,\widehat p]=i$, and define the [quantum-mechanical propagator](../../../../../quantum-mechanical-propagator.md) by $U(\beta,\alpha;T)=\langle\beta|e^{-iT\widehat H}|\alpha\rangle$. Use $N$ intervals of length $\varepsilon=T/N$, endpoint coordinates $q_0=\alpha,q_N=\beta$, and the [Trotter product formula](../../../../../lie-product-formula.md). Inserting the completeness relations of the [position eigenstates](../../../../../position-eigenstate.md) between the short-time factors gives

$$
U=\lim_{N\to\infty}\int\prod_{j=1}^{N-1}dq_j\prod_{j=1}^N\langle q_j|e^{-i\varepsilon\widehat p^2/(2m)}e^{-i\varepsilon V(\widehat q)}|q_{j-1}\rangle.
$$

Normalize [momentum eigenstates](../../../../../momentum-eigenstate.md) by $\langle q|p\rangle=e^{ipq}/\sqrt{2\pi}$. The [Gaussian integral](../../../../../gaussian-integral.md) over the intermediate [momentum](../../../../../momentum.md) is

$$
\int\frac{dp}{2\pi}\exp\left(ip(q_j-q_{j-1})-\frac{i\varepsilon p^2}{2m}\right)=\left(\frac{m}{2\pi i\varepsilon}\right)^{1/2}\exp\left(\frac{im(q_j-q_{j-1})^2}{2\varepsilon}\right).
$$

The square-root branch is fixed by continuation from $\operatorname{Im}\varepsilon<0$. Consequently the precise [time-sliced configuration-space path integral](../../../../../time-sliced-configuration-space-path-integral.md) is

$$
\boxed{U=\lim_{N\to\infty}\left(\frac{m}{2\pi i\varepsilon}\right)^{N/2}\int_{\mathbb R^{N-1}}\prod_{j=1}^{N-1}dq_j\exp\left[i\sum_{j=1}^N\left\{\frac{m(q_j-q_{j-1})^2}{2\varepsilon}-\varepsilon V(q_{j-1})\right\}\right].}
$$

This formula defines the notation $\int\mathcal Dq\,e^{iS[q]}$; it is not an unnormalized infinite product of ordinary integrals. For real time take the boundary value from $T-i\delta$, $\delta>0$, or the corresponding oscillatory-distribution limit. For a self-adjoint, bounded-below [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) under the usual product-formula hypotheses, the operator limit supplies the definition even where the coordinate kernel is a distribution. The discrete exponent approaches the [action](../../../../../action.md) with [kinetic term](../../../../../kinetic-term.md) $m\dot q^2/2$, and the prefactor is part of the [functional measure](../../../../../functional-measure.md). A different consistent slicing gives the same kernel for this separated kinetic-plus-potential Hamiltonian.

For the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md), expand the [action](../../../../../action.md) about a [classical path](../../../../../classical-path.md) $x$, writing $q=x+\xi$ with homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) on $\xi$. The only mixed term is

$$
m\int_0^T(\dot x\dot\xi-\omega^2x\xi)\,dt=m[\dot x\xi]_0^T-m\int_0^T(\ddot x+\omega^2x)\xi\,dt=0.
$$

The boundary term vanishes and the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) sets the remaining integrand to zero. Thus $S[x+\xi]=S[x]+S[\xi]$ exactly, rather than only to quadratic approximation. Translation of each integrated coordinate has unit [Jacobian determinant](../../../../../jacobian-determinant.md); in the continuum measure convention of the question this is $\mathcal Dq=\mathcal D\xi$. The [classical-path factorization of a quadratic path integral](../../../../../classical-path-factorization-of-a-quadratic-path-integral.md) follows:

$$
\boxed{U(\beta,\alpha;T)=e^{iS[x]}F(T),\qquad F(T)=\int_{\xi(0)=\xi(T)=0}\mathcal D\xi\,e^{iS[\xi]}.}
$$

The fluctuation [action](../../../../../action.md), measure and boundary values depend on $T,m,\omega$ but not on $\alpha,\beta$. For real $T$ with $\sin\omega T\ne0$ the boundary-value [classical path](../../../../../classical-path.md) exists uniquely. At the conjugate times $\omega T=k\pi$, generic endpoints admit no such path and the kernel is a delta distribution; the formula is interpreted by the same regulated boundary limit, not as an ordinary finite prefactor times a nonexistent classical solution.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
