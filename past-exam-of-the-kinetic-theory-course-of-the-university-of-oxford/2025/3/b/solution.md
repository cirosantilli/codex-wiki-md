<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Collisionless Boltzmann equation](../../../../collisionless-boltzmann-equation.md) in [action-angle variables](../../../../action-angle-variables.md),

$$
\partial_tf+\{f,H\}=0,\qquad \{f,H\}=\partial_{\boldsymbol\theta}f\cdot\partial_{\mathbf J}H-\partial_{\mathbf J}f\cdot\partial_{\boldsymbol\theta}H.
$$

Define the orbital [frequency](../../../../frequency.md) vector by

$$
\boxed{\boldsymbol\Omega(\mathbf J)=\partial_{\mathbf J}H_0=(\Omega_\varphi,\Omega_R).}
$$

The slow evolution of the angle average $f_0$ starts at second order in the perturbation. At first order, the [Poisson bracket](../../../../poisson-bracket.md) therefore gives

$$
(\partial_t+\boldsymbol\Omega\cdot\partial_{\boldsymbol\theta})\delta f=\partial_{\mathbf J}f_0\cdot\partial_{\boldsymbol\theta}\delta\Phi.
$$

For the $\mathbf k$th term in the [Fourier series](../../../../fourier-series-split.md), this reads

$$
(\partial_t+i\mathbf k\cdot\boldsymbol\Omega)\delta f_{\mathbf k}=i\mathbf k\cdot\partial_{\mathbf J}f_0\,\delta\phi_{\mathbf k}.
$$

The lowercase $\delta\phi_{\mathbf k}$ here denotes the [Fourier coefficient](../../../../fourier-coefficient.md) of the uppercase $\delta\Phi$ in the [Hamiltonian](../../../../hamiltonian.md); these are the same perturbing potential. Multiply by the [integrating factor](../../../../integrating-factor.md) $e^{i\mathbf k\cdot\boldsymbol\Omega t}$ and set the initial homogeneous response to zero. One obtains

$$
\boxed{\delta f_{\mathbf k}(\mathbf J,t)=i\int_0^t dt'\,\mathbf k\cdot\frac{\partial f_0(\mathbf J,t')}{\partial\mathbf J}\,e^{-i\mathbf k\cdot\boldsymbol\Omega(t-t')}\delta\phi_{\mathbf k}(\mathbf J,t').}
$$

Retaining the slow time dependence of $f_0$ inside this [integral](../../../../integral-split.md) is compatible with the subsequent second-order calculation; changes in $\boldsymbol\Omega$ caused by that slow evolution affect only higher orders in this approximation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
