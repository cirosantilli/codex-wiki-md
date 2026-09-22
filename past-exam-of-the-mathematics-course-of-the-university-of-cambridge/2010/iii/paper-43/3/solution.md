<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $V=\mathbb C^3$ be the defining [SU(3)](../../../../../su-3-group.md) representation. A [mixed SU(3) tensor representation](../../../../../mixed-su-3-tensor-representation.md) belongs to $V^{\otimes k}\otimes(V^*)^{\otimes l}$, with transformation law

$$
T'^{\alpha_1\ldots\alpha_k}_{\beta_1\ldots\beta_l}
=U^{\alpha_1}{}_{\gamma_1}\cdots U^{\alpha_k}{}_{\gamma_k}
(U^{-1})^{\delta_1}{}_{\beta_1}\cdots(U^{-1})^{\delta_l}{}_{\beta_l}
T^{\gamma_1\ldots\gamma_k}_{\delta_1\ldots\delta_l}.
$$

The unrestricted [tensor](../../../../../tensor.md) has [dimension](../../../../../dimension-vector-space.md) $3^{k+l}$. The upper and lower counts are independent; setting them equal would lose part of the printed generality.

For an irreducible [tensor](../../../../../tensor.md), impose the appropriate [Young symmetrizer](../../../../../young-symmetrizer.md) on each set of indices and subtract all upper-lower contractions. Antisymmetric pairs can be converted using the invariant alternating [tensor](../../../../../tensor.md), since $\bigwedge^2\mathbf3\cong\overline{\mathbf3}$ and $\bigwedge^2\overline{\mathbf3}\cong\mathbf3$. A full alternating triple is a singlet because $\det U=1$. [Traces](../../../../../matrix-trace.md) use the invariant [Kronecker delta](../../../../../kronecker-delta.md) and yield lower-rank [tensors](../../../../../tensor.md). Repeating these operations gives invariant irreducible subspaces, with multiplicities retained.

An explicit algorithm for the complete decomposition starts at $(p,q)=(0,0)$, [tensors](../../../../../tensor.md) with $\mathbf3$ exactly $k$ times, and then with $\overline{\mathbf3}$ exactly $l$ times. At each step apply

$$
(p,q)\otimes(1,0)=(p+1,q)\oplus(p-1,q+1)\oplus(p,q-1),
$$



$$
(p,q)\otimes(0,1)=(p,q+1)\oplus(p+1,q-1)\oplus(p-1,q),
$$

omitting terms with negative labels and adding multiplicities of coincident terms. The first is the [sl3 highest-weight tensor rule](../../../../../sl3-highest-weight-tensor-rule.md): a Young diagram of row lengths $(p+q,q,0)$ gains a box in one of its three rows. The third-row term loses a [determinant](../../../../../determinant.md) column of height three, leaving labels $(p,q-1)$. The second rule follows by conjugation, which exchanges $p$ and $q$. Thus the procedure determines all constituents of the general [tensor](../../../../../tensor.md), not just one selected symmetry type.

The separately symmetric, traceless component has labels $(k,l)$. Before imposing [traces](../../../../../matrix-trace.md) its [dimension](../../../../../dimension-vector-space.md) is $\binom{k+2}{2}\binom{l+2}{2}$. The contraction map has target the separately [symmetric tensors](../../../../../symmetric-tensor.md) of degrees $(k-1,l-1)$ and is onto: in polynomial coordinates it is $\sum_i\partial_{x_i}\partial_{y_i}$, the adjoint of multiplication by $\sum_ix_iy_i$ in the monomial-factorial [inner product](../../../../../inner-product.md). Multiplication is injective, so the adjoint is surjective. Hence the [symmetric traceless SU(3) tensor representation](../../../../../symmetric-traceless-su-3-tensor-representation.md) has [dimension](../../../../../dimension-vector-space.md)

$$
\boxed{d(k,l)=\binom{k+2}{2}\binom{l+2}{2}-\binom{k+1}{2}\binom{l+1}{2}
=\frac{(k+1)(l+1)(k+l+2)}2.}
$$

For $k=0$ or $l=0$ the subtracted term is zero. The highest [tensor](../../../../../tensor.md) $e_1^{\otimes k}\otimes(e^3)^{\otimes l}$ is trace-free and has [highest weight](../../../../../highest-weight-of-a-representation.md) $k\omega_1+l\omega_2$. The three positive-root factors in the [Weyl dimension formula](../../../../../weyl-dimension-formula.md) are $k+1$, $l+1$ and $(k+l+2)/2$, giving exactly the kernel [dimension](../../../../../dimension-vector-space.md) above. Thus the whole symmetric traceless kernel is that irreducible constituent.

There is a genuine distinction between this highest-weight constituent and the literal largest-dimensional constituent. For example, $\mathbf3^{\otimes5}$ contains $(3,1)$, obtained by antisymmetrizing one pair, with [dimension](../../../../../dimension-vector-space.md) $24$, whereas the fully symmetric $(5,0)$ has [dimension](../../../../../dimension-vector-space.md) $21$. Thus $d(k,l)$ cannot be the answer to “largest [dimension](../../../../../dimension-vector-space.md)” for every unrestricted pair of counts.

The [maximal dimension in mixed SU(3) tensor powers](../../../../../maximal-dimension-in-mixed-su-3-tensor-powers.md) can nevertheless be determined exactly. Every constituent [highest weight](../../../../../highest-weight-of-a-representation.md) differs from $k\omega_1+l\omega_2$ by $a\alpha_1+b\alpha_2$ with nonnegative integers $a,b$, where $\alpha_1=2\omega_1-\omega_2$ and $\alpha_2=-\omega_1+2\omega_2$. Its labels therefore satisfy

$$
p=k-2a+b\ge0,\qquad q=l+a-2b\ge0.
$$

If both $a,b$ are positive, subtracting $c=\min(a,b)$ from both increases the labels to $(p+c,q+c)$, whose [dimension](../../../../../dimension-vector-space.md) is strictly larger. The resulting boundary labels occur in the [tensor](../../../../../tensor.md): use $a$ disjoint antisymmetric upper pairs or $b$ disjoint antisymmetric lower pairs, and then take the separately symmetric traceless component. Consequently the exact answer is the finite formula

$$
\boxed{D_{\max}(k,l)=\max\left\{
\max_{0\le a\le\lfloor k/2\rfloor}d(k-2a,l+a),\quad
\max_{0\le b\le\lfloor l/2\rfloor}d(k+b,l-2b)\right\}.}
$$

This supplies a practical closed finite computation for arbitrary $k,l$. To reduce it to at most four evaluations, put $K=k+1$, $L=l+1$ and $r=1+\sqrt3$. The first continuous maximum is at $a_*=(K-rL)/(2+r)$, clipped to $[0,k/2]$; test its two neighbouring allowed integers. The second is similarly at $b_*=(L-rK)/(2+r)$, clipped to $[0,l/2]$. Indeed differentiating the first cubic gives a derivative with the sign of $(K-2a)^2-2(K-2a)(L+a)-2(L+a)^2$, which changes sign once at that root. For equal upper and lower counts, both maxima are at zero and the familiar result is $(k+1)^3$.

For three [quarks](../../../../../quark.md), the unconstrained flavour product is

$$
\mathbf3\otimes\mathbf3\otimes\mathbf3
=(\mathbf6\oplus\overline{\mathbf3})\otimes\mathbf3
=\mathbf{10}_{[3]}\oplus\mathbf8_{[21]}\oplus\mathbf8_{[21]}\oplus\mathbf1_{[111]}.
$$

The brackets indicate permutation symmetry: symmetric, mixed, and alternating. The [three-quark colour singlet](../../../../../three-quark-colour-singlet.md) is proportional to $\epsilon_{abc}$ and is alternating. The [fermion](../../../../../fermion.md) wavefunction must be alternating overall. In the usual spatially symmetric ground-state S-wave, the spin-flavour part must therefore be symmetric.

The three-spin-one-half space has a symmetric spin-$3/2$ sector and mixed-symmetry spin-$1/2$ sectors; it has no fully alternating sector because $\bigwedge^3\mathbb C^2=0$. Symmetric flavour can pair with symmetric [spin](../../../../../spin.md), giving the [baryon decuplet](../../../../../baryon-decuplet.md) of [spin](../../../../../spin.md) $3/2$. The flavour-octet multiplicity space and the spin-$1/2$ multiplicity space both transform as the two-dimensional standard representation of the [symmetric group](../../../../../symmetric-group.md). Their product contains exactly one symmetric combination: its characters at the identity, a transposition and a three-cycle are $4,0,1$, so the symmetric multiplicity is $(4+3\cdot0+2\cdot1)/6=1$. This gives one [baryon octet](../../../../../baryon-octet.md) of [spin](../../../../../spin.md) $1/2$. Alternating singlet flavour would need alternating [spin](../../../../../spin.md) to make the spin-flavour part symmetric, and that sector does not exist. Therefore the [Pauli constraint on three-quark flavour multiplets](../../../../../pauli-constraint-on-three-quark-flavour-multiplets.md) yields

$$
\boxed{\mathbf8\text{ with }J^P=\tfrac12^+,\qquad\mathbf{10}\text{ with }J^P=\tfrac32^+,\qquad\text{no flavour singlet in the symmetric spatial ground state}.}
$$

The spin-flavour [dimension](../../../../../dimension-vector-space.md) check is $8\cdot2+10\cdot4=56=\dim\operatorname{Sym}^3\mathbb C^6$, the [symmetric spin-flavour SU6 representation](../../../../../symmetric-spin-flavour-su6-representation.md).

The spatial-symmetry qualification matters if the wording is interpreted as total $L=0$ alone. Rotationally scalar excited orbital functions can have mixed permutation symmetry. For example, the two independent differences among $r_{12}^2,r_{23}^2,r_{31}^2$, multiplied by a symmetric radial factor, span such a space while remaining rotational scalars. Combining this standard permutation representation with the spin-$1/2$ standard representation gives an alternating spin-orbital combination; multiplying by alternating singlet flavour makes it symmetric, and the colour factor restores overall fermionic antisymmetry. Thus total $L=0$ without a symmetric ground-state orbital assumption would not by itself exclude a singlet.

For a quark-antiquark pair, colour singletness selects the contraction $\delta^a{}_b$, and the independent flavour product gives

$$
\boxed{\mathbf3_F\otimes\overline{\mathbf3}_F=\mathbf8_F\oplus\mathbf1_F,\qquad
\tfrac12\otimes\tfrac12=0\oplus1.}
$$

[Quark](../../../../../quark.md) and [antiquark](../../../../../antiquark.md) are distinguishable, so there is no three-identical-quark exclusion of either flavour multiplet or either [spin](../../../../../spin.md). Both the octet and singlet admit [spin](../../../../../spin.md) singlets and [spin](../../../../../spin.md) triplets. Their [baryon number](../../../../../baryon-number.md) is zero. The flavour octet has rows $(Y,I)=(1,1/2),(0,1),(0,0),(-1,1/2)$, while the singlet has $(Y,I)=(0,0)$. The octet's zero-isospin state is $(u\bar u+d\bar d-2s\bar s)/\sqrt6$, and the singlet is $(u\bar u+d\bar d+s\bar s)/\sqrt3$. Each row contains all $I_3=-I,\ldots,I$, and [electric charge](../../../../../electric-charge.md) is $Q=I_3+Y/2$.

For ground-state [mesons](../../../../../meson.md) with $L=0$, opposite intrinsic quark-antiquark parities give $P=-1$. The neutral self-conjugate states have [charge conjugation](../../../../../charge-conjugation.md) $C=(-1)^{L+S}$, so **both flavour multiplets occur as $0^{-+}$ [pseudoscalar mesons](../../../../../pseudoscalar-meson.md) and $1^{--}$ [vector mesons](../../../../../vector-meson.md)**, forming a flavour nonet in each channel. Charged and open-flavour states have no individual charge-conjugation [eigenvalue](../../../../../eigenvalue.md). The [meson](../../../../../meson.md) request does not restrict orbital excitation: in general $J=|L-S|,\ldots,L+S$, $P=(-1)^{L+1}$, and the same formula for $C$ applies where defined. Thus the flavour representations stay $\mathbf1\oplus\mathbf8$, with these additional orbital-spin quantum numbers.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
