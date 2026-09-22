# Paper 102

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_102.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_102.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

**Over the complex numbers, every finite-dimensional representation of a solvable Lie algebra has a basis in which every representing matrix is upper triangular.** The [Lie theorem](../../../lie-algebra.md#lie-s-theorem) is often stated first as the existence of a common [eigenvector](../../../linear-operator-theory.md#eigenvector) in every nonzero finite-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) of a [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra). Applying that assertion successively to [quotient representations](../../../representation-theory.md#quotient-representation) gives an invariant [complete flag](../../../vector-space.md#complete-flag), and hence the upper triangular form. The same proof works over any [algebraically closed field](../../../algebra.md#algebraically-closed-field) of [characteristic zero](../../../algebra.md#characteristic-zero).

We prove the common [eigenvector](../../../linear-operator-theory.md#eigenvector) assertion by induction on $\dim\mathfrak g$, writing the action as $av$. The zero [Lie algebra](../../../lie-algebra.md) is immediate. If $\mathfrak g\ne0$ is [solvable](../../../lie-algebra.md#solvable-lie-algebra), its [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) shows that $[\mathfrak g,\mathfrak g]\ne\mathfrak g$. Choose a codimension-one [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) $\mathfrak a$ containing $[\mathfrak g,\mathfrak g]$, and choose $x\notin\mathfrak a$. By induction there are $v\ne0$ and a [linear functional](../../../linear-algebra.md#linear-functional) $\lambda:\mathfrak a\to\mathbb C$ such that $av=\lambda(a)v$ for all $a\in\mathfrak a$.

Let $W$ be the span of $v,xv,x^2v,\ldots$. If $m=\dim W$, the first $m$ of these vectors form a [basis](../../../vector-space.md#basis), and $W$ is $x$-invariant. We claim that for each $a\in\mathfrak a$,

$$
a x^jv=\lambda(a)x^jv+\operatorname{span}\{v,xv,\ldots,x^{j-1}v\}.
$$

For $j=0$ this is the definition of $v$. For the induction step, use $ax=x a+[a,x]$ and $[a,x]\in\mathfrak a$. Applying the induction hypothesis to both $a$ and $[a,x]$ proves the claim. Consequently $W$ is $\mathfrak a$-invariant, and every $a\in\mathfrak a$ acts on $W$ by an upper triangular [matrix](../../../vector-space.md#matrix) with all diagonal entries $\lambda(a)$.

Since both $x$ and $a$ preserve $W$, the [matrix trace](../../../linear-algebra.md#matrix-trace) of their [commutator](../../../lie-algebra.md#commutator) on $W$ is zero. The claim applied to $[x,a]\in\mathfrak a$ gives

$$
0=\operatorname{tr}_W[x,a]=m\lambda([x,a]).
$$

Here [characteristic zero](../../../algebra.md#characteristic-zero) is essential: $m\ne0$ in the field, so $\lambda([x,a])=0$. Now the common [weight space](../../../semisimple-lie-algebra.md#weight-space)

$$
E_\lambda=\{w\in V:aw=\lambda(a)w\text{ for all }a\in\mathfrak a\}
$$

is nonzero and $x$-invariant. Indeed, for $w\in E_\lambda$,

$$
a(xw)=x(aw)+[a,x]w=\lambda(a)xw+\lambda([a,x])w=\lambda(a)xw.
$$

An endomorphism of a nonzero finite-dimensional complex [vector space](../../../vector-space.md) has an [eigenvector](../../../linear-operator-theory.md#eigenvector), so choose an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $x$ in $E_\lambda$. It is a common [eigenvector](../../../linear-operator-theory.md#eigenvector) for $\mathfrak g=\mathfrak a+\mathbb Cx$. This proves the [Lie theorem](../../../lie-algebra.md#lie-s-theorem).

**For the printed matrices in characteristic $p$, $[x,y]=x$, and there is no common eigenvector.** Index the standard [basis](../../../vector-space.md#basis) by $e_0,\ldots,e_{p-1}$. The cyclic entry in the PDF gives

$$
x e_j=e_{j-1}\quad(j\text{ modulo }p),\qquad ye_j=je_j.
$$

The $p$ diagonal [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $y$ are distinct in $k$. Thus every [eigenvector](../../../linear-operator-theory.md#eigenvector) of $y$ is a scalar multiple of a single $e_j$. Since $p\ge2$, $xe_j$ is never a scalar multiple of $e_j$, proving the assertion even when $k$ is not an [algebraically closed field](../../../algebra.md#algebraically-closed-field).

For $1\le j\le p-1$,

$$
[x,y]e_j=j e_{j-1}-(j-1)e_{j-1}=e_{j-1}.
$$

At the cyclic boundary,

$$
[x,y]e_0=-(p-1)e_{p-1}=e_{p-1}.
$$

Hence $[x,y]=x$. The two-dimensional [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) $kx+ky$ has [derived algebra](../../../lie-algebra.md#derived-algebra) $kx$, whose own [derived algebra](../../../lie-algebra.md#derived-algebra) is zero, so it is [solvable](../../../lie-algebra.md#solvable-lie-algebra). It nevertheless has no common [eigenvector](../../../linear-operator-theory.md#eigenvector), including after extending $k$ to its [algebraic closure](../../../algebra.md#algebraic-closure). This is a [failure of Lie theorem in positive characteristic](../../../lie-algebra.md#failure-of-lie-theorem-in-positive-characteristic). In the proof above, the obstruction is precisely that $\dim W=p$ can vanish as a scalar in $k$.

**The derived algebra of a complex solvable Lie algebra is nilpotent.** First suppose $\mathfrak g\subseteq\mathfrak{gl}(V)$. By the [Lie theorem](../../../lie-algebra.md#lie-s-theorem), put every element of $\mathfrak g$ in upper triangular form. The diagonal of a [commutator](../../../lie-algebra.md#commutator) of upper triangular [matrices](../../../vector-space.md#matrix) is zero, so $\mathfrak d=[\mathfrak g,\mathfrak g]$ consists of strictly upper triangular [matrices](../../../vector-space.md#matrix). The [Lie algebra](../../../lie-algebra.md) of all such [matrices](../../../vector-space.md#matrix) is a [nilpotent Lie algebra](../../../lie-algebra.md#nilpotent-lie-algebra): if $F_r$ consists of [matrices](../../../vector-space.md#matrix) whose entries vanish whenever $j-i<r$, then

$$
[F_r,F_s]\subseteq F_{r+s},\qquad F_{\dim V}=0.
$$

Therefore the [lower central series of a Lie algebra](../../../lie-algebra.md#lower-central-series-of-a-lie-algebra) of $\mathfrak d$ reaches zero. Alternatively, every element of $\mathfrak d$ is a [nilpotent linear map](../../../linear-operator-theory.md#nilpotent-linear-map), and the [Engel theorem](../../../lie-algebra.md#engel-s-theorem) states that a finite-dimensional [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) consisting of [nilpotent linear maps](../../../linear-operator-theory.md#nilpotent-linear-map) is a [nilpotent Lie algebra](../../../lie-algebra.md#nilpotent-lie-algebra).

For an abstract complex [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra) $\mathfrak g$, apply the preceding result to its [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). The [Lie algebra](../../../lie-algebra.md) $\operatorname{ad}\mathfrak d=[\operatorname{ad}\mathfrak g,\operatorname{ad}\mathfrak g]$ is [nilpotent](../../../lie-algebra.md#nilpotent-lie-algebra). Since $\ker(\operatorname{ad}|_{\mathfrak d})=\mathfrak d\cap Z(\mathfrak g)$ is central in $\mathfrak d$, some term of the [lower central series of a Lie algebra](../../../lie-algebra.md#lower-central-series-of-a-lie-algebra) of $\mathfrak d$ lies in that central [ideal](../../../commutative-algebra.md#ideal); the next term is zero. Thus $\mathfrak d$ itself is [nilpotent](../../../lie-algebra.md#nilpotent-lie-algebra).

Conversely, every [nilpotent Lie algebra](../../../lie-algebra.md#nilpotent-lie-algebra) is [solvable](../../../lie-algebra.md#solvable-lie-algebra), since its [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) is contained term by term in its [lower central series of a Lie algebra](../../../lie-algebra.md#lower-central-series-of-a-lie-algebra). If $\mathfrak d$ is [nilpotent](../../../lie-algebra.md#nilpotent-lie-algebra), it is therefore [solvable](../../../lie-algebra.md#solvable-lie-algebra), and $\mathfrak g/\mathfrak d$ is [Abelian](../../../group.md#abelian-group). More directly, the [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) of $\mathfrak g$, after its first term, is the [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) of $\mathfrak d$. Consequently the [derived algebra nilpotence criterion](../../../lie-algebra.md#derived-algebra-nilpotence-criterion) is

$$
\boxed{\mathfrak g\text{ solvable}\quad\Longleftrightarrow\quad[\mathfrak g,\mathfrak g]\text{ nilpotent}.}
$$

## 2

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**The form attached to $V$ is $B_V(x,y)=\operatorname{tr}_V(xy)$.** More generally, for a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) $\rho$, the [Trace form of a Lie algebra representation](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation) is

$$
B_V(x,y)=\operatorname{tr}_V(\rho(x)\rho(y)).
$$

The unqualified [Killing form](../../../lie-algebra.md#killing-form) is the special case of the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra),

$$
B(x,y)=\operatorname{tr}_{\mathfrak g}(\operatorname{ad}x\operatorname{ad}y).
$$

The distinction matters: a [Trace form of a Lie algebra representation](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation) can be degenerate even when $\mathfrak g$ is [semisimple](../../../semisimple-lie-algebra.md), for example on the [trivial Lie algebra representation](../../../lie-algebra.md#trivial-lie-algebra-representation).

The [Trace form of a Lie algebra representation](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation) is [bilinear](../../../linear-algebra.md#bilinear-map) and symmetric, because $\operatorname{tr}(AB)=\operatorname{tr}(BA)$. It is an [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra):

$$
B_V([x,y],z)=B_V(x,[y,z]).
$$

This follows by expanding both [commutators](../../../lie-algebra.md#commutator) and cyclically permuting factors under the [matrix trace](../../../linear-algebra.md#matrix-trace). Equivalently,

$$
B_V([x,y],z)+B_V(y,[x,z])=0.
$$

Its [radical of a bilinear form](../../../linear-algebra.md#radical-of-a-bilinear-form) is an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra), since if $B_V(y,-)=0$, then $B_V([x,y],z)=-B_V(y,[x,z])=0$. The [Killing form](../../../lie-algebra.md#killing-form) is also preserved by every [automorphism of a Lie algebra](../../../lie-algebra.md#automorphism-of-a-lie-algebra), because the corresponding [adjoint operators](../../../hilbert-space.md#adjoint-operator) are conjugate. On a complex finite-dimensional [Lie algebra](../../../lie-algebra.md), the [Cartan criterion for semisimplicity](../../../lie-algebra.md#cartan-criterion-for-semisimplicity) says that the [Killing form](../../../lie-algebra.md#killing-form) is nondegenerate exactly when the [Lie algebra](../../../lie-algebra.md) is [semisimple](../../../semisimple-lie-algebra.md). The [Cartan solvability criterion](../../../lie-algebra.md#cartan-solvability-criterion) says that $\mathfrak g$ is [solvable](../../../lie-algebra.md#solvable-lie-algebra) exactly when $B(\mathfrak g,[\mathfrak g,\mathfrak g])=0$.

We next construct the [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root). Use the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition)

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\beta\in\Phi}\mathfrak g_\beta.
$$

For $u\in\mathfrak g_\beta$, $v\in\mathfrak g_\gamma$, invariance of the [Killing form](../../../lie-algebra.md#killing-form) gives

$$
(\beta(h)+\gamma(h))B(u,v)=0\quad(h\in\mathfrak h).
$$

Thus $B(\mathfrak g_\beta,\mathfrak g_\gamma)=0$ unless $\beta+\gamma=0$, and $B(\mathfrak g_\beta,\mathfrak h)=0$ for nonzero $\beta$. Nondegeneracy of $B$ on $\mathfrak g$ now implies that $-\alpha$ is a [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) and that $B$ pairs $\mathfrak g_\alpha$ and $\mathfrak g_{-\alpha}$ nondegenerately.

Nondegeneracy of $B|_{\mathfrak h}$ defines a unique $t_\alpha\in\mathfrak h$ by

$$
B(t_\alpha,h)=\alpha(h)\quad(h\in\mathfrak h).
$$

Choose $x\in\mathfrak g_\alpha$ and $y\in\mathfrak g_{-\alpha}$ with $B(x,y)=1$. Their [Lie bracket](../../../lie-algebra.md#lie-bracket) lies in the zero [root space](../../../semisimple-lie-algebra.md#root-space), namely $\mathfrak h$, and

$$
B([x,y],h)=B(x,[y,h])=\alpha(h)B(x,y)=\alpha(h).
$$

Therefore $[x,y]=t_\alpha$.

The essential [nonisotropic root lemma](../../../semisimple-lie-algebra.md#nonisotropic-root-lemma) is that $\alpha(t_\alpha)\ne0$. Suppose instead that it vanished. Then $[t_\alpha,x]=[t_\alpha,y]=0$, so $\langle x,y,t_\alpha\rangle$ would be a [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra) with [derived algebra](../../../lie-algebra.md#derived-algebra) $\mathbb Ct_\alpha$. Apply the [Lie theorem](../../../lie-algebra.md#lie-s-theorem) to its action on $\mathfrak g$ by the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). The [commutator](../../../lie-algebra.md#commutator) $\operatorname{ad}t_\alpha=[\operatorname{ad}x,\operatorname{ad}y]$ is strictly upper triangular in a suitable [basis](../../../vector-space.md#basis), hence [nilpotent](../../../linear-operator-theory.md#nilpotent-linear-map). But $t_\alpha\in\mathfrak h$, so the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) makes $\operatorname{ad}t_\alpha$ diagonalizable. A diagonalizable [nilpotent linear map](../../../linear-operator-theory.md#nilpotent-linear-map) is zero. Thus $t_\alpha$ is central in $\mathfrak g$. The [center of a Lie algebra](../../../lie-algebra.md#center-of-a-lie-algebra) of a [semisimple Lie algebra](../../../semisimple-lie-algebra.md) is zero; equivalently a central element lies in the [radical of the Killing form](../../../lie-algebra.md#radical-of-the-killing-form). This forces $t_\alpha=0$, contradicting $\alpha\ne0$.

Writing $c=\alpha(t_\alpha)$, define

$$
\boxed{X_\alpha=x,\qquad H_\alpha=\frac{2t_\alpha}{c},\qquad Y_\alpha=\frac{2y}{c}.}
$$

The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) and $[x,y]=t_\alpha$ give

$$
[H_\alpha,X_\alpha]=2X_\alpha,\qquad [H_\alpha,Y_\alpha]=-2Y_\alpha,\qquad [X_\alpha,Y_\alpha]=H_\alpha.
$$

The three vectors are linearly independent because they lie in the distinct summands $\mathfrak g_\alpha$, $\mathfrak h$, and $\mathfrak g_{-\alpha}$. Their span is therefore a copy of the [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra).

**The weight lattice consists of the functionals integral on all coroots.** With $H_\alpha$ the [coroot](../../../semisimple-lie-algebra.md#coroot) above, the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) is

$$
P=\{\lambda\in\mathfrak h^*: \lambda(H_\alpha)\in\mathbb Z\text{ for all }\alpha\in\Phi\}
=\bigoplus_{i=1}^{\ell}\mathbb Z\omega_i,
$$

where the [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) satisfy $\omega_i(H_{\alpha_j})=\delta_{ij}$ for the [simple roots](../../../semisimple-lie-algebra.md#simple-root) $\alpha_j$. Here $P$ lies in the real span of the [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system), viewed inside $\mathfrak h^*$.

The [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations) says that every finite-dimensional complex [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) representation is a [direct sum](../../../vector-space.md#direct-sum) of irreducibles $L_m$, $m\in\mathbb Z_{\ge0}$, on which the standard $H$ has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $m,m-2,\ldots,-m$. Restrict any finite-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) of $\mathfrak g$ to each [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root). If $v$ has [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $\lambda$, then $H_\alpha v=\lambda(H_\alpha)v$, so $\lambda(H_\alpha)$ is an integer. Thus every [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) lies in $P$. The same restrictions show that the commuting simple [coroots](../../../semisimple-lie-algebra.md#coroot) act diagonalizably, justifying the simultaneous [weight-space decomposition](../../../semisimple-lie-algebra.md#weight-space-decomposition).

**For $\mathfrak{sp}(4)$, the roots are $\pm2\varepsilon_1$, $\pm2\varepsilon_2$, and $\pm\varepsilon_1\pm\varepsilon_2$.** Work on $\mathbb C^4$ with the alternating [bilinear form](../../../linear-algebra.md#bilinear-form) having matrix

$$
J=\begin{pmatrix}0&I_2\\-I_2&0\end{pmatrix}.
$$

The [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra) is

$$
\mathfrak{sp}(4)=\{M:M^TJ+JM=0\}
=\left\{\begin{pmatrix}A&B\\C&-A^T\end{pmatrix}:B=B^T,\ C=C^T\right\}.
$$

Using the [matrix units](../../../vector-space.md#matrix-unit) $E_{ij}$, take the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra)

$$
\mathfrak h=\langle h_1,h_2\rangle,\qquad h_1=E_{11}-E_{33},\qquad h_2=E_{22}-E_{44}.
$$

Define $\varepsilon_i(a_1h_1+a_2h_2)=a_i$. A regular diagonal element of $\mathfrak h$ has centralizer precisely $\mathfrak h$, and every element of $\mathfrak h$ acts diagonalizably. Thus it is a [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra). The requested Cartan decomposition is the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition)

$$
\mathfrak{sp}(4)=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathbb CX_\alpha.
$$

Choose [positive roots](../../../semisimple-lie-algebra.md#positive-root) $\varepsilon_1-\varepsilon_2$, $2\varepsilon_2$, $\varepsilon_1+\varepsilon_2$, $2\varepsilon_1$. The [symplectic root sl2 triple](../../../semisimple-lie-algebra.md#symplectic-root-sl2-triple) are given explicitly by

$$
\begin{array}{c|c|c|c}
\alpha&X_\alpha&H_\alpha&Y_\alpha\\\hline
\varepsilon_1-\varepsilon_2&E_{12}-E_{43}&h_1-h_2&E_{21}-E_{34}\\
\varepsilon_1+\varepsilon_2&E_{14}+E_{23}&h_1+h_2&E_{41}+E_{32}\\
2\varepsilon_1&E_{13}&h_1&E_{31}\\
2\varepsilon_2&E_{24}&h_2&E_{42}
\end{array}
$$

For the negative [root spaces](../../../semisimple-lie-algebra.md#root-space), use the corresponding $Y_\alpha$. These eight [root vectors](../../../semisimple-lie-algebra.md#root-vector), together with $h_1,h_2$, form a [basis](../../../vector-space.md#basis): the block description above has dimension $4+3+3=10$, and the ten listed vectors are independent. Finally, the [matrix unit](../../../vector-space.md#matrix-unit) identity

$$
[E_{ij},E_{kl}]=\delta_{jk}E_{il}-\delta_{li}E_{kj}
$$

verifies $[X_\alpha,Y_\alpha]=H_\alpha$ for every row. The diagonal differences verify $[H_\alpha,X_\alpha]=2X_\alpha$ and $[H_\alpha,Y_\alpha]=-2Y_\alpha$. Thus each row supplies a [basis](../../../vector-space.md#basis) of the required [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root).

## 3

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

**Schur's lemma says that a nonzero intertwiner between irreducible representations is an isomorphism; over $\mathbb C$, every endomorphism of a finite-dimensional irreducible representation is scalar.** To prove the [Schur lemma](../../../representation-theory.md#schur-s-lemma), let $T:V\to W$ be a [intertwining operator](../../../representation-theory.md#intertwining-operator) between [irreducible representations](../../../representation-theory.md#irreducible-representation). Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and [image of a linear map](../../../vector-space.md#image-of-a-linear-map) are invariant. If $T\ne0$, irreducibility forces $\ker T=0$ and $\operatorname{im}T=W$. This proves the first assertion over any field. In particular the endomorphisms of an [irreducible representation](../../../representation-theory.md#irreducible-representation) form a [division ring](../../../commutative-algebra.md#division-ring).

When $V$ is finite-dimensional over an [algebraically closed field](../../../algebra.md#algebraically-closed-field), an endomorphism $T$ has an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$. The endomorphism $T-\lambda I$ has nonzero [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). By the first assertion it must be zero, so $T=\lambda I$. Consequently, for complex finite-dimensional [irreducible representations](../../../representation-theory.md#irreducible-representation), the space of [intertwining operators](../../../representation-theory.md#intertwining-operator) has dimension zero for nonisomorphic representations and dimension one for isomorphic representations.

**Every finite-dimensional representation of a complex semisimple Lie algebra is completely reducible.** We prove the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) using the allowed [Casimir operator](../../../semisimple-lie-algebra.md#casimir-element) facts, without assuming a splitting in advance. For dual [bases](../../../vector-space.md#basis) $x_i,x^i$ with respect to the [Killing form](../../../lie-algebra.md#killing-form), the [Casimir element](../../../semisimple-lie-algebra.md#casimir-element)

$$
\Omega=\sum_i x_i x^i\in U(\mathfrak g)
$$

is central in the [universal enveloping algebra](../../../lie-algebra.md#universal-enveloping-algebra). Hence its [Casimir operator](../../../semisimple-lie-algebra.md#casimir-element) $C_M=\sum_i\rho_M(x_i)\rho_M(x^i)$ commutes with the action on every [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) $M$ and is compatible with [subrepresentations](../../../representation-theory.md#subrepresentation), [quotient representations](../../../representation-theory.md#quotient-representation), and [intertwining operators](../../../representation-theory.md#intertwining-operator). On the [trivial Lie algebra representation](../../../lie-algebra.md#trivial-lie-algebra-representation) it acts by zero. On every nontrivial finite-dimensional [Irreducible Lie algebra representation](../../../lie-algebra.md#irreducible-lie-algebra-representation) it acts by a nonzero scalar.

For clarity, the last fact can be expressed by the [Casimir eigenvalue](../../../semisimple-lie-algebra.md#casimir-eigenvalue) formula: on an irreducible with [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight) $\lambda$, the scalar is $(\lambda,\lambda+2\rho)$, with the inner product induced by the [Killing form](../../../lie-algebra.md#killing-form) and $\rho$ the [half-sum of positive roots](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots). On the real span of the [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) this inner product is positive definite, and the scalar is positive for $\lambda\ne0$. For a [semisimple Lie algebra](../../../semisimple-lie-algebra.md) with several simple factors the scalars add, so a nontrivial representation still gives a nonzero scalar. These are properties of the [Casimir operator](../../../semisimple-lie-algebra.md#casimir-element) being used here.

First establish [Casimir splitting of a trivial quotient](../../../semisimple-lie-algebra.md#casimir-splitting-of-a-trivial-quotient). Suppose

$$
0\longrightarrow N\longrightarrow E\overset{q}{\longrightarrow}\mathbb C\longrightarrow0
$$

is a [short exact sequence](../../../module-theory.md#short-exact-sequence) of finite-dimensional [Lie algebra representations](../../../lie-algebra.md#lie-algebra-representation), with trivial quotient. The [generalized eigenspaces](../../../linear-operator-theory.md#generalized-eigenspace) of $C_E$ are invariant, so

$$
E=E_0\oplus\bigoplus_{c\ne0}E_c.
$$

Each $E_c$ with $c\ne0$ maps to zero under $q$: applying a sufficiently large power of $C_E-cI$ and using $C_{\mathbb C}=0$ gives $(-c)^r q(e)=0$. Thus $q(E_0)=\mathbb C$.

Take a [composition series of a module](../../../module-theory.md#composition-series-of-a-module) of $E_0$. The [Casimir operator](../../../semisimple-lie-algebra.md#casimir-element) is nilpotent on $E_0$, so its scalar on every irreducible [composition factor](../../../module-theory.md#composition-factor) is zero. The stated [Casimir operator](../../../semisimple-lie-algebra.md#casimir-element) property makes every such factor trivial. In a [basis](../../../vector-space.md#basis) adapted to the [composition series of a module](../../../module-theory.md#composition-series-of-a-module), the image of $\mathfrak g$ on $E_0$ therefore consists of strictly upper triangular [matrices](../../../vector-space.md#matrix), so that image is [solvable](../../../lie-algebra.md#solvable-lie-algebra). The allowed fact that a [semisimple Lie algebra](../../../semisimple-lie-algebra.md) acts trivially on every one-dimensional representation implies that $\mathfrak g$ is a [perfect Lie algebra](../../../semisimple-lie-algebra.md#perfect-lie-algebra): otherwise a nonzero [linear functional](../../../linear-algebra.md#linear-functional) on $\mathfrak g/[\mathfrak g,\mathfrak g]$ would define a nontrivial one-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). Thus $\mathfrak g=[\mathfrak g,\mathfrak g]$, and its image is consequently a [perfect Lie algebra](../../../semisimple-lie-algebra.md#perfect-lie-algebra) too. A [perfect Lie algebra](../../../semisimple-lie-algebra.md#perfect-lie-algebra) that is also a [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra) is zero, since its [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) is constant until it vanishes. Hence $\mathfrak g$ acts trivially on $E_0$. Choose $e\in E_0$ with $q(e)=1$. The map $1\mapsto e$ is an invariant section, proving the [split short exact sequence](../../../module-theory.md#split-short-exact-sequence) assertion.

Now let $W\subseteq V$ be any nonzero [subrepresentation](../../../representation-theory.md#subrepresentation). On the [Hom representation](../../../lie-algebra.md#hom-representation) $\operatorname{Hom}(V,W)$ the action is

$$
(x\cdot f)(v)=x f(v)-f(xv).
$$

Consider the invariant subspace

$$
E=\{f\in\operatorname{Hom}(V,W):f|_W\in\mathbb C I_W\}.
$$

Restriction produces a [short exact sequence](../../../module-theory.md#short-exact-sequence)

$$
0\longrightarrow\operatorname{Hom}(V/W,W)\longrightarrow E\longrightarrow\mathbb C I_W\longrightarrow0.
$$

Surjectivity follows by extending $I_W$ to a linear map on $V$. The quotient is trivial, because $I_W$ commutes with the action on $W$. The preceding [Casimir splitting of a trivial quotient](../../../semisimple-lie-algebra.md#casimir-splitting-of-a-trivial-quotient) yields an invariant $p:V\to W$ with $p|_W=I_W$. Thus

$$
V=W\oplus\ker p,
$$

and $\ker p$ is invariant. The zero [subrepresentation](../../../representation-theory.md#subrepresentation) also has a complement. Repeatedly splitting off an irreducible [subrepresentation](../../../representation-theory.md#subrepresentation) now gives a [direct sum](../../../vector-space.md#direct-sum) of irreducibles, proving the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem).

A [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra) is a linear map $D:\mathfrak g\to\mathfrak g$ satisfying the [Leibniz rule](../../../calculus.md#leibniz-rule)

$$
D[x,y]=[Dx,y]+[x,Dy].
$$

The space $\operatorname{Der}(\mathfrak g)$ is a [vector subspace](../../../vector-space.md#vector-subspace) of $\operatorname{End}(\mathfrak g)$. Equip it with the [commutator](../../../lie-algebra.md#commutator) $[D,E]=DE-ED$. Expanding the [Leibniz rule](../../../calculus.md#leibniz-rule) twice gives

$$
\begin{aligned}
DE[x,y]&=[DEx,y]+[Ex,Dy]+[Dx,Ey]+[x,DEy],\\
ED[x,y]&=[EDx,y]+[Dx,Ey]+[Ex,Dy]+[x,EDy].
\end{aligned}
$$

Subtracting proves that $[D,E]$ is again a [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra). Antisymmetry and the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) hold for the [commutator](../../../lie-algebra.md#commutator) in every associative endomorphism algebra, so this defines the [derivation Lie algebra](../../../lie-algebra.md#derivation-lie-algebra).

The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) says that $\operatorname{ad}x$ is a [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra). Moreover, for $D\in\operatorname{Der}(\mathfrak g)$,

$$
[D,\operatorname{ad}x](y)=D[x,y]-[x,Dy]=[Dx,y],
$$

so

$$
\boxed{[D,\operatorname{ad}x]=\operatorname{ad}(Dx).}
$$

This makes $\operatorname{ad}\mathfrak g$ an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) in $\operatorname{Der}(\mathfrak g)$.

Finally suppose $\mathfrak g$ is [semisimple](../../../semisimple-lie-algebra.md). Let $\mathfrak g$ act on $\operatorname{Der}(\mathfrak g)$ by $x\cdot D=[\operatorname{ad}x,D]$. The [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) supplies an invariant complement $M$ to $\operatorname{ad}\mathfrak g$. For $D\in M$, invariance gives $[\operatorname{ad}x,D]\in M$, while the [ideal](../../../commutative-algebra.md#ideal) identity above gives $[\operatorname{ad}x,D]\in\operatorname{ad}\mathfrak g$. Their intersection is zero, so $\operatorname{ad}(Dx)=0$ for every $x$. The [center of a Lie algebra](../../../lie-algebra.md#center-of-a-lie-algebra) of a [semisimple Lie algebra](../../../semisimple-lie-algebra.md) is zero, hence $Dx=0$ for every $x$, and $M=0$. Therefore

$$
\boxed{\operatorname{Der}(\mathfrak g)=\operatorname{ad}\mathfrak g.}
$$

Every [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra) is inner, and the element giving it is unique because the [center of a Lie algebra](../../../lie-algebra.md#center-of-a-lie-algebra) vanishes.

## 4

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Start with the [tensor product of Lie algebra representations](../../../lie-algebra.md#tensor-product-of-lie-algebra-representations), whose action is

$$
x\cdot(v\otimes w)=(xv)\otimes w+v\otimes(xw).
$$

Writing $T_x=\rho(x)\otimes I+I\otimes\rho(x)$, the two tensor factors commute, so $[T_x,T_y]=T_{[x,y]}$. This verifies the [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) identity over every field.

The [exterior square](../../../linear-algebra.md#exterior-square) and [symmetric square](../../../linear-algebra.md#symmetric-square) are the [quotient vector spaces](../../../vector-space.md#quotient-vector-space)

$$
\bigwedge^2V=(V\otimes V)/\langle v\otimes v:v\in V\rangle,
\qquad
S^2V=(V\otimes V)/\langle v\otimes w-w\otimes v:v,w\in V\rangle.
$$

In the [exterior square](../../../linear-algebra.md#exterior-square), expanding $(v+w)\otimes(v+w)$ shows that $v\wedge w=-w\wedge v$, including in [characteristic two](../../../algebra.md#characteristic-two). Both defining relation spaces are invariant under the [tensor product](../../../linear-algebra.md#tensor-product) action: $x(v\otimes v)=xv\otimes v+v\otimes xv$ is an exterior relation, and the image of a symmetric relation is a sum of symmetric relations. Thus the quotient actions are well-defined and satisfy

$$
x(v\wedge w)=xv\wedge w+v\wedge xw,\qquad x(vw)=(xv)w+v(xw).
$$

For the printed [basis](../../../vector-space.md#basis) $v_1,\ldots,v_n$, [bases](../../../vector-space.md#basis) are $v_i\wedge v_j$ with $i<j$ and $v_iv_j$ with $i\le j$. Their dimensions are $n(n-1)/2$ and $n(n+1)/2$ respectively.

**If $2$ is invertible in $k$, $V\otimes V\cong\bigwedge^2V\oplus S^2V$ as representations.** Define the flip $\tau(v\otimes w)=w\otimes v$. It commutes with the [Lie algebra](../../../lie-algebra.md) action and satisfies $\tau^2=I$. Therefore

$$
P_+=\frac{I+\tau}{2},\qquad P_-=\frac{I-\tau}{2}
$$

are complementary invariant [linear projections](../../../vector-space.md#projection-linear-algebra). The maps

$$
vw\longmapsto\frac{v\otimes w+w\otimes v}{2},\qquad
v\wedge w\longmapsto\frac{v\otimes w-w\otimes v}{2}
$$

identify $S^2V$ with $\operatorname{im}P_+$ and $\bigwedge^2V$ with $\operatorname{im}P_-$. Their inverses are the corresponding quotient maps restricted to these subspaces. This proves the assertion for every field of odd [characteristic](../../../algebra.md#characteristic-of-a-field), and also for [characteristic zero](../../../algebra.md#characteristic-zero).

**Over every field, $S^2(V\oplus W)\cong S^2V\oplus S^2W\oplus(V\otimes W)$.** The [symmetric square of a direct sum](../../../linear-algebra.md#symmetric-square-of-a-direct-sum) isomorphism sends the first two summands into products within $V$ and within $W$, and sends $v\otimes w$ to the mixed product $vw$. If $v_i$ and $w_j$ are [bases](../../../vector-space.md#basis), the monomial [basis](../../../vector-space.md#basis) of $S^2(V\oplus W)$ is the disjoint union

$$
\{v_iv_j:i\le j\},\qquad\{w_iw_j:i\le j\},\qquad\{v_iw_j:\text{all }i,j\}.
$$

Thus the map is bijective, with no division by $2$ needed. The [Leibniz rule](../../../calculus.md#leibniz-rule) for the action preserves each of these three summands and agrees with its usual [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) action, proving equivariance.

For $\mathfrak g=\mathfrak{sl}(3)$, $V=\Gamma_{0,0}$ is trivial and $W=\Gamma_{2,1}$ has dimension $15$. Hence

$$
S^2(V\oplus W)\cong\Gamma_{0,0}\oplus\Gamma_{2,1}\oplus S^2\Gamma_{2,1}.
$$

It remains to find the [irreducible representations](../../../representation-theory.md#irreducible-representation) in the [symmetric square of the sl3 representation of highest weight (2,1)](../../../semisimple-lie-algebra.md#symmetric-square-of-the-sl3-representation-of-highest-weight-2-1). We give the [formal character](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) calculation explicitly.

Let $E=\mathbb C^3$ be the defining [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra) representation. In [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label), its [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) are $(1,0)$, $(-1,1)$, and $(0,-1)$; the [dual representation](../../../representation-theory.md#dual-representation) has their negatives. The equivariant contraction

$$
c:S^2E\otimes E^*\longrightarrow E,\qquad c(uv\otimes f)=f(u)v+f(v)u
$$

is surjective. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) has dimension $18-3=15$. The tensor $e_1^2\otimes e_3^*$ is a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) of [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $(2,1)$ in that [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). By the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem), the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) contains the [irreducible representation](../../../representation-theory.md#irreducible-representation) $\Gamma_{2,1}$, whose [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) gives dimension $15$; therefore the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) equals $\Gamma_{2,1}$. This yields

$$
\chi_W=\chi_{S^2E}\chi_{E^*}-\chi_E.
$$

Multiplying the six [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) of $S^2E$ by the three [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) of $E^*$ and subtracting those of $E$ gives the following full [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) list:

$$
\begin{array}{c|l}
\text{multiplicity}&\text{weights in Dynkin labels}\\\hline
1&(2,1),(3,-1),(2,-2),(1,-3),(0,2),(-1,-2),(-2,3),(-2,0),(-3,2)\\
2&(1,0),(0,-1),(-1,1)
\end{array}
$$

The multiplicities sum to $9+2\cdot3=15$.

For any finite-dimensional [weight-space decomposition](../../../semisimple-lie-algebra.md#weight-space-decomposition), a [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $\mu$ of multiplicity $m_\mu$ contributes $m_\mu(m_\mu+1)/2$ to [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $2\mu$ in its [symmetric square](../../../linear-algebra.md#symmetric-square). Distinct [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $\mu,\nu$ contribute $m_\mu m_\nu$ to $\mu+\nu$. Equivalently,

$$
\chi_{S^2W}(z)=\frac{\chi_W(z)^2+\chi_W(z^2)}{2}.
$$

Applying this to the displayed list gives all dominant [weight multiplicities](../../../semisimple-lie-algebra.md#weight-multiplicity) in the second column below. The remaining columns are the [weight multiplicities](../../../semisimple-lie-algebra.md#weight-multiplicity) of the candidate [irreducible representations](../../../representation-theory.md#irreducible-representation):

$$
\begin{array}{c|r|rrrrr}
\text{weight}&S^2W&\Gamma_{4,2}&\Gamma_{3,1}&\Gamma_{0,4}&\Gamma_{1,2}&\Gamma_{2,0}\\\hline
(4,2)&1&1&0&0&0&0\\
(5,0)&1&1&0&0&0&0\\
(2,3)&1&1&0&0&0&0\\
(3,1)&3&2&1&0&0&0\\
(0,4)&2&1&0&1&0&0\\
(1,2)&5&2&1&1&1&0\\
(2,0)&8&3&2&1&1&1\\
(0,1)&9&3&2&1&2&1
\end{array}
$$

For an explicit way to compute each irreducible column, set $z_1z_2z_3=1$ and use the [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula) in the form

$$
\chi_{a,b}(z_1,z_2,z_3)=
\frac{\det\begin{pmatrix}z_1^{a+b+2}&z_1^{b+1}&1\\z_2^{a+b+2}&z_2^{b+1}&1\\z_3^{a+b+2}&z_3^{b+1}&1\end{pmatrix}}
{\det\begin{pmatrix}z_1^2&z_1&1\\z_2^2&z_2&1\\z_3^2&z_3&1\end{pmatrix}}.
$$

A monomial $z_1^{n_1}z_2^{n_2}z_3^{n_3}$ has [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) $(n_1-n_2,n_2-n_3)$. Equivalently, the quotient is enumerated by [Semistandard Young tableaux](../../../representation-theory-of-the-symmetric-group.md#semistandard-young-tableau) of shape $(a+b,b)$ with entries $1,2,3$, weakly increasing across rows and strictly increasing down columns; the exponents count the three entries.

The five irreducible columns sum to the $S^2W$ column. These are all its dominant [weights](../../../semisimple-lie-algebra.md#weight-representation-theory), and all five candidate characters have no other dominant [weights](../../../semisimple-lie-algebra.md#weight-representation-theory). Every [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) orbit meets the dominant chamber, and [weight multiplicities](../../../semisimple-lie-algebra.md#weight-multiplicity) are constant on [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) orbits. Thus the table proves equality of the full [formal characters](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module), and the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) gives

$$
\boxed{S^2\Gamma_{2,1}\cong\Gamma_{4,2}\oplus\Gamma_{3,1}\oplus\Gamma_{0,4}\oplus\Gamma_{1,2}\oplus\Gamma_{2,0}.}
$$

The [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) checks the result:

$$
60+24+15+15+6=120=\frac{15\cdot16}{2}.
$$

Consequently the requested decomposition is

$$
\boxed{S^2(\Gamma_{0,0}\oplus\Gamma_{2,1})\cong\Gamma_{0,0}\oplus\Gamma_{2,1}\oplus\Gamma_{4,2}\oplus\Gamma_{3,1}\oplus\Gamma_{0,4}\oplus\Gamma_{1,2}\oplus\Gamma_{2,0}.}
$$

Its total dimension is $1+15+120=136=16\cdot17/2$.

## 5

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

An abstract [root system](../../../semisimple-lie-algebra.md#root-system), in the reduced crystallographic convention, is a finite subset $\Phi$ of a finite-dimensional real [Euclidean space](../../../functional-analysis.md#euclidean-norm) $E$ satisfying the following conditions:

- $0\notin\Phi$ and $\Phi$ spans $E$.
- For each $\alpha\in\Phi$, $\Phi\cap\mathbb R\alpha=\{\alpha,-\alpha\}$; this is the reduced condition.
- The [root reflection](../../../semisimple-lie-algebra.md#root-reflection) $s_\alpha(v)=v-2(v,\alpha)\alpha/(\alpha,\alpha)$ preserves $\Phi$.
- Every [Cartan integer](../../../semisimple-lie-algebra.md#cartan-integer) $\langle\beta,\alpha^\vee\rangle=2(\beta,\alpha)/(\alpha,\alpha)$ is an integer.

The [root system](../../../semisimple-lie-algebra.md#root-system) is irreducible if it is not a union of two nonempty mutually orthogonal [root systems](../../../semisimple-lie-algebra.md#root-system). The integrality condition is essential for the finite angle list below; arbitrary finite reflection systems need not satisfy it.

**The possible angles are $0$, $\pi/6$, $\pi/4$, $\pi/3$, $\pi/2$, $2\pi/3$, $3\pi/4$, $5\pi/6$, and $\pi$.** For [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) $\alpha,\beta$, put

$$
a=\frac{2(\beta,\alpha)}{(\alpha,\alpha)},\qquad b=\frac{2(\alpha,\beta)}{(\beta,\beta)}.
$$

Both are [integers](../../../number-theory.md#integer), they have the same sign when nonzero, and

$$
ab=4\cos^2\theta.
$$

If the [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) are linearly independent, strict [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $0\le ab<4$. Hence $ab\in\{0,1,2,3\}$. These values give, respectively,

$$
\begin{array}{c|c|c}
ab&\theta&\text{ratio of squared lengths, larger to smaller}\\\hline
0&\pi/2&\text{unrestricted by this calculation}\\
1&\pi/3,\ 2\pi/3&1\\
2&\pi/4,\ 3\pi/4&2\\
3&\pi/6,\ 5\pi/6&3
\end{array}
$$

For the last column, the possible absolute pairs $(|a|,|b|)$ are $(1,1)$, $(1,2)$, and $(1,3)$, up to interchange, and $a/b=(\beta,\beta)/(\alpha,\alpha)$. Parallel [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) are equal or opposite by reducedness, giving $0$ or $\pi$. Thus the list is exhaustive, and the rank-two [root systems](../../../semisimple-lie-algebra.md#root-system) realize each nonparallel possibility.

Now suppose two [simple roots](../../../semisimple-lie-algebra.md#simple-root) $\alpha,\beta$ have angle $5\pi/6$. Distinct [simple roots](../../../semisimple-lie-algebra.md#simple-root) have nonpositive inner product. Here is a proof from their defining sign property: if $(\delta,\epsilon)>0$, then $s_\delta(\epsilon)=\epsilon-n\delta$ with a positive [Cartan integer](../../../semisimple-lie-algebra.md#cartan-integer) $n$. This would be a [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) whose coefficients in the [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) include both a positive and a negative coefficient, which is impossible. Therefore, after normalizing the [simple roots](../../../semisimple-lie-algebra.md#simple-root) to unit length, any nonzero off-diagonal inner product is at most $-1/2$, by the angle list.

Let $u=\alpha/\|\alpha\|$, $v=\beta/\|\beta\|$, so $(u,v)=-\sqrt3/2$. If there were a third [simple root](../../../semisimple-lie-algebra.md#simple-root) with unit vector $w$, write $r=(u,w)\le0$ and $s=(v,w)\le0$. Independence of the [simple roots](../../../semisimple-lie-algebra.md#simple-root) makes their [Gram matrix](../../../linear-algebra.md#gram-matrix) positive definite, so

$$
0<\det\begin{pmatrix}1&-\sqrt3/2&r\\-\sqrt3/2&1&s\\r&s&1\end{pmatrix}
=\frac14-r^2-s^2-\sqrt3rs.
$$

If either $r$ or $s$ were nonzero, its absolute value would be at least $1/2$. Since $rs\ge0$, the displayed determinant would then be nonpositive. Thus $r=s=0$. Every other [simple root](../../../semisimple-lie-algebra.md#simple-root) is orthogonal to both $\alpha$ and $\beta$: a [triple bond isolates a G2 component](../../../semisimple-lie-algebra.md#triple-bond-isolates-a-g2-component).

Indeed, the [root reflections](../../../semisimple-lie-algebra.md#root-reflection) in $\alpha,\beta$ preserve their plane and fix its orthogonal complement; the [root reflections](../../../semisimple-lie-algebra.md#root-reflection) in the other [simple roots](../../../semisimple-lie-algebra.md#simple-root) preserve that complement and fix the plane. The given facts that these reflections generate the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) and that every [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) is [Weyl group](../../../semisimple-lie-algebra.md#weyl-group)-conjugate to a [simple root](../../../semisimple-lie-algebra.md#simple-root) imply that every [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) lies entirely in one of those two orthogonal subspaces. If there were any other [simple root](../../../semisimple-lie-algebra.md#simple-root), this would make $\Phi$ reducible. Therefore irreducibility forces rank two.

Up to interchanging the [simple roots](../../../semisimple-lie-algebra.md#simple-root), take $\alpha$ short and $\beta$ long. The squared-length ratio is $3$. Choose a scale and orthonormal coordinates so that

$$
\alpha=(1,0),\qquad\beta=\left(-\frac32,\frac{\sqrt3}{2}\right).
$$

The [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) are $\langle\beta,\alpha^\vee\rangle=-3$ and $\langle\alpha,\beta^\vee\rangle=-1$. In coefficient coordinates $m\alpha+n\beta$, the two [root reflections](../../../semisimple-lie-algebra.md#root-reflection) are

$$
s_\alpha(m,n)=(-m+3n,n),\qquad s_\beta(m,n)=(m,m-n).
$$

Their orbits of $\alpha$ and $\beta$ are, respectively,

$$
\{\pm\alpha,\pm(\alpha+\beta),\pm(2\alpha+\beta)\},\qquad
\{\pm\beta,\pm(3\alpha+\beta),\pm(3\alpha+2\beta)\}.
$$

These sets are closed under both displayed reflections; for example $s_\beta(\alpha)=\alpha+\beta$, $s_\alpha(\alpha+\beta)=2\alpha+\beta$, $s_\alpha(\beta)=3\alpha+\beta$, and $s_\beta(3\alpha+\beta)=3\alpha+2\beta$. The assumption that every [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) is conjugate to a [simple root](../../../semisimple-lie-algebra.md#simple-root) now determines all twelve [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system), with no further ones possible.

<a id="5/image-the-twelve-g2-roots-with-the-six-positive-roots-labelled-and-the-simple-roots-emphasized"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-102-g2-roots.png)

**[Figure 1](#5/image-the-twelve-g2-roots-with-the-six-positive-roots-labelled-and-the-simple-roots-emphasized). The twelve G2 roots, with the six positive roots labelled and the simple roots emphasized**.

For completeness, this twelve-element set really is a [root system](../../../semisimple-lie-algebra.md#root-system). It is finite, spans the plane, and is reduced. The six [short roots](../../../semisimple-lie-algebra.md#short-root) have length $1$ and directions spaced by $\pi/3$; the six [long roots](../../../semisimple-lie-algebra.md#long-root) have length $\sqrt3$ and interleaved directions, also spaced by $\pi/3$. Their mutual [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) are integral: within either length class they are $0$, $\pm1$, or $\pm2$ as applicable, and between the two length classes they are $0$, $\pm1$, or $\pm3$. Closure under all [root reflections](../../../semisimple-lie-algebra.md#root-reflection) follows by conjugating the two simple reflections, since every listed [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) lies in a simple-root orbit. The nonorthogonal [simple roots](../../../semisimple-lie-algebra.md#simple-root) make it irreducible. We have therefore proved existence as well as uniqueness, up to isometry and overall scale:

$$
\boxed{\text{The unique irreducible type is the }G_2\text{ root system}.}
$$

## 6

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A smooth [vector field](../../../calculus.md#vector-field) on a [smooth manifold](../../../differential-geometry.md#smooth-manifold) $M$ is a smooth section of the [tangent bundle](../../../fiber-bundle.md#tangent-bundle): it assigns $v(p)\in T_pM$ to each $p$, smoothly in local coordinates. In a coordinate chart it has the form $v=\sum_i a_i\partial/\partial x_i$, with smooth coefficients $a_i$. Equivalently, it acts on smooth functions as a derivation, $v(fh)=v(f)h+fv(h)$.

For a [Lie group](../../../lie-theory.md#lie-group) $G$, write $L_a(h)=ah$ for [Left translation on a Lie group](../../../lie-theory.md#left-and-right-translation-on-a-lie-group). A [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) satisfies

$$
(dL_a)_h v(h)=v(ah)\qquad(a,h\in G).
$$

Thus it is determined by its value at the identity. Given the printed $X\in T_gG$, first translate it to the identity:

$$
\xi=(dL_{g^{-1}})_gX\in T_eG.
$$

The unique [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) with value $X$ at $g$ is

$$
\boxed{v_X(h)=(dL_h)_e\xi=(dL_{hg^{-1}})_gX.}
$$

The smoothness of multiplication makes this a smooth [vector field](../../../calculus.md#vector-field), the chain rule proves left invariance, and setting $h=g$ gives $v_X(g)=X$.

We prove the [completeness of left-invariant vector fields](../../../lie-theory.md#completeness-of-left-invariant-vector-fields): this [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) is a [complete vector field](../../../differential-geometry.md#complete-vector-field). The [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem), applied in a local chart, gives a unique local [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) $u:(-\varepsilon,\varepsilon)\to G$ through $e$. For every $h\in G$, the curve $t\mapsto hu(t)$ is an [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) through $h$, because

$$
\frac{d}{dt}(hu(t))=(dL_h)_{u(t)}v_X(u(t))=v_X(hu(t)).
$$

Crucially, the same interval $(-\varepsilon,\varepsilon)$ works for every initial point.

Let $\gamma$ be the maximal [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) through $g$, with maximal interval $(a,b)$. If $b<\infty$, choose $t_0\in(a,b)$ with $b-t_0<\varepsilon/2$. The curve

$$
t\longmapsto\gamma(t_0)u(t-t_0)
$$

exists on $(t_0-\varepsilon,t_0+\varepsilon)$ and agrees with $\gamma$ on the overlap by uniqueness of the local [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation). It extends $\gamma$ past $b$, a contradiction. The same argument at a finite $a$ excludes that possibility. Thus $(a,b)=\mathbb R$, and uniqueness on overlapping intervals gives uniqueness on all of $\mathbb R$.

After establishing completeness, uniqueness also gives the [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) law for the global curve through $e$:

$$
u(s+t)=u(s)u(t).
$$

Both sides, as curves in $t$, are [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) through $u(s)$ at $t=0$. Defining the [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) by $u(t)=\exp(t\xi)$, the answer is

$$
\boxed{\gamma_g(t)=g\exp(t\xi),\qquad \xi=(dL_{g^{-1}})_gX,\qquad t\in\mathbb R.}
$$

**The identity component $G^\circ$ is an open normal subgroup, and every open identity neighbourhood generates it.** Let $G^\circ$ be the [connected component](../../../geometry-and-topology.md#connected-component) of $e$. The product of connected spaces is connected, so the image of $G^\circ\times G^\circ$ under multiplication is connected and contains $e$. It is therefore contained in $G^\circ$. Inversion has the same property. Thus $G^\circ$ is a [subgroup](../../../group.md#subgroup).

A [smooth manifold](../../../differential-geometry.md#smooth-manifold) is locally connected. In particular, a coordinate neighbourhood of $e$ can be chosen homeomorphic to an open ball, so there is a connected open neighbourhood $O$ of $e$ contained in $G^\circ$. Its translates $hO$, $h\in G^\circ$, are open and lie in $G^\circ$, and cover $G^\circ$. Therefore the [identity component of a Lie group](../../../lie-theory.md#identity-component-of-a-lie-group) is open in $G$. Conjugation by any $a\in G$ is a [homeomorphism](../../../topology.md#homeomorphism) fixing $e$, so it maps $G^\circ$ into itself; conjugation by $a^{-1}$ gives the reverse inclusion. Hence $G^\circ$ is a [normal subgroup](../../../group-theory.md#normal-subgroup).

If $U$ is an open neighbourhood of $e$ in $G^\circ$, let $H=\langle U\rangle$, allowing inverses in the meaning of generated [subgroup](../../../group.md#subgroup). For each $h\in H$, $hU$ is open and lies in $H$, so $H=\bigcup_{h\in H}hU$ is open in $G^\circ$. Every other left [coset](../../../group-theory.md#coset) of $H$ is also open. Thus $H$ is both open and closed in the connected space $G^\circ$. It is nonempty, so $H=G^\circ$.

A [quadratic form](../../../linear-algebra.md#quadratic-form) on $V=\mathbb R^n$ is a function $Q(v)=B(v,v)$ for a symmetric [bilinear form](../../../linear-algebra.md#bilinear-form) $B$. Equivalently, $Q(tv)=t^2Q(v)$ and the polarization

$$
B(u,v)=\frac{Q(u+v)-Q(u)-Q(v)}2
$$

is a [bilinear map](../../../linear-algebra.md#bilinear-map). In coordinates there is a unique real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $A$ with $Q(v)=v^TAv$. No assumption of nondegeneracy or positive definiteness is needed.

An element $g\in\operatorname{GL}_n(\mathbb R)$ stabilizes $Q$ when $Q(gv)=Q(v)$ for every $v$. By the [polarization identity](../../../linear-algebra.md#polarization-identity), this is equivalent to preserving $B$, or in coordinates to

$$
G_Q=\{g\in\operatorname{GL}_n(\mathbb R):g^TAg=A\}.
$$

This is a closed [Matrix Lie group](../../../lie-theory.md#matrix-lie-group). The [Lie algebra of a quadratic-form stabilizer](../../../lie-theory.md#lie-algebra-of-a-quadratic-form-stabilizer) is

$$
\boxed{T_eG_Q=\{X\in M_n(\mathbb R):X^TA+AX=0\}.}
$$

To prove necessity, differentiate $g(t)^TAg(t)=A$ along any smooth curve in $G_Q$ with $g(0)=I$, $g'(0)=X$. The derivative at zero is $X^TA+AX$.

To prove sufficiency, suppose $X^TA+AX=0$ and consider the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) $g(t)=e^{tX}$. Then

$$
\frac{d}{dt}\bigl(e^{tX^T}Ae^{tX}\bigr)=e^{tX^T}(X^TA+AX)e^{tX}=0.
$$

Its value at zero is $A$, so $e^{tX}\in G_Q$ for every real $t$. This curve has derivative $X$ at zero, proving the claimed [tangent space](../../../differential-geometry.md#tangent-space) description even for a degenerate [quadratic form](../../../linear-algebra.md#quadratic-form).

Equivalently, the condition is $B(Xu,v)+B(u,Xv)=0$ for all $u,v$. For a nondegenerate [quadratic form](../../../linear-algebra.md#quadratic-form) it is the corresponding [Special orthogonal Lie algebra](../../../semisimple-lie-algebra.md#special-orthogonal-lie-algebra). To see the degenerate case explicitly, choose a [basis](../../../vector-space.md#basis) with

$$
A=\begin{pmatrix}D&0\\0&0\end{pmatrix},\qquad D=\operatorname{diag}(I_r,-I_s).
$$

Writing $X=\begin{pmatrix}P&R\\S&T\end{pmatrix}$, the condition becomes

$$
P^TD+DP=0,\qquad R=0,
$$

while $S,T$ are arbitrary. Thus the nullspace of the [quadratic form](../../../linear-algebra.md#quadratic-form) is invariant, but arbitrary infinitesimal maps into it are allowed. When $A=0$, the formula correctly gives $G_Q=\operatorname{GL}_n(\mathbb R)$ and $T_eG_Q=M_n(\mathbb R)$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
