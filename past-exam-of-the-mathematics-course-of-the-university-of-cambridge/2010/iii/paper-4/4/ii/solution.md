<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Replace the [determinant](../../../../../../determinant.md) condition by preservation of a nondegenerate [alternating bilinear form](../../../../../../alternating-bilinear-form.md) $B$ on $F^{2m}$. In a [symplectic basis](../../../../../../symplectic-basis.md) the [symplectic group over a finite field](../../../../../../symplectic-group-over-a-finite-field.md) is

$$
Sp_{2m}(q)=\{g\in GL_{2m}(q):g^{\mathsf T}Jg=J\},
\qquad J=\begin{pmatrix}0&I_m\\-I_m&0\end{pmatrix}.
$$

To count [symplectic bases](../../../../../../symplectic-basis.md), choose the first [vector](../../../../../../vector.md) $e$ in $q^{2m}-1$ ways, then choose $f$ with $B(e,f)=1$ in $q^{2m-1}$ ways. Their span is nondegenerate; its [symplectic orthogonal complement](../../../../../../symplectic-orthogonal-complement.md) has [dimension](../../../../../../dimension-vector-space.md) $2m-2$ and supplies the rest of the [basis](../../../../../../basis.md). The resulting recurrence gives the [finite symplectic group order](../../../../../../finite-symplectic-group-order.md)

$$
\boxed{|Sp_{2m}(q)|=q^{m^2}\prod_{i=1}^m(q^{2i}-1).}
$$

The elementary replacements are [symplectic transvections](../../../../../../symplectic-transvection.md)

$$
T_{v,c}(x)=x+cB(x,v)v,\qquad v\ne0,\ c\in F.
$$

Expanding $B(Tx,Ty)$ shows that the two cross terms cancel and the last term vanishes because $B(v,v)=0$. Thus these maps preserve $B$; their inverses are $T_{v,-c}$.

We need both generation and primitivity to use the argument from part (i). For nonzero [vectors](../../../../../../vector.md) $v,w$ with $B(v,w)\ne0$, the [symplectic transvection](../../../../../../symplectic-transvection.md) with direction $w-v$ and parameter $1/B(v,w)$ sends $v$ to $w$. When $B(v,w)=0$, choose $z$ nonorthogonal to both and use two such steps. Such $z$ exists because two proper [hyperplanes](../../../../../../hyperplane.md) cannot cover a [vector space](../../../../../../vector-space-split.md): if the two linear forms are independent prescribe both values to be one, and if dependent prescribe either a nonzero value. Hence [symplectic transvections](../../../../../../symplectic-transvection.md) act transitively on nonzero [vectors](../../../../../../vector.md).

They generate the whole [symplectic group over a finite field](../../../../../../symplectic-group-over-a-finite-field.md). Indeed first use them to make a given symplectic transformation fix $e_1$. Its image $f'$ of $f_1$ still satisfies $B(e_1,f')=1$. A [symplectic transvection](../../../../../../symplectic-transvection.md) with direction $f_1-f'$ fixes $e_1$ and sends $f'$ to $f_1$ if the pairing is nonzero. If that pairing is zero, pass through $f'+ce_1$ for any $c\ne0$: it has nonzero pairing with both partners, and both required directions lie in $e_1^\perp$. We have now fixed the first [hyperbolic pair](../../../../../../hyperbolic-pair.md), and induction applies in its nondegenerate orthogonal complement. The final two-dimensional case is exactly the elementary generation of $SL_2(q)=Sp_2(q)$ proved in part (i).

For a fixed [projective point](../../../../../../projective-point.md) $\langle e\rangle$, the [symplectic transvections](../../../../../../symplectic-transvection.md) $T_{e,c}$ form an abelian [subgroup](../../../../../../subgroup.md) normal in its [stabilizer subgroup](../../../../../../stabilizer-subgroup.md); conjugation scales $c$ by the square of the scalar multiplying $e$. Their conjugates supply all [symplectic transvections](../../../../../../symplectic-transvection.md). A central element commutes with every [symplectic transvection](../../../../../../symplectic-transvection.md), so it preserves every direction line and must be scalar. Conversely scalars commute with the whole group. The kernel of the projective action consists of scalar [matrices](../../../../../../matrix.md), and preservation of $B$ restricts the scalar to $\lambda^2=1$. Thus the [center of a group](../../../../../../center-of-a-group.md) has size $\gcd(2,q-1)$ and the [projective symplectic group over a finite field](../../../../../../projective-symplectic-group-over-a-finite-field.md) acts faithfully.

For $m\ge2$ the [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) has precisely three orbits: its fixed point, the other points in $e^\perp$, and the points outside $e^\perp$. Transitivity on each follows by extending, respectively, an independent isotropic pair or a [hyperbolic pair](../../../../../../hyperbolic-pair.md) to a [symplectic basis](../../../../../../symplectic-basis.md). Write

$$
N=\frac{q^{2m}-1}{q-1},\qquad
h=\frac{q^{2m-1}-1}{q-1}.
$$

A nontrivial proper block through the fixed point would be a union of these [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) orbits, hence would have size either $h$ or $q^{2m-1}+1$. A block size divides $N$. But $N-qh=1$, so $h>1$ cannot divide $N$, and $N/2<q^{2m-1}+1<N$, excluding the other size. This proves primitivity. For $m=1$ the projective action is the [two-transitive](../../../../../../two-transitive-group-action.md) action of $PSL_2(q)$.

Here is a direct check of [perfectness of finite symplectic groups](../../../../../../perfectness-of-finite-symplectic-groups.md), including the small fields where the diagonal [group commutator](../../../../../../group-commutator.md) needs replacement. If $q>3$, every [symplectic transvection](../../../../../../symplectic-transvection.md) lies in an embedded $SL_2(q)$ on a hyperbolic plane containing its direction, and that [subgroup](../../../../../../subgroup.md) is perfect by part (i). Since the [symplectic transvections](../../../../../../symplectic-transvection.md) generate, the whole [symplectic group over a finite field](../../../../../../symplectic-group-over-a-finite-field.md) is perfect.

For $q=3$ and $m\ge2$, all $T_{v,1}$ are conjugate, so their common image $z$ generates the [abelianization](../../../../../../abelianization.md) and satisfies $3z=0$. Choose independent perpendicular [vectors](../../../../../../vector.md) $e,f$. The four commuting [symplectic transvections](../../../../../../symplectic-transvection.md) with directions $e,f,e+f,e-f$ and parameter one multiply to the identity: the sum of their rank-one [matrices](../../../../../../matrix.md) is zero in characteristic 3. Thus also $4z=0$, giving $z=0$.

For $q=2$ and $m\ge3$, use the seven nonzero [vectors](../../../../../../vector.md) of a three-dimensional [isotropic subspace of a symplectic vector space](../../../../../../isotropic-subspace-of-a-symplectic-vector-space.md). Their [symplectic transvections](../../../../../../symplectic-transvection.md) commute, and their product is the identity. To see this explicitly, write a [vector](../../../../../../vector.md) in three isotropic [basis](../../../../../../basis.md) coordinates: in the sum of the outer products $vv^{\mathsf T}$ each diagonal coefficient occurs four times and each off-diagonal coefficient twice, all zero in characteristic 2. The common [abelianization](../../../../../../abelianization.md) image $z$ therefore satisfies $2z=7z=0$. Again the group is perfect.

The simplicity argument from part (i) now applies to the projective [symplectic group over a finite field](../../../../../../symplectic-group-over-a-finite-field.md). The remaining exceptional group besides $Sp_2(2)$ and $PSp_2(3)$ is $Sp_4(2)$. It is not simple: it is isomorphic to $S_6$. One can verify this identification without assuming it. On $F_2^4$ set

$$
Q_0(x_1,x_2,y_1,y_2)=x_1y_1+x_2y_2,\qquad
Q_a(v)=Q_0(v)+B(a,v).
$$

These are all 16 [quadratic forms](../../../../../../quadratic-form.md) with polar form $B$; the [Arf invariant of a quadratic form](../../../../../../arf-invariant-of-a-quadratic-form.md) gives $\operatorname{Arf}(Q_a)=Q_0(a)$. There are six with invariant one. The [symplectic group over a finite field](../../../../../../symplectic-group-over-a-finite-field.md) permutes these six forms. Differences of their parameter [vectors](../../../../../../vector.md) span $F_2^4$: writing $e_i,f_i$ for the [symplectic basis](../../../../../../symplectic-basis.md), the six parameters are

$$
e_1+f_1,\ e_1+f_1+e_2,\ e_1+f_1+f_2,\
e_2+f_2,\ e_2+f_2+e_1,\ e_2+f_2+f_1.
$$

Their pairwise differences include each of $e_1,e_2,f_1,f_2$. An element fixing all six forms therefore fixes all linear forms $B(a-b,-)$, hence is the identity. This gives a faithful action on six objects; the group order is 720, so its image is all of $S_6$. Consequently

$$
\boxed{|PSp_{2m}(q)|=\frac{q^{m^2}\prod_{i=1}^m(q^{2i}-1)}{\gcd(2,q-1)},\qquad
PSp_{2m}(q)\text{ simple except }(m,q)=(1,2),(1,3),(2,2).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
