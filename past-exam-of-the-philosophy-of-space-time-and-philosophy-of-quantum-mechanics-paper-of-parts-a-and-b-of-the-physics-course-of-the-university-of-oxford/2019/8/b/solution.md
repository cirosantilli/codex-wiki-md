<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**[Quantum mechanics](../../../../quantum-mechanics-split.md) is compatible with [quantum no-signalling](../../../../quantum-no-signalling.md), but its full correlations are incompatible with [Bell local causality](../../../../bell-local-causality.md) under the usual additional assumptions.** The answer depends on which locality condition is meant. A local operational prohibition on controllable faster-than-light communication is weaker than a causal explanation of correlations by a complete shared past.

Let $a,b\in\{-1,1\}$ be outcomes, $x,y$ local settings and $\lambda$ a complete relevant past specification. [Bell factorization](../../../../bell-local-causality.md) and [measurement independence](../../../../measurement-independence.md) demand

$$
p(a,b|x,y,\lambda)=p(a|x,\lambda)p(b|y,\lambda),
\qquad \rho(\lambda|x,y)=\rho(\lambda).
$$

Neither assumes deterministic response. Put $A_x(\lambda)=\sum_a a\,p(a|x,\lambda)$ and similarly $B_y$, so $|A_x|,|B_y|\leq1$. Pointwise,

$$
|A_0(B_0+B_1)+A_1(B_0-B_1)|
\leq|B_0+B_1|+|B_0-B_1|\leq2.
$$

Averaging with the same $\rho$ for all settings gives the [CHSH inequality](../../../../chsh-inequality.md) $|E_{00}+E_{01}+E_{10}-E_{11}|\leq2$. For a [spin singlet state](../../../../spin-singlet-state.md), $E(\mathbf a,\mathbf b)=-\mathbf a\cdot\mathbf b$. Choose $\mathbf a_0=\widehat z$, $\mathbf a_1=\widehat x$, $\mathbf b_0=(\widehat z+\widehat x)/\sqrt2$, $\mathbf b_1=(\widehat z-\widehat x)/\sqrt2$; the magnitude becomes $2\sqrt2$. Thus the assumptions cannot all be maintained.[1964, §§II–V, local response functions and incompatibility with singlet correlations; the displayed CHSH derivation is the stochastic extension](../../../../on-the-einstein-podolsky-rosen-paradox-by-john-stewart-bell.md)

There is nevertheless no signalling contradiction. If a local unread measurement has [Kraus operators](../../../../kraus-operator.md) $M_a$ with $\sum_aM_a^\dagger M_a=I$, then

$$
\rho'_B=\operatorname{tr}_A\sum_a(M_a\otimes I)\rho_{AB}(M_a^\dagger\otimes I)=\rho_B.
$$

The equality follows by testing both sides against any distant [observable](../../../../observable.md) and using cyclicity of the [trace](../../../../matrix-trace.md). Distant conditional states can differ after selecting $a$, but communicating that selection needs an ordinary message. The [microcausality](../../../../microcausality.md) condition in [quantum field theory](../../../../quantum-field-theory-split.md) similarly ensures commutation of spacelike-separated local [observables](../../../../observable.md); it does not make the vacuum or other entangled [quantum states](../../../../quantum-state.md) Bell-factorizable.

One can preserve different notions of locality by changing premises. [Bohmian mechanics](../../../../de-broglie-bohm-theory.md) retains unique outcomes but its [guidance equation](../../../../guidance-equation.md) is nonlocal for entangled systems; [quantum equilibrium equivariance](../../../../quantum-equilibrium-equivariance.md) preserves the equilibrium distribution which masks that dependence from signalling. The [many-worlds interpretation](../../../../many-worlds-interpretation.md) can combine local interaction equations with no unique global outcome, but a claim of locality must explain its branch-relative correlations; it has not thereby constructed the above Bell-local single-outcome model. The [measurement-independence loophole](../../../../measurement-independence-loophole.md), including suitable retrocausal or correlated-setting models, drops the shared setting-independent $\rho$ premise. Such models are logical possibilities, not demonstrations that the ordinary locality assumptions survive unchanged.

The justified answer is therefore conditional rather than an unqualified yes or no. Operational locality is retained by the quantum formalism. A theory reproducing all its correlations cannot retain Bell factorization, independent settings and the ordinary joint-outcome framework together. Neither denial of hidden variables nor an appeal to relativity alone removes the probabilistic contradiction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8](../../8.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the philosophy of space-time and philosophy of quantum mechanics paper of Parts A and B of the physics course of the University of Oxford](../../../split.md)
5. [Philosophy of space-time and philosophy of quantum mechanics paper of Parts A and B of the physics course of the University of Oxford](../../../../philosophy-of-space-time-and-philosophy-of-quantum-mechanics-paper-of-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
