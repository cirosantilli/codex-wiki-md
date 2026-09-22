<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $L\ge2$, so neighbouring operators act at distinct sites. The identity

$$
S_n^xS_{n+1}^x+S_n^yS_{n+1}^y
=\tfrac12(S_n^+S_{n+1}^-+S_n^-S_{n+1}^+)
$$

expresses the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) of this [quantum XY chain](../../../../../quantum-xy-chain.md) in [spin ladder operators](../../../../../spin-ladder-operator.md). Substituting the [Schwinger boson representation](../../../../../schwinger-boson-representation.md) gives the requested quartic expression:

$$
\boxed{H=-\frac J2\sum_n
\left(a_n^\dagger b_n b_{n+1}^\dagger a_{n+1}
+b_n^\dagger a_n a_{n+1}^\dagger b_{n+1}\right).}
$$

Operators at different sites commute, allowing [normal ordering](../../../../../normal-ordering.md) without a correction here. For the first quartic term, the [inverse discrete Fourier transforms](../../../../../inverse-discrete-fourier-transform.md) give

$$
\begin{aligned}
\sum_n a_n^\dagger b_{n+1}^\dagger b_n a_{n+1}
&=\frac1{L^2}\sum_{n,p,q,r,t}
e^{i(p+q-r-t)n}e^{i(q-t)}A_p^\dagger B_q^\dagger B_r A_t\\
&=\frac1L\sum_{p,q,r,t}
\delta^{(L)}_{p+q,r+t}e^{i(q-t)}A_p^\dagger B_q^\dagger B_r A_t.
\end{aligned}
$$

Here $\delta^{(L)}$ is one when its two [momenta](../../../../../momentum-split.md) agree modulo $2\pi$ and zero otherwise; it expresses lattice [momentum conservation](../../../../../momentum-conservation.md). The other quartic term has the same ordered operators with phase $e^{i(p-r)}$. On the support of this [Kronecker delta](../../../../../kronecker-delta.md), $p-r=t-q$ modulo $2\pi$, so the two phases sum to $2\cos(q-t)$. Thus the [Fourier vertex of a Schwinger boson chain](../../../../../fourier-vertex-of-a-schwinger-boson-chain.md) is

$$
\boxed{H=-\frac JL\sum_{p,q,r,t}
\delta^{(L)}_{p+q,r+t}\cos(q-t)\,
A_p^\dagger B_q^\dagger B_r A_t.}
$$

An equivalent three-sum expression sets $t=p+q-r$ modulo $2\pi$, so its coefficient is $\cos(r-p)$. The factor $1/L$ comes from four factors $L^{-1/2}$ and one site sum, while the factor of two from the two exchange terms cancels the original $1/2$. The formula is [Hermitian](../../../../../hermitian-operator.md): conjugation exchanges $p$ with $t$ and $q$ with $r$, and the coefficient is unchanged after imposing lattice [momentum conservation](../../../../../momentum-conservation.md). It also preserves each local total [boson](../../../../../boson.md) number in its real-space form, hence preserves the physical constrained subspace.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
