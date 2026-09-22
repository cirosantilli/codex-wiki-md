<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $\langle O\rangle=\langle G|O|G\rangle$. The given state is a [two-species uniform boson number state](../../../../two-species-uniform-boson-number-state.md): only the $q=0$ mode of each species is occupied. Applying an [annihilation operator](../../../../annihilation-operator.md) to an unoccupied mode gives zero, while $A_0^\dagger A_0$ has [eigenvalue](../../../../eigenvalue.md) $n_A$. Thus

$$
\boxed{\langle A_q^\dagger A_k\rangle=n_A\delta_{q0}\delta_{k0},\qquad
\langle B_q^\dagger B_k\rangle=n_B\delta_{q0}\delta_{k0}.}
$$

The two species have independent fixed [occupation numbers](../../../../occupation-number.md), so mixed [expectation values](../../../../expectation-value.md) factorize. The inverse [discrete Fourier transforms](../../../../discrete-fourier-transform-split.md) yield

$$
\langle a_i^\dagger a_j\rangle=\frac{n_A}{L},\qquad
\langle b_i^\dagger b_j\rangle=\frac{n_B}{L},\qquad
\boxed{\langle a_n^\dagger a_n+b_n^\dagger b_n\rangle
=\frac{n_A+n_B}{L}.}
$$

In the momentum-space [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md), only $p=q=r=t=0$ contributes: each [annihilation operator](../../../../annihilation-operator.md) must remove an occupied [boson](../../../../boson.md), and each [creation operator](../../../../creation-operator.md) must restore it to the same mode. Hence

$$
\langle A_p^\dagger B_q^\dagger B_r A_t\rangle
=n_An_B\delta_{p0}\delta_{q0}\delta_{r0}\delta_{t0},
\qquad
\boxed{\langle H\rangle=-\frac JLn_An_B.}
$$

There is no replacement of $n_B$ by $n_B+1$ in this [energy](../../../../energy-split.md): in the real-space calculation the relevant neighboring-site [commutator](../../../../commutator.md) is zero. Both expressions assume distinct neighbouring sites, as in [ii](../b/ii.md).

To match the prescribed [spin](../../../../spin.md) length in the mean, impose $n_A+n_B=2sL=:N$. At fixed integer $N$, the [energy](../../../../energy-split.md) is minimized by maximizing $n_An_B=[N^2-(n_A-n_B)^2]/4$. Consequently the best choices within this relaxed family are

$$
\boxed{\{n_A,n_B\}=\{\lfloor sL\rfloor,\lceil sL\rceil\}.}
$$

When $N$ is even, $n_A=n_B=sL$ and $\langle H\rangle=-Js^2L$. When $N$ is odd, either assignment of $(N-1)/2,(N+1)/2$ gives $\langle H\rangle=-J(N^2-1)/(4L)$. Without fixing $N$, this auxiliary [boson](../../../../boson.md) [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) has no lower bound: taking $n_A=n_B\to\infty$ sends its [expectation value](../../../../expectation-value.md) to $-\infty$.

Next, $S_i^x=(a_i^\dagger b_i+b_i^\dagger a_i)/2$. Each term changes the two species' [occupation numbers](../../../../occupation-number.md), producing a state [orthogonal](../../../../orthogonal-vectors.md) to $|G\rangle$. Therefore

$$
\boxed{\langle S_i^x\rangle=0,\qquad \langle S_i^y\rangle=0,\qquad
\langle S_i^z\rangle=\frac{n_A-n_B}{2L}.}
$$

For distinct sites $i,j$ modulo $L$, expand the product of the two [spin operators](../../../../spin-operator.md). The terms $S_i^+S_j^+$ and $S_i^-S_j^-$ again have zero [expectation value](../../../../expectation-value.md). The remaining terms give

$$
\begin{aligned}
\langle S_i^+S_j^-\rangle
&=\langle a_i^\dagger a_j\rangle\langle b_i b_j^\dagger\rangle
=\frac{n_A}{L}\frac{n_B}{L},\\
\langle S_i^-S_j^+\rangle&=\frac{n_An_B}{L^2}.
\end{aligned}
$$

Here $\langle b_i b_j^\dagger\rangle=n_B/L+\delta_{ij}$ and the [Kronecker delta](../../../../kronecker-delta.md) vanishes at distinct sites. Consequently

$$
\boxed{\langle S_m^xS_{m+n}^x\rangle=\frac{n_An_B}{2L^2}
\quad(n\not\equiv0\pmod L).}
$$

The same holds for the $y$ components. At the balanced choice and as $L\to\infty$, each transverse [two-point correlation function](../../../../two-point-correlation-function.md) tends to $s^2/2$ independently of separation, whereas the one-point transverse [magnetization](../../../../magnetization.md) is zero. This is [transverse spin order in a number eigenstate](../../../../transverse-spin-order-in-a-number-eigenstate.md): the state has a definite total $S^z=(n_A-n_B)/2$ and retains the global [U(1)](../../../../circle-group.md) [symmetry](../../../../symmetry-physics.md) of rotations about $z$, yet has the transverse correlations of an ordered state with no selected common azimuth. The sum of the $x$ and $y$ correlations tends to $s^2$, describing ferromagnetic [long-range order](../../../../long-range-order.md) within this approximation. The [thermodynamic limit](../../../../thermodynamic-limit.md) is understood with both the separation and $L$ growing, without identifying the two sites periodically.

**Fixed-spin qualification.** The proposed state is not actually in the physical fixed-$s$ [Hilbert space](../../../../hilbert-space-split.md) for $s>0,L>1$. It satisfies the [local spin constraint in the Schwinger boson representation](../../../../local-spin-constraint-in-the-schwinger-boson-representation.md) only in [expectation value](../../../../expectation-value.md). For example, with $L=2,s=1/2,n_A=n_B=1$,

$$
|G\rangle=\tfrac12(a_0^\dagger+a_1^\dagger)(b_0^\dagger+b_1^\dagger)|\mathrm{vac}\rangle.
$$

The nonzero component $a_0^\dagger b_0^\dagger|\mathrm{vac}\rangle/2$ has local total [occupation numbers](../../../../occupation-number.md) $(2,0)$ and hence local [spins](../../../../spin.md) $(1,0)$, instead of $(1/2,1/2)$. More generally the local total [number operator](../../../../number-operator.md) $N_n$ has [variance](../../../../variance-split.md)

$$
\boxed{\operatorname{Var}(N_n)
=\frac{n_A+n_B}{L}\left(1-\frac1L\right)
=2s\left(1-\frac1L\right)>0.}
$$

Each species contributes a [binomial distribution](../../../../binomial-distribution.md) at a given site, with success probability $1/L$, and the two contributions are independent. In the physical subspace that [variance](../../../../variance-split.md) must be zero. The proposed state even has

$$
\langle S_n^2\rangle=s(s+1)+\tfrac14\operatorname{Var}(N_n),
$$

by the [Casimir operator](../../../../casimir-element.md) identity from [a](../a.md). Thus the calculated [energy](../../../../energy-split.md) is a relaxed [mean-field theory](../../../../mean-field-theory.md) estimate, not a [Rayleigh-Ritz variational principle](../../../../rayleigh-ritz-variational-principle.md) bound for the stated fixed-$s$ [quantum XY chain](../../../../quantum-xy-chain.md). Projecting onto $N_n=2s$ at every site would give a physical trial state and generally change its [expectation values](../../../../expectation-value.md); in the two-site example the projected state has [energy](../../../../energy-split.md) $-J$, whereas the unprojected value is $-J/2$. The calculated [long-range order](../../../../long-range-order.md) characterizes the supplied approximation and does not establish [long-range order](../../../../long-range-order.md) in the exact one-dimensional [ground state](../../../../ground-state.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
