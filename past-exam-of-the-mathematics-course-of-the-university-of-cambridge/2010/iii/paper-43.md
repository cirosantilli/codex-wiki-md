# Paper 43

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper43.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper43.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) acts on the algebra itself by $\operatorname{ad}_X(Y)=[X,Y]$. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives $[\operatorname{ad}_X,\operatorname{ad}_Y]=\operatorname{ad}_{[X,Y]}$, so this is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). In the generator basis, the column labelled $b$ records the coefficients of $[T_a,T_b]$, giving

$$
\boxed{(t_a^{\mathrm{Ad}})^c{}_b=i f_{abc}.}
$$

In the orthonormal compact-algebra convention, the [structure constants of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) are totally antisymmetric. With the row index written first this is $(t_a^{\mathrm{Ad}})_{bc}=-if_{abc}$.

Applying the representation to the generator [commutator](../../../lie-algebra.md#commutator) and taking a [trace](../../../linear-algebra.md#matrix-trace) against $t_c^R$ gives

$$
\operatorname{tr}([t_a^R,t_b^R]t_c^R)
=i f_{abd}\operatorname{tr}(t_d^Rt_c^R)
=i C(R)f_{abc}.
$$

Consequently, for a nonzero [trace](../../../linear-algebra.md#matrix-trace) normalization,

$$
\boxed{f_{abc}=-\frac{i}{C(R)}\operatorname{tr}([t_a^R,t_b^R]t_c^R).}
$$

The [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace) also shows that this expression is antisymmetric in every pair of indices, justifying the orthonormal convention used for the adjoint matrices.

The summed [quadratic Casimir operator](../../../semisimple-lie-algebra.md#quadratic-casimir-operator) has scalar value $C_2(R)$ on the representation under consideration. Taking its [trace](../../../linear-algebra.md#matrix-trace) in two ways yields

$$
\sum_{a=1}^{d(G)}\operatorname{tr}(t_a^Rt_a^R)=C(R)d(G)=C_2(R)d(R),
$$

and hence

$$
\boxed{C(R)=\frac{d(R)C_2(R)}{d(G)}.}
$$

The constant $C(R)$ is the representation's [Dynkin index](../../../semisimple-lie-algebra.md#dynkin-index) in this normalization.

Differentiating the [tensor product of group representations](../../../representation-theory.md#tensor-product-of-group-representations) gives

$$
\boxed{t_a^{R_1\otimes R_2}=t_a^{R_1}\otimes I_{d(R_2)}+I_{d(R_1)}\otimes t_a^{R_2}.}
$$

The generators acting on the two factors commute, so the sum of their squares is

$$
\sum_a(t_a^{R_1\otimes R_2})^2
=[C_2(R_1)+C_2(R_2)]I+2\sum_at_a^{R_1}\otimes t_a^{R_2}.
$$

For a [semisimple Lie algebra](../../../semisimple-lie-algebra.md), every element is a sum of [commutators](../../../lie-algebra.md#commutator). Since the [trace](../../../linear-algebra.md#matrix-trace) of each represented [commutator](../../../lie-algebra.md#commutator) vanishes, all represented generators are [traceless matrices](../../../linear-algebra.md#traceless-matrix). The [trace](../../../linear-algebra.md#matrix-trace) of the cross term is therefore zero. Taking the [trace](../../../linear-algebra.md#matrix-trace) after decomposition into [irreducible representations](../../../representation-theory.md#irreducible-representation) instead gives the [tensor-product Casimir trace identity](../../../semisimple-lie-algebra.md#tensor-product-casimir-trace-identity)

$$
\boxed{[C_2(R_1)+C_2(R_2)]d(R_1)d(R_2)=\sum_i C_2(R_i)d(R_i),}
$$

where repeated irreducible constituents occur repeatedly in the sum.

This step requires tracelessness, as holds for the special unitary groups used below. For an arbitrary algebra with an abelian factor, the general [trace](../../../linear-algebra.md#matrix-trace) formula has the extra term $2\sum_a\operatorname{tr}(t_a^{R_1})\operatorname{tr}(t_a^{R_2})$. For example, one-dimensional representations of an abelian generator with charges one and one have individual Casimirs one, while the product generator has charge two and Casimir four. Thus the identity without the cross term is not a theorem for every [Lie algebra](../../../lie-algebra.md) as the unrestricted opening wording might suggest.

For the [fundamental-antifundamental decomposition for SU(N)](../../../representation-theory.md#fundamental-antifundamental-decomposition-for-su-n), write a product [tensor](../../../linear-algebra.md#tensor) as a [matrix](../../../vector-space.md#matrix) $M^i{}_j$. It transforms as $M\mapsto UMU^{-1}$, and decomposes uniquely as

$$
M=\frac{\operatorname{tr}M}{N}I+\left(M-\frac{\operatorname{tr}M}{N}I\right).
$$

The first term is a [trivial representation](../../../representation-theory.md#trivial-representation), and the second is the invariant traceless subspace, of [dimension](../../../vector-space.md#dimension-vector-space) $N^2-1$. Its infinitesimal transformation is a [commutator](../../../lie-algebra.md#commutator), so it is the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). This representation is irreducible for $N\ge2$: an [invariant subspace](../../../representation-theory.md#invariant-subspace) is an ideal of $\mathfrak{sl}_N$; commuting a nonzero ideal element with diagonal and elementary matrices produces off-diagonal elementary matrices, whose further [commutators](../../../lie-algebra.md#commutator) generate all off-diagonal matrices and traceless diagonal matrices. A purely diagonal nonzero element also produces an off-diagonal element unless it is scalar, and a traceless scalar in characteristic zero is zero. Therefore

$$
\boxed{\mathbf N\otimes\overline{\mathbf N}=\mathbf1\oplus\mathbf{Adj},\qquad d(\mathbf{Adj})=N^2-1.}
$$

For the conjugate defining representation the generators are $-t_a^T$, so its [trace](../../../linear-algebra.md#matrix-trace) index and Casimir equal those of the defining representation. With $C(\mathbf N)=1/2$, the [trace](../../../linear-algebra.md#matrix-trace) formula gives $C_2(\mathbf N)=(N^2-1)/(2N)$. The product [trace](../../../linear-algebra.md#matrix-trace) identity, with the zero Casimir of the singlet, then reads

$$
2\frac{N^2-1}{2N}N^2=C_2(\mathbf{Adj})(N^2-1).
$$

Cancelling the nonzero factor yields

$$
\boxed{C_2(\mathbf{Adj})=N.}
$$

## 2

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) is a linear map $\rho:\mathfrak g\to\operatorname{End}(V)$ preserving brackets: $\rho([X,Y])=[\rho(X),\rho(Y)]$. Differentiating a smooth [unitary representation](../../../representation-theory.md#unitary-representation) $D$ of a [Lie group](../../../lie-theory.md#lie-group) gives $\rho(X)=\left.\frac{d}{dt}D(e^{tX})\right|_{t=0}$, an anti-Hermitian operator for each real algebra element $X$. In the physics convention one uses Hermitian generators $t_X=i\rho(X)$ and writes $D(e^{tX})=e^{-it t_X}$. Conversely, [integration of a Lie-algebra representation](../../../lie-algebra.md#integration-of-a-lie-algebra-representation) gives a representation of the connected simply connected group. A representation of another group with the same algebra additionally has to be trivial on the kernel of its [covering map](../../../algebraic-topology.md#covering-space).

For the [angular momentum commutation relations](../../../quantum-mechanics.md#angular-momentum-commutation-relations), take $J_3$ Hermitian and $J_+^\dagger=J_-$ on a positive-definite inner-product space. A [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) has $J_3|j,j\rangle=j|j,j\rangle$ and $J_+|j,j\rangle=0$. Set $v_\ell=(J_-)^\ell|j,j\rangle$. Commuting $J_3$ through each lowering operator gives $J_3v_\ell=(j-\ell)v_\ell$. Furthermore,

$$
[J_+,(J_-)^\ell]=\sum_{r=0}^{\ell-1}(J_-)^r(2J_3)(J_-)^{\ell-1-r},
$$

so acting on the highest-weight state and summing the coefficients gives

$$
J_+v_\ell=\ell(2j-\ell+1)v_{\ell-1}.
$$

Taking the [inner product](../../../linear-algebra.md#inner-product) with $v_{\ell-1}$ produces the [unitary highest-weight termination](../../../quantum-mechanics.md#unitary-highest-weight-termination) recursion

$$
\|v_\ell\|^2=\ell(2j-\ell+1)\|v_{\ell-1}\|^2.
$$

The first factor requires $j\ge0$. If $2j$ is not an integer, the first integer $\ell>2j+1$ would make the norm negative, while every preceding norm is positive. Thus

$$
\boxed{2j\in\mathbb Z_{\ge0}.}
$$

For these values, $v_0,\ldots,v_{2j}$ have strictly positive norms and distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue), while $v_{2j+1}$ has zero norm and hence is zero. They therefore span a space of [dimension](../../../vector-space.md#dimension-vector-space) $2j+1$, invariant under all three generators. Its weights are $j,j-1,\ldots,-j$. This proves **integer or half-integer [spin](../../../quantum-mechanics.md#spin) and finite [dimension](../../../vector-space.md#dimension-vector-space) $2j+1$**. The positive-definite unitary assumption matters: an unrestricted algebraic highest-weight module need not terminate. Normalizing the ladder states yields

$$
J_\pm|j,m\rangle=\sqrt{(j\mp m)(j\pm m+1)}\,|j,m\pm1\rangle.
$$

This is the [normalized highest-weight lowering formula](../../../quantum-mechanics.md#normalized-highest-weight-lowering-formula) with the usual positive ladder phases and units $\hbar=1$.

In the ordered spin-one-half basis $(|1/2,1/2\rangle,|1/2,-1/2\rangle)$, the matrices are

$$
\boxed{J_3=\frac12\begin{pmatrix}1&0\\0&-1\end{pmatrix},\quad
J_+=\begin{pmatrix}0&1\\0&0\end{pmatrix},\quad
J_-=\begin{pmatrix}0&0\\1&0\end{pmatrix}.}
$$

Thus $J_i=\sigma_i/2$, where the $\sigma_i$ are [Pauli matrices](../../../algebra.md#pauli-matrices).

Choose the active-rotation convention. The [SU(2)](../../../topological-group.md#su-2-group) lift of an axis-angle rotation is

$$
U_{1/2}(\vartheta,\mathbf n)=e^{-i\vartheta\mathbf n\cdot\boldsymbol\sigma/2}
=\cos(\vartheta/2)I-i\sin(\vartheta/2)\mathbf n\cdot\boldsymbol\sigma.
$$

The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) shows that conjugating $\mathbf x\cdot\boldsymbol\sigma$ by this [matrix](../../../vector-space.md#matrix) produces $(R\mathbf x)\cdot\boldsymbol\sigma$, with

$$
R\mathbf x=\mathbf x\cos\vartheta+(\mathbf n\times\mathbf x)\sin\vartheta
+\mathbf n(\mathbf n\cdot\mathbf x)(1-\cos\vartheta).
$$

This is the ordinary three-dimensional rotation. In any spin-$j$ representation the corresponding unitary operator and its [matrix](../../../vector-space.md#matrix) elements are

$$
\boxed{U_j(R)=e^{-i\vartheta\mathbf n\cdot\mathbf J^{(j)}},\qquad
D^{(j)}_{mm'}(R)=\langle j,m|U_j(R)|j,m'\rangle.}
$$

For half-integer [spin](../../../quantum-mechanics.md#spin), $R$ in this notation includes a choice of lift to [SU(2)](../../../topological-group.md#su-2-group); it does not define a single-valued representation of [SO(3)](../../../linear-algebra.md#so-3-group).

For the specified Euler-angle order, the rightmost rotation acts first:

$$
\boxed{U_j(R)=e^{-i\phi J_3}e^{-i\theta J_2}e^{-i\psi J_3},\qquad
D^{(j)}_{mm'}(R)=e^{-im\phi}d^{(j)}_{mm'}(\theta)e^{-im'\psi}.}
$$

Here the [Wigner D-matrix](../../../quantum-mechanics.md#wigner-d-matrix) middle factor is $d^{(j)}_{mm'}(\theta)=\langle j,m|e^{-i\theta J_2}|j,m'\rangle$. It can be calculated explicitly by realizing [spin](../../../quantum-mechanics.md#spin) $j$ as the symmetric product of $2j$ spin-one-half factors. Write $c=\cos(\theta/2)$ and $s=\sin(\theta/2)$. The fundamental rotation sends $|+\rangle$ to $c|+\rangle+s|-\rangle$ and $|-\rangle$ to $-s|+\rangle+c|-\rangle$. Expanding a normalized symmetric state with $j+m'$ plus signs gives

$$
d^{(j)}_{mm'}(\theta)=\sqrt{(j+m)!(j-m)!(j+m')!(j-m')!}
\sum_r\frac{(-1)^{m-m'+r}c^{2j+m'-m-2r}s^{m-m'+2r}}
{(j+m'-r)!\,r!\,(m-m'+r)!\,(j-m-r)!},
$$

where $\max(0,m'-m)\le r\le\min(j+m',j-m)$. The exponent $r$ counts initially positive spinors that become negative, while $m-m'+r$ counts initially negative ones that become positive; their minus signs and binomial coefficients give the displayed expression. Every factorial argument is an integer even for half-integer [spin](../../../quantum-mechanics.md#spin).

For [spin](../../../quantum-mechanics.md#spin) one-half this reduces to the explicit [matrix](../../../vector-space.md#matrix)

$$
D^{(1/2)}(\phi,\theta,\psi)=
\begin{pmatrix}
e^{-i(\phi+\psi)/2}\cos(\theta/2)&-e^{-i(\phi-\psi)/2}\sin(\theta/2)\\
e^{i(\phi-\psi)/2}\sin(\theta/2)&e^{i(\phi+\psi)/2}\cos(\theta/2)
\end{pmatrix}.
$$

Replacing $\theta$ by $\theta+2\pi$ reverses both sine and cosine, so every entry changes sign. In particular, a pure $2\pi$ rotation gives **$D^{(1/2)}=-I$**, while a $4\pi$ rotation gives $I$.

Finally, the [Adjoint double cover from SU(2) to SO(3)](../../../lie-theory.md#adjoint-double-cover-from-su-2-to-so-3) is surjective by the axis-angle construction. Its kernel consists of matrices commuting with all Pauli matrices, hence scalar matrices; within [SU(2)](../../../topological-group.md#su-2-group) these are $\pm I$. Thus

$$
\boxed{SO(3)\cong SU(2)/\{\pm I\}.}
$$

Their [Lie algebras](../../../lie-algebra.md) are isomorphic, but their global topology and representations differ. In [spin](../../../quantum-mechanics.md#spin) $j$, the central element $-I$ acts as $(-1)^{2j}I$, so exactly the integer-spin representations descend to ordinary [SO(3)](../../../linear-algebra.md#so-3-group) representations. This is the [descent of an SU(2) representation to SO(3)](../../../lie-theory.md#descent-of-an-su-2-representation-to-so-3) criterion.

## 3

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $V=\mathbb C^3$ be the defining [SU(3)](../../../topological-group.md#su-3-group) representation. A [mixed SU(3) tensor representation](../../../topological-group.md#mixed-su-3-tensor-representation) belongs to $V^{\otimes k}\otimes(V^*)^{\otimes l}$, with transformation law

$$
T'^{\alpha_1\ldots\alpha_k}_{\beta_1\ldots\beta_l}
=U^{\alpha_1}{}_{\gamma_1}\cdots U^{\alpha_k}{}_{\gamma_k}
(U^{-1})^{\delta_1}{}_{\beta_1}\cdots(U^{-1})^{\delta_l}{}_{\beta_l}
T^{\gamma_1\ldots\gamma_k}_{\delta_1\ldots\delta_l}.
$$

The unrestricted [tensor](../../../linear-algebra.md#tensor) has [dimension](../../../vector-space.md#dimension-vector-space) $3^{k+l}$. The upper and lower counts are independent; setting them equal would lose part of the printed generality.

For an irreducible [tensor](../../../linear-algebra.md#tensor), impose the appropriate [Young symmetrizer](../../../representation-theory-of-the-symmetric-group.md#young-symmetrizer) on each set of indices and subtract all upper-lower contractions. Antisymmetric pairs can be converted using the invariant alternating [tensor](../../../linear-algebra.md#tensor), since $\bigwedge^2\mathbf3\cong\overline{\mathbf3}$ and $\bigwedge^2\overline{\mathbf3}\cong\mathbf3$. A full alternating triple is a singlet because $\det U=1$. [Traces](../../../linear-algebra.md#matrix-trace) use the invariant [Kronecker delta](../../../linear-algebra.md#kronecker-delta) and yield lower-rank [tensors](../../../linear-algebra.md#tensor). Repeating these operations gives invariant irreducible subspaces, with multiplicities retained.

An explicit algorithm for the complete decomposition starts at $(p,q)=(0,0)$, [tensors](../../../linear-algebra.md#tensor) with $\mathbf3$ exactly $k$ times, and then with $\overline{\mathbf3}$ exactly $l$ times. At each step apply

$$
(p,q)\otimes(1,0)=(p+1,q)\oplus(p-1,q+1)\oplus(p,q-1),
$$



$$
(p,q)\otimes(0,1)=(p,q+1)\oplus(p+1,q-1)\oplus(p-1,q),
$$

omitting terms with negative labels and adding multiplicities of coincident terms. The first is the [sl3 highest-weight tensor rule](../../../lie-algebra.md#sl3-highest-weight-tensor-rule): a Young diagram of row lengths $(p+q,q,0)$ gains a box in one of its three rows. The third-row term loses a [determinant](../../../linear-algebra.md#determinant) column of height three, leaving labels $(p,q-1)$. The second rule follows by conjugation, which exchanges $p$ and $q$. Thus the procedure determines all constituents of the general [tensor](../../../linear-algebra.md#tensor), not just one selected symmetry type.

The separately symmetric, traceless component has labels $(k,l)$. Before imposing [traces](../../../linear-algebra.md#matrix-trace) its [dimension](../../../vector-space.md#dimension-vector-space) is $\binom{k+2}{2}\binom{l+2}{2}$. The contraction map has target the separately [symmetric tensors](../../../linear-algebra.md#symmetric-tensor) of degrees $(k-1,l-1)$ and is onto: in polynomial coordinates it is $\sum_i\partial_{x_i}\partial_{y_i}$, the adjoint of multiplication by $\sum_ix_iy_i$ in the monomial-factorial [inner product](../../../linear-algebra.md#inner-product). Multiplication is injective, so the adjoint is surjective. Hence the [symmetric traceless SU(3) tensor representation](../../../topological-group.md#symmetric-traceless-su-3-tensor-representation) has [dimension](../../../vector-space.md#dimension-vector-space)

$$
\boxed{d(k,l)=\binom{k+2}{2}\binom{l+2}{2}-\binom{k+1}{2}\binom{l+1}{2}
=\frac{(k+1)(l+1)(k+l+2)}2.}
$$

For $k=0$ or $l=0$ the subtracted term is zero. The highest [tensor](../../../linear-algebra.md#tensor) $e_1^{\otimes k}\otimes(e^3)^{\otimes l}$ is trace-free and has [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $k\omega_1+l\omega_2$. The three positive-root factors in the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) are $k+1$, $l+1$ and $(k+l+2)/2$, giving exactly the kernel [dimension](../../../vector-space.md#dimension-vector-space) above. Thus the whole symmetric traceless kernel is that irreducible constituent.

There is a genuine distinction between this highest-weight constituent and the literal largest-dimensional constituent. For example, $\mathbf3^{\otimes5}$ contains $(3,1)$, obtained by antisymmetrizing one pair, with [dimension](../../../vector-space.md#dimension-vector-space) $24$, whereas the fully symmetric $(5,0)$ has [dimension](../../../vector-space.md#dimension-vector-space) $21$. Thus $d(k,l)$ cannot be the answer to “largest [dimension](../../../vector-space.md#dimension-vector-space)” for every unrestricted pair of counts.

The [maximal dimension in mixed SU(3) tensor powers](../../../topological-group.md#maximal-dimension-in-mixed-su-3-tensor-powers) can nevertheless be determined exactly. Every constituent [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) differs from $k\omega_1+l\omega_2$ by $a\alpha_1+b\alpha_2$ with nonnegative integers $a,b$, where $\alpha_1=2\omega_1-\omega_2$ and $\alpha_2=-\omega_1+2\omega_2$. Its labels therefore satisfy

$$
p=k-2a+b\ge0,\qquad q=l+a-2b\ge0.
$$

If both $a,b$ are positive, subtracting $c=\min(a,b)$ from both increases the labels to $(p+c,q+c)$, whose [dimension](../../../vector-space.md#dimension-vector-space) is strictly larger. The resulting boundary labels occur in the [tensor](../../../linear-algebra.md#tensor): use $a$ disjoint antisymmetric upper pairs or $b$ disjoint antisymmetric lower pairs, and then take the separately symmetric traceless component. Consequently the exact answer is the finite formula

$$
\boxed{D_{\max}(k,l)=\max\left\{
\max_{0\le a\le\lfloor k/2\rfloor}d(k-2a,l+a),\quad
\max_{0\le b\le\lfloor l/2\rfloor}d(k+b,l-2b)\right\}.}
$$

This supplies a practical closed finite computation for arbitrary $k,l$. To reduce it to at most four evaluations, put $K=k+1$, $L=l+1$ and $r=1+\sqrt3$. The first continuous maximum is at $a_*=(K-rL)/(2+r)$, clipped to $[0,k/2]$; test its two neighbouring allowed integers. The second is similarly at $b_*=(L-rK)/(2+r)$, clipped to $[0,l/2]$. Indeed differentiating the first cubic gives a derivative with the sign of $(K-2a)^2-2(K-2a)(L+a)-2(L+a)^2$, which changes sign once at that root. For equal upper and lower counts, both maxima are at zero and the familiar result is $(k+1)^3$.

For three [quarks](../../../standard-model.md#quark), the unconstrained flavour product is

$$
\mathbf3\otimes\mathbf3\otimes\mathbf3
=(\mathbf6\oplus\overline{\mathbf3})\otimes\mathbf3
=\mathbf{10}_{[3]}\oplus\mathbf8_{[21]}\oplus\mathbf8_{[21]}\oplus\mathbf1_{[111]}.
$$

The brackets indicate permutation symmetry: symmetric, mixed, and alternating. The [three-quark colour singlet](../../../physics.md#three-quark-colour-singlet) is proportional to $\epsilon_{abc}$ and is alternating. The [fermion](../../../quantum-mechanics.md#fermion) wavefunction must be alternating overall. In the usual spatially symmetric ground-state S-wave, the spin-flavour part must therefore be symmetric.

The three-spin-one-half space has a symmetric spin-$3/2$ sector and mixed-symmetry spin-$1/2$ sectors; it has no fully alternating sector because $\bigwedge^3\mathbb C^2=0$. Symmetric flavour can pair with symmetric [spin](../../../quantum-mechanics.md#spin), giving the [baryon decuplet](../../../standard-model.md#baryon-decuplet) of [spin](../../../quantum-mechanics.md#spin) $3/2$. The flavour-octet multiplicity space and the spin-$1/2$ multiplicity space both transform as the two-dimensional standard representation of the [symmetric group](../../../finite-group-theory.md#symmetric-group). Their product contains exactly one symmetric combination: its characters at the identity, a transposition and a three-cycle are $4,0,1$, so the symmetric multiplicity is $(4+3\cdot0+2\cdot1)/6=1$. This gives one [baryon octet](../../../standard-model.md#baryon-octet) of [spin](../../../quantum-mechanics.md#spin) $1/2$. Alternating singlet flavour would need alternating [spin](../../../quantum-mechanics.md#spin) to make the spin-flavour part symmetric, and that sector does not exist. Therefore the [Pauli constraint on three-quark flavour multiplets](../../../physics.md#pauli-constraint-on-three-quark-flavour-multiplets) yields

$$
\boxed{\mathbf8\text{ with }J^P=\tfrac12^+,\qquad\mathbf{10}\text{ with }J^P=\tfrac32^+,\qquad\text{no flavour singlet in the symmetric spatial ground state}.}
$$

The spin-flavour [dimension](../../../vector-space.md#dimension-vector-space) check is $8\cdot2+10\cdot4=56=\dim\operatorname{Sym}^3\mathbb C^6$, the [symmetric spin-flavour SU6 representation](../../../physics.md#symmetric-spin-flavour-su6-representation).

The spatial-symmetry qualification matters if the wording is interpreted as total $L=0$ alone. Rotationally scalar excited orbital functions can have mixed permutation symmetry. For example, the two independent differences among $r_{12}^2,r_{23}^2,r_{31}^2$, multiplied by a symmetric radial factor, span such a space while remaining rotational scalars. Combining this standard permutation representation with the spin-$1/2$ standard representation gives an alternating spin-orbital combination; multiplying by alternating singlet flavour makes it symmetric, and the colour factor restores overall fermionic antisymmetry. Thus total $L=0$ without a symmetric ground-state orbital assumption would not by itself exclude a singlet.

For a quark-antiquark pair, colour singletness selects the contraction $\delta^a{}_b$, and the independent flavour product gives

$$
\boxed{\mathbf3_F\otimes\overline{\mathbf3}_F=\mathbf8_F\oplus\mathbf1_F,\qquad
\tfrac12\otimes\tfrac12=0\oplus1.}
$$

[Quark](../../../standard-model.md#quark) and [antiquark](../../../standard-model.md#antiquark) are distinguishable, so there is no three-identical-quark exclusion of either flavour multiplet or either [spin](../../../quantum-mechanics.md#spin). Both the octet and singlet admit [spin](../../../quantum-mechanics.md#spin) singlets and [spin](../../../quantum-mechanics.md#spin) triplets. Their [baryon number](../../../standard-model.md#baryon-number) is zero. The flavour octet has rows $(Y,I)=(1,1/2),(0,1),(0,0),(-1,1/2)$, while the singlet has $(Y,I)=(0,0)$. The octet's zero-isospin state is $(u\bar u+d\bar d-2s\bar s)/\sqrt6$, and the singlet is $(u\bar u+d\bar d+s\bar s)/\sqrt3$. Each row contains all $I_3=-I,\ldots,I$, and [electric charge](../../../electromagnetism.md#electric-charge) is $Q=I_3+Y/2$.

For ground-state [mesons](../../../physics.md#meson) with $L=0$, opposite intrinsic quark-antiquark parities give $P=-1$. The neutral self-conjugate states have [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) $C=(-1)^{L+S}$, so **both flavour multiplets occur as $0^{-+}$ [pseudoscalar mesons](../../../physics.md#pseudoscalar-meson) and $1^{--}$ [vector mesons](../../../physics.md#vector-meson)**, forming a flavour nonet in each channel. Charged and open-flavour states have no individual charge-conjugation [eigenvalue](../../../linear-operator-theory.md#eigenvalue). The [meson](../../../physics.md#meson) request does not restrict orbital excitation: in general $J=|L-S|,\ldots,L+S$, $P=(-1)^{L+1}$, and the same formula for $C$ applies where defined. Thus the flavour representations stay $\mathbf1\oplus\mathbf8$, with these additional orbital-spin quantum numbers.

## 4

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [SU(2) matrix](../../../topological-group.md#su-2-matrix) has the form $\begin{pmatrix}a&b\\-\overline b&\overline a\end{pmatrix}$ with $|a|^2+|b|^2=1$. Comparing this with the Pauli expansion gives

$$
a=u_0+iu_3,\qquad b=u_2+iu_1.
$$

Consequently all four Pauli coefficients must be real, and their norm condition is

$$
\boxed{u_0,u_1,u_2,u_3\in\mathbb R,\qquad u_0^2+u_1^2+u_2^2+u_3^2=1.}
$$

Conversely, the [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives $AA^\dagger=(u_0^2+|\mathbf u|^2)I$ and $\det A=u_0^2+|\mathbf u|^2$, so these conditions imply unitarity and [determinant](../../../linear-algebra.md#determinant) one. For complex coefficients the [determinant](../../../linear-algebra.md#determinant) equation alone would not imply unitarity.

On either open hemisphere,

$$
\boxed{u_0=\pm\sqrt{1-|\mathbf u|^2},\qquad|\mathbf u|<1.}
$$

Both signs are necessary globally. The two hemispheres meet along $u_0=0$, and the full four-coefficient constraint is exactly the unit sphere in $\mathbb R^4$. The coefficient map and its inverse are smooth, establishing [SU(2) as the three-sphere](../../../topological-group.md#su-2-as-the-three-sphere) as a [manifold](../../../topology.md#topological-manifold), not merely a [dimension](../../../vector-space.md#dimension-vector-space) count.

For two real coefficient quadruples, expanding the [matrix](../../../vector-space.md#matrix) product with the [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives

$$
w_0=u_0v_0-\mathbf u\cdot\mathbf v,\qquad
\mathbf w=v_0\mathbf u+u_0\mathbf v-\mathbf u\times\mathbf v.
$$

For an infinitesimal second factor, $v_0=1+O(|\mathbf v|^2)$. Therefore

$$
du_i=u_0v_i+\epsilon_{jki}v_ju_k
=\boxed{v_j\mu_{ji},\qquad\mu_{ji}=u_0\delta_{ij}+u_k\epsilon_{jki}},
$$

while $du_0=-u_iv_i$. These variations are tangent to the unit sphere because $u_0du_0+u_idu_i=0$.

On a hemisphere, differentiation of the norm constraint gives $\partial_{u_i}u_0=-u_i/u_0$, and hence

$$
\partial_{u_i}A=-\frac{u_i}{u_0}I+i\sigma_i.
$$

Contracting with the [Pauli-coordinate left-invariant vector fields on SU(2)](../../../lie-theory.md#pauli-coordinate-left-invariant-vector-fields-on-su-2) and using $\mu_{ji}u_i=u_0u_j$ gives

$$
T_jA=i\mu_{ji}\partial_{u_i}A
=-iu_jI-u_0\sigma_j-u_k\epsilon_{jki}\sigma_i.
$$

The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives exactly the same expression for $-A\sigma_j$, so

$$
\boxed{T_jA=-A\sigma_j.}
$$

It follows that

$$
[T_i,T_j]A=A\sigma_i\sigma_j-A\sigma_j\sigma_i
=A[\sigma_i,\sigma_j]=2i\epsilon_{ijk}A\sigma_k
=-2i\epsilon_{ijk}T_kA.
$$

This uses the [Pauli matrix commutator identity](../../../algebra.md#pauli-matrix-commutator-identity). The [commutator](../../../lie-algebra.md#commutator) of two first-order [vector fields](../../../calculus.md#vector-field) is again a [vector field](../../../calculus.md#vector-field), and the [matrix](../../../vector-space.md#matrix) entries of $A$ span the four coordinate functions $u_0,u_1,u_2,u_3$. Equality of their actions on these entries determines the tangent field. Therefore

$$
\boxed{[T_i,T_j]=-2i\epsilon_{ijk}T_k.}
$$

The real tangent field underneath $T_j$ is generated by the flow $A\mapsto A e^{it\sigma_j}$; left multiplication transports that tangent consistently, explaining its left invariance. The rescaled generators $-T_j/2$ have the usual positive-sign angular-momentum [commutator](../../../lie-algebra.md#commutator).

To determine the [Haar measure](../../../measure-theory.md#haar-measure), compute the metric induced from the unit three-sphere. Since $du_0=-u_i\,du_i/u_0$, its line element is

$$
ds^2=du_0^2+\sum_i du_i^2
=\left(\delta_{ij}+\frac{u_iu_j}{u_0^2}\right)du_i\,du_j.
$$

The rank-one [matrix determinant lemma](../../../linear-algebra.md#matrix-determinant-lemma) gives

$$
\det g=1+\frac{|\mathbf u|^2}{u_0^2}=\frac1{u_0^2}.
$$

Thus the [Pauli-coordinate Haar measure on SU(2)](../../../measure-theory.md#pauli-coordinate-haar-measure-on-su-2) is

$$
\boxed{d\rho(\mathbf u)=\sqrt{\det g}\,d^3u=\frac{d^3u}{|u_0|},}
$$

up to an overall normalization. To check its group invariance, fix one unit coefficient quadruple and multiply by it. The product formulas define a linear transformation of the other quadruple. The norm of a product is the product of norms, as follows either from $AA^\dagger$ or directly from the dot and cross products. Fixed multiplication by a unit quadruple is therefore an orthogonal transformation of $\mathbb R^4$. It preserves the round sphere metric and volume, on both the left and the right, proving that this is the invariant measure.

The same density can be checked directly against the [vector fields](../../../calculus.md#vector-field). On a fixed hemisphere, $u_0/|u_0|$ is constant, and

$$
\partial_{u_i}\left(\frac{\mu_{ji}}{|u_0|}\right)
=\partial_{u_j}\left(\frac{u_0}{|u_0|}\right)
+\epsilon_{jki}\partial_{u_i}\left(\frac{u_k}{|u_0|}\right)=0.
$$

The second term vanishes because its contractions involve either $\delta_{ik}$ or $u_iu_k$, both symmetric in $i,k$. Thus the density has zero divergence along every invariant tangent direction.

The hemisphere chart becomes singular at the equator, but its volume is finite:

$$
\int_{|\mathbf u|<1}\frac{d^3u}{\sqrt{1-|\mathbf u|^2}}
=4\pi\int_0^1\frac{r^2\,dr}{\sqrt{1-r^2}}
=4\pi\int_0^{\pi/2}\sin^2\chi\,d\chi=\pi^2.
$$

Both hemispheres give total volume $2\pi^2$, so probability-normalized [Haar measure](../../../measure-theory.md#haar-measure) is $d^3u/(2\pi^2|u_0|)$ on each hemisphere. Finally, the three-sphere is closed and bounded in $\mathbb R^4$, hence compact; its smooth identification with [SU(2)](../../../topological-group.md#su-2-group) proves that **$SU(2)$ is a [compact group](../../../topological-group.md#compact-group)**. The finite integral reflects this compactness, and the equatorial divergence is only a coordinate artefact.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
