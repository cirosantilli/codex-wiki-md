<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [one-particle-irreducible correlation functions](../../../../one-particle-irreducible-correlation-function.md) to identify independent local [counterterms](../../../../counterterm.md). The exact internal symmetry $\phi\mapsto-\phi$ excludes odd $b$, and [Dirac fermion number conservation](../../../../dirac-fermion-number-conservation.md) requires equal numbers of $\psi$ and $\bar\psi$, so $f$ is even. From [b](../b.md), the complete list of potentially overall divergent vertices with external legs is:

- $\Gamma_{\phi\phi}$: $(b,f)=(2,0)$, $\omega=2-n_2$, potentially divergent for $n_2\leq2$.
- $\Gamma_{\phi^4}$: $(b,f)=(4,0)$, $\omega=1-n_2$, potentially divergent for $n_2\leq1$.
- $\Gamma_{\phi^6}$: $(b,f)=(6,0)$, $\omega=-n_2$, potentially divergent only for $n_2=0$.
- $\Gamma_{\bar\psi\psi}$: $(b,f)=(0,2)$, $\omega=1-n_2$, potentially divergent for $n_2\leq1$.
- $\Gamma_{\phi^2\bar\psi\psi}$: $(b,f)=(2,2)$, $\omega=-n_2$, potentially divergent only for $n_2=0$.

The zero-leg [vacuum diagrams](../../../../vacuum-feynman-diagram.md), with $\omega=3-n_2$, may also require a [vacuum energy density](../../../../vacuum-energy-density.md) subtraction. Four-fermion vertices have $\omega\leq-1$ and do not require a new four-fermion [counterterm](../../../../counterterm.md). These are superficial bounds: a particular allowed diagram can vanish or be convergent.

Locality and [Lorentz invariance](../../../../lorentz-invariance.md) restrict the divergent parts to a finite basis. The scalar two-point vertex can contain a constant and $p^2$; there is no [Lorentz scalar](../../../../lorentz-scalar.md) linear in a single [momentum](../../../../momentum-split.md). The fermion two-point vertex can contain $I$ and $\not p$. The remaining listed vertices have no allowed derivative divergence. A complete [counterterm Lagrangian](../../../../counterterm-lagrangian.md), up to [total derivatives](../../../../total-derivative.md), is therefore

$$
\boxed{\begin{aligned}
\mathcal L_{\rm ct}={}&-\delta\Lambda+\frac{\delta Z_\phi}{2}(\partial_\mu\phi)(\partial^\mu\phi)-\frac{\delta M^2}{2}\phi^2
+\delta Z_\psi\bar\psi i\gamma^\mu\partial_\mu\psi-\delta m\bar\psi\psi\\
&-\frac{\delta g_1}{2}\phi^2\bar\psi\psi-\frac{\delta g_2}{4!}\phi^4-\frac{\delta g_3}{6!}\phi^6.
\end{aligned}}
$$

The coefficients supply [wavefunction renormalization](../../../../wave-function-renormalization.md), [mass counterterms](../../../../mass-counterterm.md) and renormalizations of the three interactions already present. Recursive subtraction of [ultraviolet subdivergences](../../../../ultraviolet-subdivergence.md) then leaves only these local overall divergences. This finite [counterterm closure](../../../../counterterm-closure.md) is why the complete theory is expected to have perturbative [renormalizability](../../../../renormalizable-quantum-field-theory.md). It does not mean every listed coefficient first becomes nonzero at one loop, or that setting an allowed coupling to zero is stable under [renormalization](../../../../renormalization.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
