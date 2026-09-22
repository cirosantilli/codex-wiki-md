<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Arnold-Liouville theorem](../../../../../../liouville-arnold-theorem.md) concerns a connected compact component $L$ of a regular common level of $n$ commuting independent smooth functions $F=(F_1,\ldots,F_n)$ on a $2n$-dimensional [symplectic manifold](../../../../../../symplectic-manifold.md). It states that $L$ is a [Lagrangian torus](../../../../../../lagrangian-torus.md), and that a neighbourhood of $L$ has [action-angle variables](../../../../../../action-angle-variables.md)

$$
(\theta,I)\in\mathbb T^n\times U,\qquad
\omega=\sum_jd\theta_j\wedge dI_j,
$$

in which every $F_i$ depends only on $I$. If $H=F_1$ or, more generally, $H=h(F)$, its [Hamiltonian flow](../../../../../../hamiltonian-flow.md) satisfies

$$
\boxed{\dot I=0,\qquad\dot\theta=\nabla_I H(I).}
$$

Angles have period $2\pi$ here. The theorem is local near this regular compact component; it does not assert globally defined [action-angle variables](../../../../../../action-angle-variables.md) across singular levels or over an entire base with monodromy.

First, $L$ has [dimension of a manifold](../../../../../../dimension-of-a-manifold.md) $n$ by the [submersion theorem](../../../../../../submersion-theorem.md). The [Hamiltonian vector fields](../../../../../../hamiltonian-vector-field.md) $X_{F_i}$ are independent, tangent to $L$, and commute. They span $TL$. Moreover

$$
\omega(X_{F_i},X_{F_j})=dF_i(X_{F_j})=\{F_i,F_j\}=0,
$$

so $L$ is a [Lagrangian submanifold](../../../../../../lagrangian-submanifold.md). Compactness makes these restricted [vector fields](../../../../../../vector-field.md) complete. Their joint flow is an $\mathbb R^n$-action on $L$. Its orbits are open because the fields span $TL$, so connectedness gives one orbit. The stabilizer $\Lambda$ of a point is discrete by the [inverse function theorem](../../../../../../inverse-function-theorem.md), and

$$
L\cong\mathbb R^n/\Lambda.
$$

Compactness forces $\Lambda$ to be a full-rank [Euclidean lattice](../../../../../../euclidean-lattice.md): otherwise an unbounded linear coordinate transverse to its span would descend to the quotient. Thus **$L$ is an $n$-torus**.

Next choose a small ball of regular values near $F(L)$ and a neighbourhood $N$ of this component which is a product family of compact tori $L_c$. This local trivialization follows directly by choosing transverse [vector fields](../../../../../../vector-field.md) $Z_j$ with $dF_i(Z_j)=\delta_{ij}$ and lifting short radial paths in the base; compactness of $L$ gives a uniform neighbourhood where their flows exist. Hence $N$ deformation retracts onto $L$. The commuting joint flows on nearby fibres have smoothly varying full-rank [Hamiltonian period lattices](../../../../../../hamiltonian-period-lattice.md). A basis $t^{(j)}(c)\in\mathbb R^n$ of their periods can be chosen smoothly on this small ball: continue the return equations from a basis at the central fibre, using their nonsingular vertical flow derivatives and the [implicit function theorem](../../../../../../implicit-function-theorem.md). No global choice of lattice basis is needed.

Because $\omega|_L=0$ and $N$ retracts onto $L$, its closed [symplectic form](../../../../../../symplectic-form.md) is exact on $N$. Choose a one-form $\lambda$ with $d\lambda=-\omega$. Let $\gamma_j(c)$ be the smoothly continued cycles represented by the period basis and define the [action integrals](../../../../../../action-integral.md)

$$
I_j(c)=\frac1{2\pi}\int_{\gamma_j(c)}\lambda.
$$

For a transverse variation $v$ of the fibre, differentiating a cycle integral and using [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md) eliminates the integral of the exact term. With the cycle parametrized by the joint-flow time $t^{(j)}$, this gives

$$
dI_j(v)=\frac1{2\pi}\int_{\gamma_j}(-\omega(v,\dot\gamma_j))
=\frac1{2\pi}\sum_i t_i^{(j)}(c)\,dF_i(v).
$$

Thus

$$
\boxed{dI_j=\frac1{2\pi}\sum_i t_i^{(j)}(c)\,dc_i.}
$$

The period matrix is nonsingular, so $I$ gives coordinates on the base. The corresponding [Hamiltonian vector fields](../../../../../../hamiltonian-vector-field.md) satisfy

$$
X_{I_j}=\frac1{2\pi}\sum_i t_i^{(j)}(c)X_{F_i}.
$$

Their time-$2\pi$ flows return along the basis cycles. They commute because each $I_j$ is a function of the commuting $F_i$. Consequently they give a free [torus action](../../../../../../torus-action.md) on $N$.

Choose a section over the action-coordinate ball and use this [torus action](../../../../../../torus-action.md) to define angles $\theta$. Since $X_{I_j}=\partial_{\theta_j}$, the [symplectic form](../../../../../../symplectic-form.md) takes the form

$$
\omega=\sum_jd\theta_j\wedge dI_j+\beta(I).
$$

The closed base two-form $\beta$ is exact on the ball: write $\beta=d\alpha$, $\alpha=\sum_j a_j(I)dI_j$, by the [Poincaré lemma](../../../../../../poincare-lemma.md). Changing the angular origins by $\theta'_j=\theta_j+a_j(I)$ removes this term, since $\sum_jd\theta'_j\wedge dI_j=\omega$. This completes the construction of [action-angle variables](../../../../../../action-angle-variables.md). The functions $F_i$ are constant on the fibres, so are functions of $I$ alone, and [Hamilton's equations](../../../../../../hamilton-s-equations.md) give the claimed straight-line motion. This proves both the topological and symplectic parts of the [Arnold-Liouville theorem](../../../../../../liouville-arnold-theorem.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
