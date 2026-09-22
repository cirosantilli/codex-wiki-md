<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For bound [hydrogen atom](../../../../hydrogen-atom.md) states, the radial [wave function](../../../../wave-function-split.md) is regular and finite at the origin, and decays at infinity so that $4\pi\int_0^\infty r^2|\Psi(r)|^2\,dr<\infty$. Equivalently the reduced radial function $w(r)=r\Psi(r)$ has $w(0)=0$ and is square integrable on the half-line. A singular $1/r$ branch is not an admissible regular Coulomb [eigenfunction](../../../../eigenfunction.md); its [derivative](../../../../derivative.md) energy diverges and it introduces an origin singularity absent from the [Hamiltonian](../../../../hamiltonian.md) domain.

Write $\kappa=e^2/(4\pi\epsilon_0)$, so $a=\hbar^2/(m\kappa)$. Multiplication by $r$ turns the radial equation into

$$
w''+\left(-\mu^2+\frac2{ar}\right)w=0,qquad
\mu^2=-2mE/\hbar^2.
$$

Since $w=a e^{-\lambda R}f(R)$ and $r=aR$, substitution gives

$$
\boxed{f''-2\lambda f'+(\lambda^2-\mu^2a^2+2/R)f=0.}
$$

Choose $\boxed{\lambda=\mu a>0}$ to remove the constant coefficient and factor out the decaying exponential. For $f=\sum_{k\geq0}a_kR^{k+c}$, the lowest power has coefficient $c(c-1)a_0$, so $\boxed{c(c-1)=0}$. The $c=0$ behavior would give $\Psi\sim a_0/R$, violating regularity; choose $c=1$.

Matching successive powers then yields

$$
\boxed{a_{k+1}=\frac{2\{\lambda(k+1)-1\}}{(k+2)(k+1)}a_k.}
$$

A nonterminating tail eventually has one sign, and its coefficient ratio is asymptotic to $2\lambda/k$. More precisely, for any $0<\delta<\lambda$, the ratio is eventually at least $(2\lambda-\delta)/(k+1)$. Its same-sign tail consequently dominates a positive constant times the exponential series of rate $2\lambda-\delta$, up to finitely many terms. The factor $e^{-\lambda R}$ cannot then make $\Psi$ decay. Thus square integrability forces termination.

If the last nonzero term is $a_{n-1}R^n$, termination requires $\lambda n=1$. Therefore

$$
\boxed{E_n=-\frac{\hbar^2}{2ma^2n^2}=-\frac A{2n^2},\qquad
A=\frac{\hbar^2}{ma^2}=\frac{me^4}{16\pi^2\epsilon_0^2\hbar^2}.}
$$

For $n=1$, $\lambda=1$, $f$ is proportional to $R$, and

$$
\boxed{\Psi_0(r)\propto e^{-r/a}.}
$$

The radial volume element is $4\pi r^2dr$, so the mean radius is the ratio of the radius-weighted [norm](../../../../norm.md) [integral](../../../../integral-split.md) to the [norm](../../../../norm.md) [integral](../../../../integral-split.md). With $r=aR$, the common angular and [normalization](../../../../normalization.md) factors cancel:

$$
\langle r\rangle=a\frac{\int_0^\infty R^3e^{-2\lambda R}\,dR}
{\int_0^\infty R^2e^{-2\lambda R}\,dR}
=\frac{3a}{2\lambda}.
$$

In the [ground state](../../../../ground-state.md) $\boxed{\langle r\rangle=3a/2}$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
