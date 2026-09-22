<h1 id="section-b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [self-adjoint](../../../../self-adjoint-operator.md) [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) bounded below with [ground-state energy](../../../../ground-state-energy.md) $E_0$, every admissible nonzero trial [wavefunction](../../../../wave-function-split.md) has a [Rayleigh quotient](../../../../rayleigh-quotient.md) at least $E_0$. To see this explicitly in a complete [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md), write $|\psi\rangle=\sum_n c_n|n\rangle$ with $H|n\rangle=E_n|n\rangle$. Then

$$
\frac{\langle\psi|H|\psi\rangle}{\langle\psi|\psi\rangle}-E_0
=\frac{\sum_n|c_n|^2(E_n-E_0)}{\sum_n|c_n|^2}\geq0,
$$

so

$$
\boxed{E_0\leq\frac{\langle\psi|H|\psi\rangle}{\langle\psi|\psi\rangle}.}
$$

For continuous spectral components, the [spectral theorem](../../../../spectral-theorem.md) replaces the sum by an integral with the same nonnegative integrand. Equality requires the trial [quantum state](../../../../quantum-state.md) to lie entirely in the [ground-state subspace](../../../../ground-state-subspace.md). The [variational method](../../../../variational-method.md) chooses a tractable family, evaluates the quotient and minimizes over its parameters. This gives an upper bound; enlarging the family can only improve that bound. The trial must belong to the [operator domain](../../../../operator-domain.md) for the operator expression above, or have finite energy in the corresponding quadratic-form version of the [quantum variational principle](../../../../quantum-variational-principle.md).

For the oscillator, use the standard kinetic operator $T=-\hbar^2d^2/(2m\,dx^2)$: the original PDF omits the superscript $2$ on the derivative in its numerator. Take $a>0$, and normalize the scaled exact [ground state](../../../../ground-state.md) as

$$
\psi_\lambda(x)=\sqrt\lambda\,\phi_0(\lambda x),\qquad\lambda>0.
$$

The factor $\sqrt\lambda$ is optional in a quotient but makes the calculation transparent. Changing variable to $u=\lambda x$ and differentiating the scaled [wavefunction](../../../../wave-function-split.md) gives

$$
\langle T\rangle_\lambda=\lambda^2T_0,\qquad
\langle V\rangle_\lambda=\lambda^{-2}V_0,
\qquad T_0=\langle\phi_0|T|\phi_0\rangle,\quad V_0=\langle\phi_0|ax^2|\phi_0\rangle.
$$

At $\lambda=1$ this trial is the exact minimizing state, so its energy $\mathcal E(\lambda)=\lambda^2T_0+\lambda^{-2}V_0$ has zero derivative there. Hence $2T_0-2V_0=0$. Since $E_0=T_0+V_0$,

$$
\boxed{\langle T\rangle=\langle V\rangle=E_0/2.}
$$

This is the [quantum virial identity from scaling](../../../../quantum-virial-identity-from-scaling.md) for a quadratic potential, and hence the oscillator form of the [virial theorem](../../../../virial-theorem.md).

For the inverse-power attraction, take $a>0$ and suppose, for contradiction, that an exact [ground state](../../../../ground-state.md) exists with separately finite [kinetic energy](../../../../kinetic-energy.md) $T_0>0$ and potential mean $U_0<0$, admitting the same dilation variations. Homogeneity now gives

$$
\mathcal E(\lambda)=\lambda^2T_0+\lambda^pU_0.
$$

Stationarity at $\lambda=1$ would require $2T_0+pU_0=0$. Its second derivative would then be

$$
\mathcal E''(1)=2T_0+p(p-1)U_0=2(2-p)T_0.
$$

For $p>2$ this is negative, contradicting a ground-state minimum. More strongly, one does not need a presumed exact state: choose any normalized smooth test function supported away from the singular origin. Its $T$ and $U$ are finite, and its scaled quotient satisfies

$$
\boxed{\mathcal E(\lambda)=\lambda^2T+\lambda^pU\longrightarrow-\infty
\quad(\lambda\to\infty,\ p>2).}
$$

The unregularized attraction therefore exhibits [fall to the centre for a supercritical inverse-power potential](../../../../fall-to-the-centre-for-a-supercritical-inverse-power-potential.md) and has no stable [ground state](../../../../ground-state.md).

There is a necessary qualification to the PDF's broader wording about “no bound state”. Under the usual finite-energy [virial theorem](../../../../virial-theorem.md) assumptions, a putative negative-energy [bound state](../../../../bound-state.md) would satisfy

$$
E=T+U=\left(1-\frac2p\right)T>0,
$$

which contradicts being below the continuum threshold at zero. Thus no negative-energy bound state satisfying those regularity assumptions is possible. But this singular differential expression needs a specified domain at $x=0$; separately divergent kinetic and potential means or boundary conditions not preserved by dilation invalidate that ordinary calculation. The [domain assumptions in singular-potential virial arguments](../../../../domain-assumptions-in-singular-potential-virial-arguments.md) must therefore be stated: the scaling proof establishes absence of a semibounded ground-state problem, rather than a domain-independent theorem about every formal square-integrable solution. A short-distance regularization would be a different potential.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
