<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Fredholm Kuranishi reduction](../../../../../../fredholm-kuranishi-reduction.md) has the following form. Let $F$ be a smooth map between real Hilbert spaces with $F(0)=0$ whose derivative $L=DF(0)$ is a [Fredholm operator](../../../../../../fredholm-operator.md). Split the source as $K\oplus V$, where $K=\ker L$, and the target as $R\oplus C$, where $R=\operatorname{im}L$ and $C$ represents the finite-dimensional cokernel. The restriction $L:V\to R$ is a bounded isomorphism. The [implicit function theorem](../../../../../../implicit-function-theorem.md) applied to $P_RF(k+v)=0$ solves it uniquely near zero as $v=v(k)$, with $v(0)=Dv(0)=0$. Thus

$$
\kappa(k)=P_CF(k+v(k)),\qquad
\kappa:K\longrightarrow C,\qquad
\kappa(0)=D\kappa(0)=0,
$$

is a smooth finite-dimensional obstruction map, and **the local zero set of $F$ is the graph over $\kappa^{-1}(0)$**. If a compact group acts preserving the problem, average inner products to choose invariant splittings; uniqueness in the [implicit function theorem](../../../../../../implicit-function-theorem.md) makes the construction equivariant.

Apply this to the [vector-bundle curvature](../../../../../../curvature-form.md) equation near $A$. Complete connections in $L^2_\ell$ and the [unitary bundle gauge group](../../../../../../unitary-bundle-gauge-group.md) in $L^2_{\ell+1}$ with integer $\ell\geq3$, so the required multiplication and gauge operations are smooth. The [Coulomb slice for unitary connections](../../../../../../coulomb-slice-for-unitary-connections.md) imposes $d_A^*a=0$. Its local existence follows from the gauge-fixing equation: the derivative in the gauge direction is $d_A^*d_A$, invertible on the orthogonal complement of its parallel kernel by the elliptic estimate. The local slice theorem then says that its remaining identifications are precisely by $\operatorname{Stab}(A)$.

On this slice the equation is

$$
F_{A+a}^+=d_A^+a+(a\wedge a)^+=0.
$$

Its kernel is the harmonic representative space $H_A^1$, and its cokernel is $H_A^2$. The hypothesis $H_A^2=0$ makes the obstruction target zero. Therefore the solutions near $A$ are an equivariant smooth graph over $H_A^1$, and the gauge-orbit neighborhood is a neighborhood of zero in $H_A^1/\operatorname{Stab}(A)$.

It remains to compute this representation, not just its dimension. A [reducible SU2 connection](../../../../../../reducible-su2-connection.md) with circle holonomy preserves $E=L\oplus L^{-1}$. In this splitting,

$$
\operatorname{ad}E\cong\underline{\mathbb R}\oplus(L^2)_{\mathbb R},\qquad
\begin{pmatrix}it&z\\-\overline z&-it\end{pmatrix}
\longleftrightarrow(t,z).
$$

The diagonal part is a trivial real connection. Its degree-one deformation space is the space of ordinary harmonic one-forms. To check this directly, if $d^*a=0$ and $d^+a=0$, then $da$ is an exact [anti-self-dual two-form](../../../../../../anti-self-dual-differential-form.md). [Stokes theorem](../../../../../../stokes-theorem.md) gives

$$
\|da\|_2^2=-\int_Xda\wedge da=-\int_Xd(a\wedge da)=0,
$$

so $da=0$ and $a$ is harmonic. This neutral deformation space vanishes because $b_1(X)=0$. Hence all of $H_A^1$ is in the off-diagonal part, where the complex structure of $L^2$ commutes with both operators; it is a complex vector space.

Using part (a), part (b), and $H_A^2=0$,

$$
\dim_{\mathbb R}H_A^1=\operatorname{ind}D_A+\dim H_A^0
=8e(E)-2,
\qquad
\boxed{d=\dim_{\mathbb C}H_A^1=4e(E)-1.}
$$

Parameterize the stabilizer by $u_\lambda=\operatorname{diag}(\lambda^{-1},\lambda)$, with $\lambda\in S^1$. Under our convention $A^u=u^{-1}Au+u^{-1}du$, its action on an off-diagonal perturbation is

$$
\begin{pmatrix}0&z\\-\overline z&0\end{pmatrix}
\longmapsto
\begin{pmatrix}0&\lambda^2z\\-\overline{\lambda^2z}&0\end{pmatrix}.
$$

Consequently the equivariant graph identifies a neighborhood of $[A]$ with a neighborhood of the origin in

$$
\boxed{\mathbb C^{\,4e(E)-1}/S^1,\qquad \lambda\cdot z=\lambda^2z.}
$$

This proves the exact scalar weight requested, with a stabilizer parametrization consistent with the chosen gauge convention. The ineffective kernel is $\{\pm1\}$. The orbit space is also the cone on $\mathbb{CP}^{d-1}$, because the weight-two circle has the same nonzero orbits as the ordinary scalar circle. This is the [local cone at an unobstructed reducible SU2 instanton](../../../../../../local-cone-at-an-unobstructed-reducible-su2-instanton.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
