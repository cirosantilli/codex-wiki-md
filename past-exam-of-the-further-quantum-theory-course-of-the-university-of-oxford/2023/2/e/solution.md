<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $g\geq0$, the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) is nonnegative: its [quadratic form](../../../../quadratic-form-split.md) is $\hbar^2\int|\psi'|^2dx/(2m)+g(|\psi(a)|^2+|\psi(-a)|^2)\geq0$. Thus it has no negative-[energy](../../../../energy-split.md) [bound states](../../../../bound-state.md). A nonnegative-[energy](../../../../energy-split.md) exterior [wavefunction](../../../../wave-function-split.md) cannot be square integrable unless it vanishes identically, so there are no other [bound states](../../../../bound-state.md) either.

For $g<0$, set $\nu=-mg/\hbar^2>0$. The even equation is the zero of $f(\kappa)=\nu(1+e^{-2a\kappa})-\kappa$. Since $f(0)=2\nu>0$, $f(\kappa)\to-\infty$ and $f'(\kappa)=-2a\nu e^{-2a\kappa}-1<0$, the [intermediate value theorem](../../../../intermediate-value-theorem.md) and strict [monotonicity](../../../../monotonic-function.md) give exactly one positive [equation root](../../../../root-of-an-equation.md).

The odd equation is the zero of $h(\kappa)=\nu(1-e^{-2a\kappa})-\kappa$. Here $h(0)=0$, $h'(0)=2a\nu-1$, $h''(\kappa)=-4a^2\nu e^{-2a\kappa}<0$, and $h(\kappa)\to-\infty$. If $2a\nu\leq1$, strict [concavity](../../../../concave-function.md) makes $h(\kappa)<0$ for every $\kappa>0$. If $2a\nu>1$, $h$ initially increases, has exactly one maximum, and then decreases through zero exactly once. This proves the [bound-state count of an attractive symmetric double-delta potential](../../../../bound-state-count-of-an-attractive-symmetric-double-delta-potential.md):

$$
\boxed{N(g)=\begin{cases}
0,&g\geq0,\\
1,&-\dfrac{\hbar^2}{2ma}\leq g<0,\\
2,&g<-\dfrac{\hbar^2}{2ma}.
\end{cases}}
$$

At the threshold $g=-\hbar^2/(2ma)$, the odd zero-[energy](../../../../energy-split.md) solution is proportional to $x$ inside $(-a,a)$ and to $a\operatorname{sgn}x$ outside. It is bounded but not a [square-integrable function](../../../../square-integrable-function.md), so it is a [zero-energy scattering resonance](../../../../zero-energy-scattering-resonance.md) rather than a second [bound state](../../../../bound-state.md). Each negative-[energy](../../../../energy-split.md) [bound state](../../../../bound-state.md) is either even or odd by [nondegeneracy of one-dimensional bound states](../../../../nondegeneracy-of-one-dimensional-bound-states.md); the two branches above exhaust the count.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
