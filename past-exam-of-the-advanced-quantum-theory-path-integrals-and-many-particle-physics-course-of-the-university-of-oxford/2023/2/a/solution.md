<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\hbar=1$ throughout. Let $N_a=a^\dagger a$, $N_b=b^\dagger b$ and $N=N_a+N_b$. Operators belonging to different [boson](../../../../boson.md) species commute. The proposed [Schwinger boson representation](../../../../schwinger-boson-representation.md) gives

$$
\begin{aligned}
S^+S^-&=a^\dagger b b^\dagger a=N_a(N_b+1),\\
S^-S^+&=b^\dagger a a^\dagger b=N_b(N_a+1).
\end{aligned}
$$

Consequently the first of the [spin commutation relations](../../../../spin-commutation-relations.md) is

$$
\boxed{[S^+,S^-]=N_a-N_b=2S^z.}
$$

The [number operator](../../../../number-operator.md) [commutators](../../../../commutator.md) $[N_a,a^\dagger]=a^\dagger$, $[N_a,a]=-a$ and their $b$ counterparts give

$$
\begin{aligned}
[S^z,S^+]&=\tfrac12([N_a,a^\dagger]b-a^\dagger[N_b,b])=a^\dagger b=S^+,\\
[S^z,S^-]&=-b^\dagger a=-S^-.
\end{aligned}
$$

Thus all the [spin commutation relations](../../../../spin-commutation-relations.md) hold. Also $[N,S^\pm]=[N,S^z]=0$: each fixed-$N$ sector is invariant. To identify its [spin](../../../../spin.md), calculate the [Casimir operator](../../../../casimir-element.md):

$$
\begin{aligned}
S^2&=(S^z)^2+\tfrac12(S^+S^-+S^-S^+)\\
&=\tfrac14(N_a-N_b)^2+N_aN_b+\tfrac12(N_a+N_b)\\
&=\frac N2\left(\frac N2+1\right).
\end{aligned}
$$

The [irreducible spin representation](../../../../irreducible-spin-representation.md) with prescribed $s$ therefore requires $N=2s$, and its normalized [Fock basis](../../../../fock-basis.md) correspondence is

$$
\boxed{|s,m\rangle\ \longleftrightarrow\ |s+m,s-m\rangle
=\frac{(a^\dagger)^{s+m}(b^\dagger)^{s-m}}
{\sqrt{(s+m)!(s-m)!}}|0,0\rangle.}
$$

Conversely, $s=(n_a+n_b)/2$ and $m=(n_a-n_b)/2$. The nonnegative integer [occupation numbers](../../../../occupation-number.md) give precisely $m=-s,-s+1,\ldots,s$, and there are $2s+1$ such states. As a check, the [spin raising operator](../../../../spin-raising-operator.md) acts as

$$
a^\dagger b|s+m,s-m\rangle
=\sqrt{(s+m+1)(s-m)}\,|s+m+1,s-m-1\rangle,
$$

which is the usual [spin ladder operator](../../../../spin-ladder-operator.md) coefficient $\sqrt{s(s+1)-m(m+1)}$.

For a lattice of fixed [spins](../../../../spin.md), the [local spin constraint in the Schwinger boson representation](../../../../local-spin-constraint-in-the-schwinger-boson-representation.md) is essential:

$$
\boxed{(a_n^\dagger a_n+b_n^\dagger b_n)|\psi\rangle=2s|\psi\rangle
\quad\text{at every site }n.}
$$

The full two-species [bosonic Fock space](../../../../bosonic-fock-space.md) also contains other local [irreducible spin representations](../../../../irreducible-spin-representation.md); fixing only the total [boson](../../../../boson.md) number does not remove them.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
