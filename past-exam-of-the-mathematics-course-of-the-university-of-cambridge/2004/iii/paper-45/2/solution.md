<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $V=\mathbb C^3$ be the defining flavor [SU(3)](../../../../../su-3-group.md) [representation](../../../../../group-representation.md). Under $U\in SU(3)$, $q^\alpha\mapsto U^\alpha{}_{\beta}q^\beta$. The [antiquark](../../../../../antiquark.md) transforms in the [dual representation](../../../../../dual-representation.md):

$$
\bar q_\alpha\mapsto (U^{-1})^\beta{}_{\alpha}\bar q_\beta.
$$

Since $U$ is unitary, its lower-index column of components transforms by $U^*$, the complex conjugate numerical matrix. Thus $q^\alpha\bar q_\alpha$ is invariant. The defining triplet and its conjugate are inequivalent complex [representations](../../../../../group-representation.md); conjugation reverses their [weights](../../../../../weight-representation-theory.md). Write $\mathbf3=V$ and $\overline{\mathbf3}=V^*$, and distinguish a [direct sum](../../../../../direct-sum.md) $\oplus$ from a [tensor product](../../../../../tensor-product.md) $\otimes$.

First split $V\otimes V$ into [symmetric tensors](../../../../../symmetric-tensor.md) and [totally antisymmetric tensors](../../../../../totally-antisymmetric-tensor.md):

$$
V\otimes V=\operatorname{Sym}^2V\oplus\Lambda^2V.
$$

The symmetric part has dimension $3(3+1)/2=6$. Contracting the antisymmetric part with the invariant [Levi-Civita symbol](../../../../../levi-civita-symbol.md) gives $A_\gamma=\tfrac12\epsilon_{\gamma\alpha\beta}A^{\alpha\beta}$, which transforms as a dual vector because $\det U=1$. Its inverse is $A^{\alpha\beta}=\epsilon^{\alpha\beta\gamma}A_\gamma$. Hence

$$
\boxed{\mathbf3\otimes\mathbf3=\overline{\mathbf3}\oplus\mathbf6.}
$$

The symmetric part is the irreducible [highest-weight representation](../../../../../highest-weight-representation.md) with [Dynkin labels](../../../../../dynkin-label.md) $(2,0)$; its six monomials give the standard symmetric-square [representation](../../../../../group-representation.md).

For three triplets, the antisymmetric first-pair sector becomes $V^*\otimes V$. Its [tensors](../../../../../tensor.md) $M^\alpha{}_{\beta}$ split into their scalar trace and traceless part:

$$
V^*\otimes V=\mathbf1\oplus\mathbf8,\qquad
M=\frac{\operatorname{tr}M}{3}\mathbf1+\left(M-\frac{\operatorname{tr}M}{3}\mathbf1\right).
$$

The traceless part is the [adjoint representation of SU(3)](../../../../../adjoint-representation-of-su-3.md); conjugation acts as $M\mapsto UMU^{-1}$. It is irreducible because an invariant subspace would be an ideal in the simple complex [special linear Lie algebra](../../../../../special-linear-lie-algebra.md) $\mathfrak{sl}_3$.

The symmetric first-pair sector consists of $T^{abc}=T^{bac}$ and has dimension $6\cdot3=18$. Complete symmetrization maps it onto $\operatorname{Sym}^3V$, whose dimension is $\binom53=10$. Its kernel is the mixed-symmetry eight-dimensional sector. More explicitly, the equivariant map $T^{abc}\mapsto M^a{}_e=\epsilon_{ebc}T^{abc}$ has trace zero because the first two indices of $T$ are symmetric; it annihilates the completely symmetric part and is not identically zero. Since the target adjoint module is irreducible, the map is onto its eight-dimensional space. Its kernel is consequently exactly the ten-dimensional completely symmetric part. Complete symmetrization supplies an invariant splitting, so this sector is $\mathbf{10}\oplus\mathbf8$. Combining the sectors gives the [tensor cube of the defining SU(3) representation](../../../../../tensor-cube-of-the-defining-su-3-representation.md)

$$
\boxed{\mathbf3^{\otimes3}=\mathbf1\oplus\mathbf8\oplus\mathbf8\oplus\mathbf{10}.}
$$

Here the decuplet has [Dynkin labels](../../../../../dynkin-label.md) $(3,0)$, and the singlet is the fully antisymmetric contraction $\epsilon_{abc}T^{abc}$. The two octets are distinct copies, not two different irreducible types.

For [two conjugate SU(3) triplets with a triplet](../../../../../two-conjugate-su-3-triplets-with-a-triplet.md), begin with $T^a{}_{bc}$ and split its lower pair. An antisymmetric lower pair is identified by $\epsilon^{bcd}$ with an upper index, giving $V\otimes V=\mathbf6\oplus\overline{\mathbf3}$. The symmetric lower-pair sector has dimension $3\cdot6=18$, and its contraction is the equivariant map

$$
C(T)_b=\sum_aT^a{}_{ba}.
$$

It is onto $V^*$, since the invariant embedding

$$
\iota(v)^a{}_{bc}=\frac14(\delta^a_bv_c+\delta^a_cv_b)
$$

satisfies $C\iota(v)=v$. Every such [tensor](../../../../../tensor.md) therefore splits uniquely as $\iota(C(T))+(T-\iota(C(T)))$. The latter [tensor](../../../../../tensor.md) is symmetric in its lower indices and has zero contraction, with dimension $18-3=15$. It contains the [highest-weight vector](../../../../../highest-weight-vector.md) $e_1\otimes(e_3^*)^2$ of [Dynkin labels](../../../../../dynkin-label.md) $(1,2)$; contraction vanishes because its upper and lower indices differ. The [Weyl dimension formula](../../../../../weyl-dimension-formula.md) for an [SU(3)](../../../../../su-3-group.md) module with labels $(p,q)$ is $\dim V_{(p,q)}=(p+1)(q+1)(p+q+2)/2$, which gives $15$ for $(1,2)$. These [tensor](../../../../../tensor.md) [representations](../../../../../group-representation.md) are unitary, so invariant subspaces have invariant orthogonal complements; the irreducible highest-[weight](../../../../../weight-representation-theory.md) summand containing this vector exhausts the fifteen-dimensional kernel. Thus

$$
\boxed{\overline{\mathbf3}\otimes\overline{\mathbf3}\otimes\mathbf3
=\overline{\mathbf3}\oplus\overline{\mathbf3}\oplus\mathbf6\oplus V_{(1,2)}.}
$$

The question's dimension label $15$ denotes $V_{(1,2)}$, rather than its conjugate $V_{(2,1)}$; they have equal dimensions but different [tensors](../../../../../tensor.md). Conjugating the triplet-cube decomposition gives

$$
\boxed{\overline{\mathbf3}^{\otimes3}=\mathbf1\oplus\mathbf8\oplus\mathbf8\oplus\overline{\mathbf{10}}.}
$$

The octet is self-conjugate, whereas the symmetric decuplet changes $(3,0)$ to $(0,3)$.

Now consider the flavor [diquark](../../../../../diquark.md) $D_\alpha\propto\epsilon_{\alpha\beta\gamma}q^\beta q^\gamma$. This notation describes an antisymmetric two-[quark](../../../../../quark.md) flavor state; color and [spin](../../../../../spin.md) factors are separate. In particular $D_3=(ud-du)/\sqrt2$ has [isospin](../../../../../isospin.md) zero, [baryon number](../../../../../baryon-number.md) $2/3$, [strangeness](../../../../../strangeness.md) zero and [flavor hypercharge](../../../../../flavor-hypercharge.md) $2/3$. The strange [antiquark](../../../../../antiquark.md) has $I=0$, $B=-1/3$, $S=+1$ and $Y=2/3$. Thus $D_3D_3\bar s$ has

$$
\boxed{B=1,\qquad S=+1,\qquad Y=2,\qquad I=0,\qquad Q=+1.}
$$

The charge follows from the [Gell-Mann--Nishijima formula](../../../../../gell-mann-nishijima-formula.md). Each of the three factors has lower flavor index $3$, so their product is the completely symmetric [tensor](../../../../../tensor.md) component $A_{333}$. It lies entirely in $\operatorname{Sym}^3V^*=\overline{\mathbf{10}}$, the [pentaquark antidecuplet](../../../../../pentaquark-antidecuplet.md). Equivalently, the symmetric diquark pair belongs to $\overline{\mathbf6}$, and $\overline{\mathbf6}\otimes\overline{\mathbf3}=\overline{\mathbf{10}}\oplus\mathbf8$, with this highest-hypercharge state in the antidecuplet.

It cannot be in an octet. The octet has the [weights](../../../../../weight-representation-theory.md) of a traceless $q^\alpha\bar q_\beta$ [tensor](../../../../../tensor.md), whose hypercharges are $Y_\alpha-Y_\beta$. For $(u,d,s)$ the [quark](../../../../../quark.md) values are $1/3,1/3,-2/3$, so these differences are only $0,+1,-1$; there is no $Y=2$ [weight](../../../../../weight-representation-theory.md). The octet's top row instead has $Y=1$ and $I=1/2$. This is a flavor-[representation](../../../../../group-representation.md) assignment for a possible [pentaquark](../../../../../pentaquark.md), not a proof that the configuration binds or that its full color-[spin](../../../../../spin.md)-orbital wavefunction satisfies all [Fermi statistics](../../../../../fermi-dirac-statistics.md) constraints.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
