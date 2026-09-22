<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the canonical nonnegative [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) and its [Riemannian heat kernel](../../../../../riemannian-heat-kernel.md) for $t>0$. For the spectral conclusion we use closed compact manifolds, so the operator has a discrete [spectrum](../../../../../spectrum-functional-analysis.md) and a finite [heat trace](../../../../../heat-trace.md). The kernel identity itself can also be formulated for the canonical [Friedrichs extension](../../../../../friedrichs-extension.md) on a noncompact manifold; this specifies the heat operator rather than assuming uniqueness among unrestricted solutions of the [heat equation](../../../../../heat-equation.md).

An [isometry](../../../../../isometry.md) $h$ preserves the Laplacian, its defining quadratic form and therefore its [heat semigroup](../../../../../heat-semigroup.md). Consequently

$$
K_N(hz,hw,t)=K_N(z,w,t).
$$

Set $H(x,y,t)=\sum_{g\in U}K_N(\widetilde x,g\widetilde y,t)$. A different choice of lifts has the form $h\widetilde x,k\widetilde y$ with $h,k\in U$, because the covering is normal. The resulting sum is

$$
\sum_{g\in U}K_N(h\widetilde x,gk\widetilde y,t)=\sum_{g\in U}K_N(\widetilde x,h^{-1}gk\widetilde y,t)=H(x,y,t),
$$

since $g\mapsto h^{-1}gk$ permutes $U$. This proves independence of both lifts. Local smooth sections of the [covering map](../../../../../covering-space.md) then show that $H$ is smooth for positive time. There are finitely many summands, so spatial and time differentiation commute with the sum, and local isometry gives $(\partial_t+\Delta_x)H=0$.

For the integral and initial condition, use the sheet-counting formula

$$
\int_N\psi(z)\,dV_N(z)=\int_M\sum_{p(z)=y}\psi(z)\,dV_M(y).
$$

It follows by dividing the base into measurable pieces lying in evenly covered charts and using the locally isometric inverse branches. For a smooth test function $\phi$ on the base, this formula gives

$$
\int_M H(x,y,t)\phi(y)\,dV_M(y)=\int_NK_N(\widetilde x,z,t)\phi(pz)\,dV_N(z).
$$

On a closed manifold these integrals are finite, and the finite sheet sum entails no convergence exchange. The right side tends to $\phi(p\widetilde x)=\phi(x)$ as $t\downarrow0$ by the initial property of the [Riemannian heat kernel](../../../../../riemannian-heat-kernel.md). Thus $H$ has the correct delta initial condition.

One can identify the operator exactly, also avoiding a noncompact uniqueness issue, by [heat semigroup descent through a finite normal covering](../../../../../heat-semigroup-descent-through-a-finite-normal-covering.md). If $d=|U|$, the map $I\phi=d^{-1/2}\phi\circ p$ is unitary onto the $U$-invariant subspace of $L^2(N)$, because

$$
\|I\phi\|_{L^2(N)}^2=\|\phi\|_{L^2(M)}^2,\qquad \int_N|\nabla I\phi|^2\,dV_N=\int_M|\nabla\phi|^2\,dV_M.
$$

Locally isometric pullback proves the second equality. Smooth compactly supported invariant functions descend, and averaging over the finite group gives the corresponding equality of the closed quadratic-form domains. Hence the [Friedrichs extensions](../../../../../friedrichs-extension.md) and their [heat semigroups](../../../../../heat-semigroup.md) intertwine. The preceding integral is precisely that descended semigroup, proving

$$
\boxed{K_M(x,y,t)=\sum_{g\in U}K_N(\widetilde x,g\widetilde y,t).}
$$

For the noncompact version, finite covering maps are proper, so compactly supported test functions have compactly supported lifts; the same form argument is valid. The canonical heat kernels are sub-Markovian, which bounds integrals against bounded test functions. All operations used above are therefore defined. In particular there is no factor $1/|U|$ in the kernel formula: integrating over the sheets already accounts for its normalization.

Now take a finite ambient group $T$ of [isometries](../../../../../isometry.md) of a closed $N$, and free [Gassmann equivalent](../../../../../gassmann-equivalence.md) subgroups $U_1,U_2$. Define the orbital integral

$$
\Phi_t(g)=\int_NK_N(z,gz,t)\,dV_N(z).
$$

It is finite, and the conjugacy-invariance identity makes it a [class function](../../../../../class-function.md) on $T$. The [heat kernel on a finite isometric quotient](../../../../../heat-kernel-on-a-finite-isometric-quotient.md) and the sheet-counting formula give the quotient [heat traces](../../../../../heat-trace.md)

$$
Z_{M_i}(t)=\frac1{|U_i|}\sum_{g\in U_i}\Phi_t(g).
$$

The averaging factor belongs here, since the cover has $|U_i|$ sheets. By [Gassmann equivalence](../../../../../gassmann-equivalence.md), the two subgroups meet each conjugacy class in the same number of elements, and summing these numbers also gives $|U_1|=|U_2|$. Since $\Phi_t$ is constant on each class, the two [heat traces](../../../../../heat-trace.md) are equal for every $t>0$.

Finally, a discrete nonnegative eigenvalue multiset is determined by its [heat trace](../../../../../heat-trace.md). Its zero multiplicity is $\lim_{t\to\infty}Z(t)$. After subtracting the zero terms, the smallest remaining eigenvalue and its multiplicity are recovered from the leading exponential decay; subtract those terms and repeat. Compactness ensures only finitely many eigenvalues in any bounded interval, so this procedure recovers the entire multiset. We have proved the [Sunada theorem](../../../../../sunada-theorem.md):

$$
\boxed{\operatorname{Spec}(M_1)=\operatorname{Spec}(M_2)\text{ with multiplicities}.}
$$

The closedness assumption is used for this heat-trace deduction; on a general noncompact manifold one cannot replace it by a possibly infinite trace without further analysis.

If the initial manifold is not compact, the same isospectral conclusion can be interpreted for the canonical self-adjoint operators without taking an infinite trace. To see this, decompose the unitary representation of the finite group $T$ as $L^2(N)=\bigoplus_\rho V_\rho\otimes\mathcal H_\rho$, with $V_\rho$ irreducible and $\mathcal H_\rho$ its multiplicity space. Commutation with the group makes the Laplacian act on each summand as $I\otimes D_\rho$, by the [Schur lemma](../../../../../schur-s-lemma.md) applied to its bounded resolvents. The projection onto the $U_i$-invariant factor is $|U_i|^{-1}\sum_{u\in U_i}\rho(u)$, and its trace is therefore $\dim V_\rho^{U_i}=|U_i|^{-1}\sum_{u\in U_i}\chi_\rho(u)$. [Gassmann equivalence](../../../../../gassmann-equivalence.md) makes these dimensions equal. Unitary identifications $V_\rho^{U_1}\to V_\rho^{U_2}$, tensored with the identity on each multiplicity space, intertwine the restricted Laplacians. The normalized pullbacks identify those restrictions with the two quotient operators. This [Sunada unitary equivalence without a finite heat trace](../../../../../sunada-unitary-equivalence-without-a-finite-heat-trace.md) proves equality of their full spectra, including continuous spectrum when present.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
