<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First suppose $W[\boldsymbol\xi]>0$ for every nonzero admissible [displacement](../../../../../../displacement.md). The conserved [energy](../../../../../../energy.md) from part (b) then bounds both $T$ and $W$ by $E$. In particular,

$$
\|\dot{\boldsymbol\xi}(t)\|_\rho^2\leq2E,\qquad 2W[\boldsymbol\xi(t)]\leq2E,
$$

where $\|\boldsymbol\xi\|_\rho^2=\langle\boldsymbol\xi,\boldsymbol\xi\rangle$. The positive quadratic form $\|\dot{\boldsymbol\xi}\|_\rho^2+2W[\boldsymbol\xi]$ defines the perturbation [energy](../../../../../../energy.md) norm and is conserved. Small perturbations in this norm remain small, proving energetic linear stability. Also $\|\boldsymbol\xi(t)\|_\rho\leq\|\boldsymbol\xi(0)\|_\rho+\sqrt{2E}\,t$, excluding exponential [displacement](../../../../../../displacement.md) growth. For any admissible [normal mode](../../../../../../normal-mode.md) $\boldsymbol\xi=\boldsymbol\zeta e^{-i\omega t}$, multiplication of $-\omega^2\boldsymbol\zeta=F\boldsymbol\zeta$ by $\boldsymbol\zeta^*$ gives directly

$$
\omega^2=\frac{2W[\boldsymbol\zeta]}{\|\boldsymbol\zeta\|_\rho^2}>0,
$$

so all such frequencies are real. No variational principle has been assumed.

To prove instability, suppose some admissible $\boldsymbol\xi_0$ has $W_0=W[\boldsymbol\xi_0]<0$, and put $N_0=\|\boldsymbol\xi_0\|_\rho^2>0$. Choose the initial [velocity](../../../../../../velocity.md)

$$
\dot{\boldsymbol\xi}(0)=\alpha\boldsymbol\xi_0,\qquad\alpha=\sqrt{-2W_0/N_0}>0.
$$

Its [kinetic energy](../../../../../../kinetic-energy.md) exactly cancels $W_0$, so $E=0$ for the entire subsequent motion. Write $N(t)=\|\boldsymbol\xi(t)\|_\rho^2$. Since $F$ is self-adjoint,

$$
N'=2\operatorname{Re}\langle\boldsymbol\xi,\dot{\boldsymbol\xi}\rangle,\qquad N''=2\|\dot{\boldsymbol\xi}\|_\rho^2+2\langle\boldsymbol\xi,F\boldsymbol\xi\rangle.
$$

Zero [energy](../../../../../../energy.md) gives $\langle\boldsymbol\xi,F\boldsymbol\xi\rangle=\|\dot{\boldsymbol\xi}\|_\rho^2$, and hence $N''=4\|\dot{\boldsymbol\xi}\|_\rho^2\geq0$. Initially $N'(0)=2\alpha N_0>0$, so $N$ stays positive and its logarithm is defined. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) now gives

$$
\begin{aligned}
(\ln N)''&=\frac{NN''-(N')^2}{N^2}\\
&=\frac{4\left[N\|\dot{\boldsymbol\xi}\|_\rho^2-(\operatorname{Re}\langle\boldsymbol\xi,\dot{\boldsymbol\xi}\rangle)^2\right]}{N^2}\geq0.
\end{aligned}
$$

Therefore $(\ln N)'(t)\geq(\ln N)'(0)=2\alpha$, and integration proves

$$
\boxed{N(t)\geq N_0e^{2\alpha t},\qquad\|\boldsymbol\xi(t)\|_\rho\geq\|\boldsymbol\xi_0\|_\rho e^{\alpha t}.}
$$

This is an exponentially growing perturbation. Scaling the initial [displacement](../../../../../../displacement.md) and [velocity](../../../../../../velocity.md) down leaves $\alpha$ unchanged, so arbitrarily small initial perturbations display the same linear growth mechanism. It proves that a [negative-energy direction gives exponential growth in a self-adjoint wave equation](../../../../../../negative-energy-direction-gives-exponential-growth-in-a-self-adjoint-wave-equation.md), without assuming a discrete spectrum or quoting a trial-function variational theorem.

**Positive $W$ on nonzero displacements gives energetic stability; a negative direction gives instability.** For mathematical precision, a uniform bound on the mass-weighted [displacement](../../../../../../displacement.md) norm follows if $W\geq\tfrac12\omega_{\min}^2\|\boldsymbol\xi\|_\rho^2$ for some $\omega_{\min}>0$, giving $\|\boldsymbol\xi\|_\rho^2\leq2E/\omega_{\min}^2$. Strict positivity alone in an infinite-dimensional space need not supply such a uniform [spectral gap](../../../../../../spectral-gap.md); the standard [magnetohydrodynamic energy principle](../../../../../../magnetohydrodynamic-energy-principle.md) asserts energetic stability and absence of growing modes. Cases with zero directions are marginal and require separate consideration.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
