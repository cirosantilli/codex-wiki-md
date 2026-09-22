<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The exact mixture [equation of state](../../../../../../equation-of-state.md) is $\rho=(1-\phi)\rho_f+\phi\rho_p$. Keeping first-order terms in the small [particle volume fraction](../../../../../../particle-volume-fraction.md) and [thermal expansion](../../../../../../thermal-expansion.md) gives

$$
\boxed{\rho=\rho_0(1+\gamma\phi-\theta)}.
$$

The omitted term is $\rho_0\phi\theta$. The downward solid-volume [particle deposition flux](../../../../../../particle-deposition-flux.md) is $J_v=W_s\phi$; the corresponding particle [mass flux](../../../../../../mass-flux.md) is $J_m=\rho_pW_s\phi$. Uniform vertical mixing and constant layer depth imply

$$
H\dot\phi=-W_s\phi,\qquad \dot\theta=\beta\phi.
$$

For $W_s>0$, set $r=W_s/H$. Then

$$
\boxed{\phi(t)=\phi_0e^{-rt},\qquad
\theta(t)=\frac{\beta\phi_0}{r}(1-e^{-rt})},
$$

and hence

$$
\frac{\rho(t)-\rho_0}{\rho_0}
=\phi_0\left[\left(\gamma+\frac\beta r\right)e^{-rt}-\frac\beta r\right].
$$

The [heated particle-laden layer](../../../../../../heated-particle-laden-layer.md) loses its [stable density stratification](../../../../../../stable-density-stratification.md) when this contrast vanishes. For $\beta>0$, solving for the neutral-buoyancy time gives

$$
\boxed{T_s=\frac H{W_s}\log\left(1+\frac{\gamma W_s}{\beta H}\right)}.
$$

**The layer is neutral at $T_s$ and statically unstable for $t>T_s$.** The subsequent uniformly mixed lower-layer solution cannot represent the resulting overturning.

If $W_s=0$, then $\phi=\phi_0$, $\theta=\beta\phi_0t$, and the continuous limit is $T_s=\gamma/\beta$. If $\beta=0$, the layer stays denser than its surroundings at every finite time and becomes neutral only asymptotically when $W_s>0$; thus $T_s=\infty$. These limiting cases must replace the printed formula when its denominator vanishes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
