<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At first order the [Dyson expansion](../../../../../dyson-series.md) inserts $iS_{\mathrm{int}}=\lambda\int d^4x\,\bar\psi_\alpha(x)(\gamma_5)_{\alpha\beta}\psi_\beta(x)\phi(x)$. Contract the [scalar field](../../../../../scalar-field.md) at the [vertex](../../../../../vertex-graph-theory.md) with the external [scalar](../../../../../scalar-field.md). The four remaining [fermion](../../../../../fermion.md) fields have two admissible pairings: both external [fermions](../../../../../fermion.md) attach to the [vertex](../../../../../vertex-graph-theory.md), or the two [vertex](../../../../../vertex-graph-theory.md) [fermions](../../../../../fermion.md) contract with each other while the external pair contracts freely. [Wick's theorem](../../../../../wick-s-theorem.md) gives

$$
\boxed{\begin{aligned}
\langle T\phi(y)\psi_\rho(z)\bar\psi_\sigma(w)\rangle
={}&\lambda(\gamma_5)_{\alpha\beta}\int d^4x\,i\Delta_F(y-x)\Bigl[
 iS_F(x-w)_{\beta\sigma}\,iS_F(z-x)_{\rho\alpha}\\
&\hspace{40pt}-iS_F(0)_{\beta\alpha}\,iS_F(z-w)_{\rho\sigma}\Bigr]+O(\lambda^3).
\end{aligned}}
$$

The minus sign in the second term is the [fermion sign](../../../../../fermionic-sign.md) of the closed [contraction](../../../../../wick-contraction.md): $\langle T\bar\psi_\alpha(x)\psi_\beta(x)\rangle=-iS_F(0)_{\beta\alpha}$. The first term is connected; the second is a scalar-attached [fermion](../../../../../fermion.md) [tadpole](../../../../../tadpole-diagram.md) multiplied by a disconnected free external [fermion propagator](../../../../../dirac-propagator.md). The full time-ordered expectation includes both topologies, whereas the connected [generating functional](../../../../../generating-functional.md) retains only the first. There is no order-$\lambda^2$ contribution in this pure Yukawa expansion because the total number of [scalar fields](../../../../../scalar-field.md) would be odd.

For a [parity-preserving](../../../../../parity.md) free propagator, the [tadpole](../../../../../tadpole-diagram.md) coefficient is $\operatorname{tr}[\gamma_5S_F(0)]$, whose integrand contains only $\operatorname{tr}\gamma_5$ and $\operatorname{tr}(\gamma_5\gamma^\mu)$. Both vanish. Thus the second term is a legitimate formal [Wick contraction](../../../../../wick-contraction.md) but is zero with a compatible regulator; [normal ordering](../../../../../normal-ordering.md) the [interaction](../../../../../interaction-term.md) removes it from the outset.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
