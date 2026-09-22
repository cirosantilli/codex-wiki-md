<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Normalize the specified state by $\langle0|0\rangle=1$ and write $\langle A\rangle=\langle0|A|0\rangle$. Its zero mode is a [coherent state](../../../../coherent-state.md), so any normally ordered product of zero-mode [creation operators](../../../../creation-operator.md) and [annihilation operators](../../../../annihilation-operator.md) can be evaluated using $\psi_0\mapsto\sqrt{N_0}$ and $\psi_0^\dagger\mapsto\sqrt{N_0}$. In particular $\langle(\psi_0^\dagger)^2\psi_0^2\rangle=N_0^2$, rather than $N_0(N_0-1)$, which would apply to a zero-mode [number state](../../../../number-state.md).

Sort the [momentum-space contact-interaction Hamiltonian](../../../../momentum-space-contact-interaction-hamiltonian.md) by its number of zero-mode factors. Four such factors give $uN_0^2/(2V)$. Three zero-mode factors and one nonzero [momentum](../../../../momentum-split.md) violate [momentum conservation](../../../../momentum-conservation.md), so no such term survives. With two zero-mode factors there are three possibilities:

- Two zero-mode [creation operators](../../../../creation-operator.md) leave the opposite-[momentum](../../../../momentum-split.md) pair $\psi_{\mathbf k}\psi_{-\mathbf k}$.
- Two zero-mode [annihilation operators](../../../../annihilation-operator.md) leave $\psi_{\mathbf k}^\dagger\psi_{-\mathbf k}^\dagger$.
- One zero-mode factor on each side leaves $\psi_{\mathbf k}^\dagger\psi_{\mathbf k}$. Choosing which of the two [creation operators](../../../../creation-operator.md) and which of the two [annihilation operators](../../../../annihilation-operator.md) are zero gives four placements.

The sums over $\mathbf k\ne0$ include both members of each opposite-[momentum](../../../../momentum-split.md) pair, consistently with the overall factor $1/2$. Terms with one zero-mode factor contain three nonzero-mode factors; their [expected values](../../../../expected-value-split.md) vanish in the centered [multimode squeezed vacuum](../../../../multimode-squeezed-vacuum.md). Indeed each $\psi$ is linear in $\varphi,\varphi^\dagger$, and an odd product has zero [vacuum expectation value](../../../../vacuum-expectation-value.md). Terms with no zero-mode factors are independent of $N_0$ at fixed $\theta_k$. Therefore

$$
\boxed{\langle H_{\rm int}\rangle=\frac{uN_0^2}{2V}
+\frac{uN_0}{2V}\sum_{\mathbf k\ne0}
\left[\langle\psi_{\mathbf k}\psi_{-\mathbf k}\rangle
+\langle\psi_{\mathbf k}^\dagger\psi_{-\mathbf k}^\dagger\rangle
+4\langle\psi_{\mathbf k}^\dagger\psi_{\mathbf k}\rangle\right]
+O(N_0^0).}
$$

To evaluate these [vacuum expectation values](../../../../vacuum-expectation-value.md), use the inverse [Bogoliubov transformation](../../../../bogoliubov-transformation.md) and its [Hermitian adjoint](../../../../adjoint-operator.md):

$$
\psi_{\mathbf k}=c_k\varphi_{\mathbf k}-s_k\varphi_{-\mathbf k}^\dagger,
\qquad
\psi_{\mathbf k}^\dagger=c_k\varphi_{\mathbf k}^\dagger-s_k\varphi_{-\mathbf k}.
$$

Since $\varphi_{\mathbf k}|0\rangle=0$, the only nonzero two-factor [vacuum expectation value](../../../../vacuum-expectation-value.md) is $\langle\varphi_{\mathbf k}\varphi_{\mathbf q}^\dagger\rangle=\delta_{\mathbf k,\mathbf q}$. The [bosonic squeezed-vacuum contractions](../../../../bosonic-squeezed-vacuum-contractions.md) are consequently

$$
\boxed{\begin{aligned}
\langle\psi_{\mathbf k}^\dagger\psi_{\mathbf q}\rangle
&=s_k^2\delta_{\mathbf k,\mathbf q},\\
\langle\psi_{\mathbf k}\psi_{\mathbf q}\rangle
&=-c_ks_k\delta_{\mathbf k,-\mathbf q},\\
\langle\psi_{\mathbf k}^\dagger\psi_{\mathbf q}^\dagger\rangle
&=-c_ks_k\delta_{\mathbf k,-\mathbf q}.
\end{aligned}}
$$

In particular the three requested quantities are $-\sinh\theta_k\cosh\theta_k$, $-\sinh\theta_k\cosh\theta_k$ and $\sinh^2\theta_k$, respectively. The minus sign in the pair [vacuum expectation values](../../../../vacuum-expectation-value.md) comes from the inverse [Bogoliubov transformation](../../../../bogoliubov-transformation.md) and is essential to lowering the [interaction energy](../../../../interaction-energy.md). Substitution yields

$$
\boxed{\langle H_{\rm int}\rangle
=\frac{uN_0^2}{2V}+\frac{uN_0}{V}\sum_{\mathbf k\ne0}(2s_k^2-c_ks_k)+O(N_0^0).}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
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
