<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A finite [two-transitive group action](../../../../../two-transitive-group-action.md) is transitive on ordered pairs of distinct points. Equivalently, the action is transitive and a point [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is transitive on the remaining points. Its [rank of a transitive permutation group](../../../../../rank-of-a-transitive-permutation-group.md) is two, and the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) gives $n(n-1)\mid |G|$ for degree $n$. Such an action is primitive: a block containing a point and another point must, by the transitivity of the [stabilizer subgroup](../../../../../stabilizer-subgroup.md), contain every point.

These groups illustrate two quite different sources of symmetry. The structural theorem for finite [two-transitive](../../../../../two-transitive-group-action.md) groups says that they have either a regular elementary-abelian [normal subgroup](../../../../../normal-subgroup.md), giving the affine case, or a nonabelian simple [normal subgroup](../../../../../normal-subgroup.md), giving the almost simple case. The full classification of the second case depends on the classification of finite [simple groups](../../../../../simple-group.md); the useful point here is to describe the constructions, actions, and representative families rather than treat two-transitivity as an abstract property of a group without a specified action.

In the affine case let $V$ be a finite [vector space](../../../../../vector-space-split.md) over $\mathbb F_p$ and let $H\le GL(V)$ act transitively on $V\setminus\{0\}$. The [affine two-transitive group](../../../../../affine-two-transitive-group.md)

$$
G=V\rtimes H,\qquad (v,h):x\mapsto v+hx,
$$

is transitive by translations, and the [stabilizer subgroup](../../../../../stabilizer-subgroup.md) of zero is exactly $H$, so it is [two-transitive](../../../../../two-transitive-group-action.md). Conversely, if a [two-transitive](../../../../../two-transitive-group-action.md) group has an abelian minimal [normal subgroup](../../../../../normal-subgroup.md) $V$, normal-subgroup orbits and primitivity make $V$ transitive. An abelian transitive faithful [permutation](../../../../../permutation.md) [subgroup](../../../../../subgroup.md) is regular: an element fixing one point commutes with every element moving that point and hence fixes them all. Minimal normality makes $V$ elementary abelian, since its prime-primary [subgroups](../../../../../subgroup.md) and its [subgroup](../../../../../subgroup.md) of pth powers are characteristic. Conjugation by the [stabilizer subgroup](../../../../../stabilizer-subgroup.md) acts faithfully as linear automorphisms of $V$, and regularity gives $G=V\rtimes G_0$. This recovers precisely the construction above.

Many examples follow at once. The group $AGL_d(q)$ acts on the $q^d$ [vectors](../../../../../vector.md) of $\mathbb F_q^d$; $GL_d(q)$ sends any nonzero [vector](../../../../../vector.md) to any other by a [basis](../../../../../basis.md) map. For $d\ge2$, the [subgroup](../../../../../subgroup.md) $ASL_d(q)$ also gives a [two-transitive](../../../../../two-transitive-group-action.md) action, since the [determinant](../../../../../determinant.md) of a [basis](../../../../../basis.md) map can be adjusted on a second [basis](../../../../../basis.md) [vector](../../../../../vector.md) while retaining the prescribed first [vector](../../../../../vector.md). The affine group with linear part $Sp_{2m}(q)$ gives another family: the nonzero-vector transitivity was proved using [symplectic transvections](../../../../../symplectic-transvection.md) in part 4(ii). Here the additive group of $\mathbb F_q^d$, for $q=p^f$, is an [elementary abelian p-group](../../../../../elementary-abelian-group.md) of rank $fd$.

In particular $AGL_1(q)$ consists of $x\mapsto ax+b$ with $a\ne0$. Given distinct $x,y$ and distinct $u,v$, the equations $ax+b=u$, $ay+b=v$ have the unique solution $a=(v-u)/(y-x)$, $b=u-ax$. Thus this action is [sharply two-transitive](../../../../../sharp-two-transitivity.md), of degree $q$ and order $q(q-1)$. Adding [field automorphisms](../../../../../field-automorphism.md) gives $A\Gamma L_1(q)$, still [two-transitive](../../../../../two-transitive-group-action.md), with elements $x\mapsto ax^{p^i}+b$.

An [almost simple group](../../../../../almost-simple-group.md) lies between a nonabelian [simple group](../../../../../simple-group.md) $T$ and its automorphism group. One must still specify an action: a group can have several [permutation representations](../../../../../permutation-representation.md) with different degrees or different transitivity properties. The natural actions of $S_n$ for $n\ge2$ and $A_n$ for $n\ge4$ are the most familiar examples of a [two-transitive group action](../../../../../two-transitive-group-action.md). For $n\ge5$, the [simple group](../../../../../simple-group.md) $A_n$, a [normal subgroup](../../../../../normal-subgroup.md), places these groups in the almost simple case; the smaller two-transitive examples belong to the affine case. The [symmetric group](../../../../../symmetric-group.md) sends any ordered distinct pair to any other; for the [alternating group](../../../../../alternating-group.md) one can adjust an odd map by swapping two letters outside the target pair. Thus both are [two-transitive](../../../../../two-transitive-group-action.md) in the indicated ranges.

The projective linear examples are just as concrete. The groups $PSL_n(q)$ and $PGL_n(q)$ act two-transitively on

$$
|\mathbb P^{n-1}(\mathbb F_q)|=\frac{q^n-1}{q-1}
$$

points, by the [basis](../../../../../basis.md) and [determinant](../../../../../determinant.md) adjustment argument of part 4(i). Their field-automorphism extensions are also [two-transitive](../../../../../two-transitive-group-action.md). On the [projective line](../../../../../projective-line.md), $PGL_2(q)$ is [sharply three-transitive](../../../../../sharp-three-transitivity.md): three distinct points determine a unique [Möbius transformation](../../../../../mobius-transformation.md). Its degree is $q+1$ and its order is $q(q^2-1)$. For even $q$, $PSL_2(q)=PGL_2(q)$; for odd $q$ the special projective group has half that order and remains [two-transitive](../../../../../two-transitive-group-action.md), but cannot be [three-transitive](../../../../../three-transitive-group-action.md). In projective [dimension](../../../../../dimension-vector-space.md) at least two, triples of distinct points may be collinear or noncollinear, so the natural action is not [three-transitive](../../../../../three-transitive-group-action.md).

The [projective special unitary group over a finite field](../../../../../projective-special-unitary-group-over-a-finite-field.md) $PSU_3(q)$, for $q\ge3$, acts on the isotropic points of a space with a nondegenerate [Hermitian form](../../../../../hermitian-form.md) of [dimension](../../../../../dimension-vector-space.md) three over $\mathbb F_{q^2}$. Its degree and order are

$$
q^3+1,\qquad \frac{q^3(q^3+1)(q^2-1)}{\gcd(3,q+1)}.
$$

For two distinct isotropic lines the [Hermitian form](../../../../../hermitian-form.md) pairing is nonzero, since a three-dimensional nondegenerate Hermitian space has maximal totally isotropic [dimension](../../../../../dimension-vector-space.md) one. Scale their representatives to form a [hyperbolic pair](../../../../../hyperbolic-pair.md) and extend to a [basis](../../../../../basis.md) adapted to the [Hermitian form](../../../../../hermitian-form.md). The corresponding isometry sends one ordered pair to another, and a norm-one scalar on the orthogonal one-dimensional complement adjusts its [determinant](../../../../../determinant.md) without moving the two lines. Thus the special projective unitary action is [two-transitive](../../../../../two-transitive-group-action.md).

Two further families of [simple groups](../../../../../simple-group.md) have analogous rank-two actions:

$$
\begin{array}{c|c|c|c}
\text{family}&q&\text{degree}&\text{order}\\
Sz(q)&2^{2a+1}\ge8&q^2+1&q^2(q^2+1)(q-1)\\
{}^2G_2(q)&3^{2a+1}\ge27&q^3+1&q^3(q^3+1)(q-1)
\end{array}
$$

The [Suzuki group of Lie type](../../../../../suzuki-group-of-lie-type.md) and the [Ree group of type G2](../../../../../ree-group-of-type-g2.md) have [stabilizer subgroups](../../../../../stabilizer-subgroup.md) containing [subgroups](../../../../../subgroup.md) acting regularly on all the other points in these actions; this gives two-transitivity. For example $Sz(8)$ has degree 65 and order 29120. These are exceptional Lie-type families, distinct from the preceding linear and unitary constructions.

The [symplectic group over a finite field](../../../../../symplectic-group-over-a-finite-field.md) in characteristic two has a particularly illuminating pair of [two-transitive](../../../../../two-transitive-group-action.md) actions which are not their projective-vector actions. For $m\ge3$, $Sp_{2m}(2)$ acts on the two classes of [quadratic forms](../../../../../quadratic-form.md) whose polar form is the given [alternating bilinear form](../../../../../alternating-bilinear-form.md), distinguished by the [Arf invariant of a quadratic form](../../../../../arf-invariant-of-a-quadratic-form.md). Their degrees are

$$
2^{m-1}(2^m+1)\quad\text{and}\quad2^{m-1}(2^m-1).
$$

Transitivity on each class follows by choosing [symplectic bases](../../../../../symplectic-basis.md) giving the standard quadratic-form normal forms. Fix a form $Q$. Every other form with the same polar form is $Q_a(x)=Q(x)+B(a,x)$, and has the same [Arf invariant of a quadratic form](../../../../../arf-invariant-of-a-quadratic-form.md) exactly when $Q(a)=0$. The [stabilizer subgroup](../../../../../stabilizer-subgroup.md) of $Q$, an [orthogonal group over a finite field](../../../../../orthogonal-group-over-a-finite-field.md), is transitive on its nonzero [isotropic vectors](../../../../../isotropic-vector.md): extend such a [vector](../../../../../vector.md) to a [hyperbolic pair](../../../../../hyperbolic-pair.md) and map adapted quadratic-form [bases](../../../../../basis.md). It is therefore transitive on the other forms of the same type. This proves two-transitivity of both actions. In particular $Sp_6(2)$ has actions of degrees 28 and 36. The degree-six action of $Sp_4(2)\cong S_6$ in part 4(ii) is the smaller-dimensional precursor.

Finally the [Mathieu groups](../../../../../mathieu-group.md) supply exceptional examples with even higher transitivity:

$$
\begin{array}{c|ccccc}
G&M_{11}&M_{12}&M_{22}&M_{23}&M_{24}\\
\text{degree}&11&12&22&23&24\\
\text{transitivity}&4&5&3&4&5
\end{array}
$$

In particular all five natural actions are [two-transitive](../../../../../two-transitive-group-action.md). Together these examples exhibit affine spaces, projective and Hermitian geometries, symplectic [quadratic forms](../../../../../quadratic-form.md), and exceptional finite [simple groups](../../../../../simple-group.md) as different sources of the same pair symmetry.

**The organizing distinction is affine versus almost simple; the action, its degree, and its [stabilizer subgroup](../../../../../stabilizer-subgroup.md) are essential data.** The explicitly verified affine, symmetric, alternating, projective, unitary, and symplectic actions already give many infinite families, while the exceptional families show why no single [matrix](../../../../../matrix.md) construction covers every example.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
