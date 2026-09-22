<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The form attached to $V$ is $B_V(x,y)=\operatorname{tr}_V(xy)$.** More generally, for a [Lie algebra representation](../../../../../lie-algebra-representation.md) $\rho$, the [Trace form of a Lie algebra representation](../../../../../trace-form-of-a-lie-algebra-representation.md) is

$$
B_V(x,y)=\operatorname{tr}_V(\rho(x)\rho(y)).
$$

The unqualified [Killing form](../../../../../killing-form.md) is the special case of the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md),

$$
B(x,y)=\operatorname{tr}_{\mathfrak g}(\operatorname{ad}x\operatorname{ad}y).
$$

The distinction matters: a [Trace form of a Lie algebra representation](../../../../../trace-form-of-a-lie-algebra-representation.md) can be degenerate even when $\mathfrak g$ is [semisimple](../../../../../semisimple-lie-algebra-split.md), for example on the [trivial Lie algebra representation](../../../../../trivial-lie-algebra-representation.md).

The [Trace form of a Lie algebra representation](../../../../../trace-form-of-a-lie-algebra-representation.md) is [bilinear](../../../../../bilinear-map.md) and symmetric, because $\operatorname{tr}(AB)=\operatorname{tr}(BA)$. It is an [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md):

$$
B_V([x,y],z)=B_V(x,[y,z]).
$$

This follows by expanding both [commutators](../../../../../commutator.md) and cyclically permuting factors under the [matrix trace](../../../../../matrix-trace.md). Equivalently,

$$
B_V([x,y],z)+B_V(y,[x,z])=0.
$$

Its [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md) is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md), since if $B_V(y,-)=0$, then $B_V([x,y],z)=-B_V(y,[x,z])=0$. The [Killing form](../../../../../killing-form.md) is also preserved by every [automorphism of a Lie algebra](../../../../../automorphism-of-a-lie-algebra.md), because the corresponding [adjoint operators](../../../../../adjoint-operator.md) are conjugate. On a complex finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md), the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md) says that the [Killing form](../../../../../killing-form.md) is nondegenerate exactly when the [Lie algebra](../../../../../lie-algebra-split.md) is [semisimple](../../../../../semisimple-lie-algebra-split.md). The [Cartan solvability criterion](../../../../../cartan-solvability-criterion.md) says that $\mathfrak g$ is [solvable](../../../../../solvable-lie-algebra.md) exactly when $B(\mathfrak g,[\mathfrak g,\mathfrak g])=0$.

We next construct the [sl2 subalgebra associated with a root](../../../../../sl2-subalgebra-associated-with-a-root.md). Use the [root-space decomposition](../../../../../root-space-decomposition.md)

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\beta\in\Phi}\mathfrak g_\beta.
$$

For $u\in\mathfrak g_\beta$, $v\in\mathfrak g_\gamma$, invariance of the [Killing form](../../../../../killing-form.md) gives

$$
(\beta(h)+\gamma(h))B(u,v)=0\quad(h\in\mathfrak h).
$$

Thus $B(\mathfrak g_\beta,\mathfrak g_\gamma)=0$ unless $\beta+\gamma=0$, and $B(\mathfrak g_\beta,\mathfrak h)=0$ for nonzero $\beta$. Nondegeneracy of $B$ on $\mathfrak g$ now implies that $-\alpha$ is a [root](../../../../../root-of-a-root-system.md) and that $B$ pairs $\mathfrak g_\alpha$ and $\mathfrak g_{-\alpha}$ nondegenerately.

Nondegeneracy of $B|_{\mathfrak h}$ defines a unique $t_\alpha\in\mathfrak h$ by

$$
B(t_\alpha,h)=\alpha(h)\quad(h\in\mathfrak h).
$$

Choose $x\in\mathfrak g_\alpha$ and $y\in\mathfrak g_{-\alpha}$ with $B(x,y)=1$. Their [Lie bracket](../../../../../lie-bracket.md) lies in the zero [root space](../../../../../root-space.md), namely $\mathfrak h$, and

$$
B([x,y],h)=B(x,[y,h])=\alpha(h)B(x,y)=\alpha(h).
$$

Therefore $[x,y]=t_\alpha$.

The essential [nonisotropic root lemma](../../../../../nonisotropic-root-lemma.md) is that $\alpha(t_\alpha)\ne0$. Suppose instead that it vanished. Then $[t_\alpha,x]=[t_\alpha,y]=0$, so $\langle x,y,t_\alpha\rangle$ would be a [solvable Lie algebra](../../../../../solvable-lie-algebra.md) with [derived algebra](../../../../../derived-algebra.md) $\mathbb Ct_\alpha$. Apply the [Lie theorem](../../../../../lie-s-theorem.md) to its action on $\mathfrak g$ by the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). The [commutator](../../../../../commutator.md) $\operatorname{ad}t_\alpha=[\operatorname{ad}x,\operatorname{ad}y]$ is strictly upper triangular in a suitable [basis](../../../../../basis.md), hence [nilpotent](../../../../../nilpotent-linear-map.md). But $t_\alpha\in\mathfrak h$, so the [root-space decomposition](../../../../../root-space-decomposition.md) makes $\operatorname{ad}t_\alpha$ diagonalizable. A diagonalizable [nilpotent linear map](../../../../../nilpotent-linear-map.md) is zero. Thus $t_\alpha$ is central in $\mathfrak g$. The [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md) of a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) is zero; equivalently a central element lies in the [radical of the Killing form](../../../../../radical-of-the-killing-form.md). This forces $t_\alpha=0$, contradicting $\alpha\ne0$.

Writing $c=\alpha(t_\alpha)$, define

$$
\boxed{X_\alpha=x,\qquad H_\alpha=\frac{2t_\alpha}{c},\qquad Y_\alpha=\frac{2y}{c}.}
$$

The [root-space decomposition](../../../../../root-space-decomposition.md) and $[x,y]=t_\alpha$ give

$$
[H_\alpha,X_\alpha]=2X_\alpha,\qquad [H_\alpha,Y_\alpha]=-2Y_\alpha,\qquad [X_\alpha,Y_\alpha]=H_\alpha.
$$

The three vectors are linearly independent because they lie in the distinct summands $\mathfrak g_\alpha$, $\mathfrak h$, and $\mathfrak g_{-\alpha}$. Their span is therefore a copy of the [sl2 Lie algebra](../../../../../sl2-lie-algebra.md).

**The weight lattice consists of the functionals integral on all coroots.** With $H_\alpha$ the [coroot](../../../../../coroot.md) above, the [weight lattice](../../../../../weight-lattice.md) is

$$
P=\{\lambda\in\mathfrak h^*: \lambda(H_\alpha)\in\mathbb Z\text{ for all }\alpha\in\Phi\}
=\bigoplus_{i=1}^{\ell}\mathbb Z\omega_i,
$$

where the [fundamental weights](../../../../../fundamental-weight.md) satisfy $\omega_i(H_{\alpha_j})=\delta_{ij}$ for the [simple roots](../../../../../simple-root.md) $\alpha_j$. Here $P$ lies in the real span of the [roots](../../../../../root-of-a-root-system.md), viewed inside $\mathfrak h^*$.

The [classification of finite-dimensional sl2 representations](../../../../../classification-of-finite-dimensional-sl2-representations.md) says that every finite-dimensional complex [sl2 Lie algebra](../../../../../sl2-lie-algebra.md) representation is a [direct sum](../../../../../direct-sum.md) of irreducibles $L_m$, $m\in\mathbb Z_{\ge0}$, on which the standard $H$ has [eigenvalues](../../../../../eigenvalue.md) $m,m-2,\ldots,-m$. Restrict any finite-dimensional [Lie algebra representation](../../../../../lie-algebra-representation.md) of $\mathfrak g$ to each [sl2 subalgebra associated with a root](../../../../../sl2-subalgebra-associated-with-a-root.md). If $v$ has [weight](../../../../../weight-representation-theory.md) $\lambda$, then $H_\alpha v=\lambda(H_\alpha)v$, so $\lambda(H_\alpha)$ is an integer. Thus every [weight](../../../../../weight-representation-theory.md) lies in $P$. The same restrictions show that the commuting simple [coroots](../../../../../coroot.md) act diagonalizably, justifying the simultaneous [weight-space decomposition](../../../../../weight-space-decomposition.md).

**For $\mathfrak{sp}(4)$, the roots are $\pm2\varepsilon_1$, $\pm2\varepsilon_2$, and $\pm\varepsilon_1\pm\varepsilon_2$.** Work on $\mathbb C^4$ with the alternating [bilinear form](../../../../../bilinear-form.md) having matrix

$$
J=\begin{pmatrix}0&I_2\\-I_2&0\end{pmatrix}.
$$

The [symplectic Lie algebra](../../../../../symplectic-lie-algebra.md) is

$$
\mathfrak{sp}(4)=\{M:M^TJ+JM=0\}
=\left\{\begin{pmatrix}A&B\\C&-A^T\end{pmatrix}:B=B^T,\ C=C^T\right\}.
$$

Using the [matrix units](../../../../../matrix-unit.md) $E_{ij}$, take the [Cartan subalgebra](../../../../../cartan-subalgebra.md)

$$
\mathfrak h=\langle h_1,h_2\rangle,\qquad h_1=E_{11}-E_{33},\qquad h_2=E_{22}-E_{44}.
$$

Define $\varepsilon_i(a_1h_1+a_2h_2)=a_i$. A regular diagonal element of $\mathfrak h$ has centralizer precisely $\mathfrak h$, and every element of $\mathfrak h$ acts diagonalizably. Thus it is a [Cartan subalgebra](../../../../../cartan-subalgebra.md). The requested Cartan decomposition is the [root-space decomposition](../../../../../root-space-decomposition.md)

$$
\mathfrak{sp}(4)=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathbb CX_\alpha.
$$

Choose [positive roots](../../../../../positive-root.md) $\varepsilon_1-\varepsilon_2$, $2\varepsilon_2$, $\varepsilon_1+\varepsilon_2$, $2\varepsilon_1$. The [symplectic root sl2 triple](../../../../../symplectic-root-sl2-triple.md) are given explicitly by

$$
\begin{array}{c|c|c|c}
\alpha&X_\alpha&H_\alpha&Y_\alpha\\\hline
\varepsilon_1-\varepsilon_2&E_{12}-E_{43}&h_1-h_2&E_{21}-E_{34}\\
\varepsilon_1+\varepsilon_2&E_{14}+E_{23}&h_1+h_2&E_{41}+E_{32}\\
2\varepsilon_1&E_{13}&h_1&E_{31}\\
2\varepsilon_2&E_{24}&h_2&E_{42}
\end{array}
$$

For the negative [root spaces](../../../../../root-space.md), use the corresponding $Y_\alpha$. These eight [root vectors](../../../../../root-vector.md), together with $h_1,h_2$, form a [basis](../../../../../basis.md): the block description above has dimension $4+3+3=10$, and the ten listed vectors are independent. Finally, the [matrix unit](../../../../../matrix-unit.md) identity

$$
[E_{ij},E_{kl}]=\delta_{jk}E_{il}-\delta_{li}E_{kj}
$$

verifies $[X_\alpha,Y_\alpha]=H_\alpha$ for every row. The diagonal differences verify $[H_\alpha,X_\alpha]=2X_\alpha$ and $[H_\alpha,Y_\alpha]=-2Y_\alpha$. Thus each row supplies a [basis](../../../../../basis.md) of the required [sl2 subalgebra associated with a root](../../../../../sl2-subalgebra-associated-with-a-root.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
