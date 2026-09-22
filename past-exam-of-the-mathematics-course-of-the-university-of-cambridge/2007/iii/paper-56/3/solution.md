<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use anti-Hermitian $\mathfrak{su}(2)$ matrices, with invariant positive inner product $\langle X,Y\rangle=-2\operatorname{tr}(XY)$. On an adjoint-valued field $\Xi$, define the [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) and [gauge curvature](../../../../../gauge-field-strength.md) by

$$
\boxed{D_i\Xi=\partial_i\Xi+[A_i,\Xi],\qquad F_{ij}=\partial_iA_j-\partial_jA_i+[A_i,A_j].}
$$

Equivalently, $F=dA+A\wedge A$ and $[D_i,D_j]\Xi=[F_{ij},\Xi]$. Put $B_i=\tfrac12\epsilon_{ijk}F_{jk}$, with $\epsilon_{123}=1$. The monopole [Bogomolny equations](../../../../../bogomolny-equations.md) are $B_i=D_i\Phi$.

For a smooth [SU(2)](../../../../../su-2-group.md) gauge transformation $g(x)$, use

$$
A_i^g=gA_ig^{-1}-(\partial_i g)g^{-1},\qquad\Phi^g=g\Phi g^{-1}.
$$

Differentiating a transformed adjoint field shows $D_i^g(g\Xi g^{-1})=g(D_i\Xi)g^{-1}$: the derivatives of $g$ cancel the inhomogeneous term in $A_i^g$. Applying the commutator of these derivatives gives $F_{ij}^g=gF_{ij}g^{-1}$, and therefore $B_i^g=gB_ig^{-1}$. Both sides of $B_i=D_i\Phi$ transform identically, establishing [gauge invariance](../../../../../gauge-invariance.md) of the solution condition. Individual matrix components are covariant, rather than invariant numbers.

The monopole boundary condition is a nonzero asymptotic Higgs norm,

$$
|\Phi(x)|\longrightarrow v>0\qquad(|x|\to\infty),
$$

together with finite three-dimensional Yang-Mills-Higgs energy. Standard monopole asymptotics have $D\Phi=O(r^{-2})$ and $F=O(r^{-2})$. The normalized [Higgs field](../../../../../higgs-field.md) at infinity defines a map $S^2_\infty\to SU(2)/U(1)\simeq S^2$, whose [topological degree](../../../../../topological-degree.md) is the magnetic charge. A nonzero charge gives a genuine non-Abelian [magnetic monopole](../../../../../magnetic-monopole.md); the nonzero Higgs boundary value alone also allows the zero-charge vacuum. Thus the relevant nontrivial solutions are [Bogomolny-Prasad-Sommerfield monopoles](../../../../../bogomolny-prasad-sommerfield-monopole.md) in the zero-Higgs-potential limit.

Now form the four-dimensional connection with $\tau$-independent components. Its [gauge curvature](../../../../../gauge-field-strength.md) has

$$
\mathcal F_{ij}=F_{ij},\qquad\mathcal F_{i\tau}=\partial_i\Phi-\partial_\tau A_i+[A_i,\Phi]=D_i\Phi=B_i.
$$

The self-duality sign requires an orientation. Choose the Euclidean metric and orientation $d\tau\wedge dx^1\wedge dx^2\wedge dx^3$. For cyclic $(i,j,k)$, the [Hodge star operator](../../../../../hodge-star-operator.md) satisfies

$$
*(dx^j\wedge dx^k)=d\tau\wedge dx^i,\qquad*(d\tau\wedge dx^i)=dx^j\wedge dx^k.
$$

Using $F_{jk}=\epsilon_{jki}B_i$ and $dx^i\wedge d\tau=-d\tau\wedge dx^i$, the curvature is

$$
\mathcal F=\sum_{\rm cyclic}B_i(dx^j\wedge dx^k-d\tau\wedge dx^i).
$$

Each term has negative star eigenvalue, so

$$
\boxed{*\mathcal F=-\mathcal F.}
$$

This proves the [Anti-self-dual Yang-Mills equations](../../../../../anti-self-dual-yang-mills-equations.md) in the stated convention. The [orientation of a monopole lift](../../../../../orientation-of-a-monopole-lift.md) matters: with $dx^1\wedge dx^2\wedge dx^3\wedge d\tau$ instead, the same connection is self-dual. With that opposite orientation, the anti-self-dual lift would use $-\Phi\,d\tau$.

To fix the action normalization, take the Euclidean [Yang-Mills action](../../../../../yang-mills-action.md)

$$
S_4=\frac1{4g_{\rm YM}^2}\int_{\mathbb R^4}\sum_{\mu,\nu}|\mathcal F_{\mu\nu}|^2\,d^4x
=-\frac1{2g_{\rm YM}^2}\int\sum_{\mu,\nu}\operatorname{tr}(\mathcal F_{\mu\nu}\mathcal F_{\mu\nu})\,d^4x.
$$

Both sums are over ordered index pairs. The component identity  
$\sum_{j,k}|F_{jk}|^2=2\sum_i|B_i|^2$ gives

$$
\sum_{\mu,\nu}|\mathcal F_{\mu\nu}|^2
=\sum_{j,k}|F_{jk}|^2+2\sum_i|D_i\Phi|^2
=2\sum_{j,k}|F_{jk}|^2.
$$

Hence the four-dimensional action density in terms of the three-dimensional curvature is

$$
\boxed{\mathcal L_4=\frac1{2g_{\rm YM}^2}\sum_{j,k}|F_{jk}|^2
=\frac1{g_{\rm YM}^2}\sum_i|B_i|^2
=-\frac1{g_{\rm YM}^2}\sum_{j,k}\operatorname{tr}(F_{jk}F_{jk}).}
$$

A different overall action normalization rescales all three equal expressions together.

A [Yang-Mills instanton](../../../../../yang-mills-instanton.md) is a smooth finite-Euclidean-action self-dual or anti-self-dual connection in pure [Yang-Mills theory](../../../../../yang-mills-theory.md), with the usual asymptotic pure-gauge behavior. Physically the term generally refers to a nontrivial field; its asymptotic gauge winding labels an [instanton number](../../../../../instanton-number.md). The [Bianchi identity](../../../../../bianchi-identity.md) $D\mathcal F=0$, together with $*\mathcal F=-\mathcal F$, implies $D*\mathcal F=0$, so the first-order equations already imply the second-order [Yang-Mills equations](../../../../../yang-mills-equations.md). Finite action is a separate requirement.

Here $\mathcal L_4$ is independent of $\tau$. If the monopole has nonzero curvature, the density is positive on an open set in $\mathbb R^3$, and integrating its infinite $\tau$-extent gives

$$
\boxed{S_4=\infty.}
$$

For a finite-energy monopole this can also be written as its positive action per unit length times $\int_{\mathbb R}d\tau$. Thus **a nontrivial monopole lift is not a Yang-Mills instanton on $\mathbb R^4$**. The flat solution $A_i=0$, $\Phi=\Phi_0$ constant is the zero-action exception: it is a vacuum, or a trivial charge-zero instanton if that terminology includes flat connections. It is not a counterexample to the nontrivial-monopole assertion.

More generally, [finite Yang-Mills action forbids nontrivial translation symmetry](../../../../../finite-yang-mills-action-forbids-nontrivial-translation-symmetry.md), even when the translation preserves a connection only up to gauge. Such a symmetry would preserve its positive gauge-invariant action density. A nonflat field has a ball on which this density is bounded below by some positive constant. Repeated translations by a nonzero symmetry vector produce infinitely many disjoint copies of a sufficiently small such ball, all with the same positive action contribution, contradicting finiteness. Continuous translation invariance is a special case. Therefore **a nonflat ASDYM instanton is localized in all four Euclidean directions and has no nonzero translational symmetry**. Translating an instanton still produces another instanton with a shifted center; these position parameters belong to the [instanton moduli space](../../../../../instanton-moduli-space.md), rather than being invariances of one localized solution.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
