<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [coherent state](../../../../coherent-state.md) in the zero mode has mean [occupation number](../../../../occupation-number.md) $N_0$. The other [occupation numbers](../../../../occupation-number.md) follow from part (c), giving exactly

$$
\boxed{\langle\hat N\rangle=N_0+D,\qquad
D\equiv\sum_{\mathbf k\ne0}\sinh^2\theta_k.}
$$

Impose the fixed mean [particle number](../../../../particle-number.md) $\langle\hat N\rangle=N$ by choosing

$$
\boxed{N_0=N-D.}
$$

Here $D$ is the [quantum depletion of a Bose condensate](../../../../quantum-depletion-of-a-bose-condensate.md). The approximation requires $0\le D\ll N$, so $N_0$ remains positive and macroscopically large. The specified [coherent state](../../../../coherent-state.md) and [multimode squeezed vacuum](../../../../multimode-squeezed-vacuum.md) are not exact [eigenstates](../../../../eigenstate.md) of the total [number operator](../../../../number-operator.md); $N$ in this variational construction is their prescribed mean [particle number](../../../../particle-number.md).

Write $P=\sum_{\mathbf k\ne0}s_kc_k$. Substituting into the retained part of the [interaction energy](../../../../interaction-energy.md) before truncating gives

$$
\begin{aligned}
\langle H_{\rm int}\rangle
&\simeq\frac{u}{2V}(N-D)^2+\frac{u}{V}(N-D)(2D-P)\\
&=\frac{uN^2}{2V}+\frac{uN}{V}(D-P)
+\frac{u}{V}\left(-\frac32D^2+DP\right).
\end{aligned}
$$

The last two terms quadratic in $D,P$ have no explicit large-$N$ factor when the [Bogoliubov transformation](../../../../bogoliubov-transformation.md) parameters are held fixed, and are discarded along with the nonzero-mode quartic contribution already omitted in part (c). This is the same truncation that underlies the [number-conserving Bogoliubov quadratic Hamiltonian](../../../../number-conserving-bogoliubov-quadratic-hamiltonian.md). Thus, defining the physical [number density](../../../../number-density.md) correctly as $\rho=N/V=N/L^3$,

$$
\boxed{\langle H_{\rm int}\rangle\simeq\frac{u\rho}{2}N
+u\rho\sum_{\mathbf k\ne0}
(\sinh^2\theta_k-\sinh\theta_k\cosh\theta_k).}
$$

Replacing $N_0$ by $N$ at the outset would give the wrong coefficient $2\sinh^2\theta_k$: expanding the leading condensate [interaction energy](../../../../interaction-energy.md) supplies the necessary subtraction.

**The printed definition $\rho=N/L$ is an error.** In three dimensions the [contact interaction](../../../../contact-interaction-quantum-mechanics.md) coupling $u$ has units of [energy](../../../../energy-split.md) times [volume](../../../../volume.md), so $uN/L$ does not even have units of [energy](../../../../energy-split.md). There is a direct counterexample with no depletion: when $\theta_k=0$, the specified [coherent state](../../../../coherent-state.md) has exactly $\langle H_{\rm int}\rangle=uN^2/(2L^3)$. In fixed length and [energy](../../../../energy-split.md) units, $L=2$, $u=1$ and $N=100$ give $625$, whereas the printed $u\rho N/2$ with $\rho=N/L$ gives $2500$. The requested formula and the minimization in part (e) hold with $\rho=N/L^3$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
