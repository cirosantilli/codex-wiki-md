# Paper 42

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_42.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_42.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [SU(2) group](../../../topological-group.md#su-2-group) consists of complex $2\times2$ matrices $U$ with $U^\dagger U=I$ and $\det U=1$. The [SO(3) group](../../../linear-algebra.md#so-3-group) consists of real $3\times3$ matrices $R$ with $R^TR=I$ and $\det R=1$. Differentiate these equations along a path through the identity. This gives

$$
\mathfrak{su}(2)=\{X:X^\dagger=-X,\ \operatorname{tr}X=0\},\qquad
\mathfrak{so}(3)=\{L:L^T=-L\}.
$$

Conversely the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) of each displayed infinitesimal matrix satisfies the corresponding group equations, so these are exactly the [Lie algebras](../../../lie-algebra.md), with bracket the matrix [commutator](../../../lie-algebra.md#commutator).

Using the [Pauli matrices](../../../algebra.md#pauli-matrices), put $t_a=-i\sigma_a/2$. They form a real basis of the [SU(2) Lie algebra](../../../semisimple-lie-algebra.md#su-2-lie-algebra). The [Pauli matrix commutator identity](../../../algebra.md#pauli-matrix-commutator-identity) gives $[t_a,t_b]=\epsilon_{abc}t_c$. Define $J_a$ on $\mathbb R^3$ by $J_av=e_a\times v$. These are a basis of the [SO(3) Lie algebra](../../../semisimple-lie-algebra.md#so-3-lie-algebra); the vector triple-product identity gives $[J_a,J_b]=\epsilon_{abc}J_c$. Thus

$$
\boxed{\sum_a u_at_a\longmapsto\sum_a u_aJ_a}
$$

is a real linear bijection preserving the bracket. This is the [SU(2)-SO(3) Lie algebra isomorphism](../../../linear-operator-theory.md#cross-product-model-of-su-2). It is a Lie-algebra isomorphism, not a group isomorphism: the [Adjoint double cover from SU(2) to SO(3)](../../../lie-theory.md#adjoint-double-cover-from-su-2-to-so-3) has kernel $\{I,-I\}$.

The [SU(3) group](../../../topological-group.md#su-3-group) is defined similarly by $U^\dagger U=I$ and $\det U=1$ on complex $3\times3$ matrices. One [SU(2)](../../../topological-group.md#su-2-group) subgroup is $\{\operatorname{diag}(V,1):V\in SU(2)\}$. The real orthogonal matrices with determinant one form an [SO(3) group](../../../linear-algebra.md#so-3-group) subgroup, since real orthogonality is also complex unitarity.

Under the defining [group action](../../../group-theory.md#group-action), the [group orbit](../../../group-theory.md#orbit-of-a-group-action) of $e_1$ is exactly the unit sphere in $\mathbb C^3$:

$$
\boxed{SU(3)e_1=\{z:z^\dagger z=1\}=S^5.}
$$

Unitarity proves containment. Conversely, extend a unit vector $z$ to an orthonormal basis and use it as the first column of a unitary matrix. Multiplying the last column by the inverse of its determinant makes that determinant one without changing the first column. The [isotropy group](../../../group-theory.md#stabilizer-subgroup) of $e_1$ must also preserve its orthogonal complement, and therefore is

$$
\boxed{\{\operatorname{diag}(1,V):V\in SU(2)\}\cong SU(2).}
$$

This proves the [unit sphere orbit of the defining special unitary action](../../../topological-group.md#unit-sphere-orbit-of-the-defining-special-unitary-action), including $S^5\cong SU(3)/SU(2)$.

For the complex quadric, write $z=x+iy$. Its defining relation separates into

$$
|x|^2-|y|^2=1,\qquad x\cdot y=0.
$$

The Hermitian norm is then $z^\dagger z=1+2|y|^2$, which is not constant on this set. For example, $e_1$ and $\sqrt2e_1+ie_2$ both satisfy the complex bilinear relation but have Hermitian norms one and three. Since the [SU(3) group](../../../topological-group.md#su-3-group) preserves that norm, **the quadric cannot be a single SU(3) [group orbit](../../../group-theory.md#orbit-of-a-group-action)**. In fact it is not even invariant under the whole group: $\operatorname{diag}(e^{it},e^{-it},1)e_1$ fails the bilinear relation when $e^{2it}\ne1$.

The real [SO(3) group](../../../linear-algebra.md#so-3-group) does preserve the quadric, acting simultaneously on $x$ and $y$. Its [group orbits](../../../group-theory.md#orbit-of-a-group-action) are classified completely by $r=|y|\geq0$. For $r=0$, $y=0$ and $x$ is a real unit vector, giving the [group orbit](../../../group-theory.md#orbit-of-a-group-action) $S^2$ and [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) $SO(2)$. For $r>0$, the vectors $x/\sqrt{1+r^2}$ and $y/r$ are orthonormal. Adjoining their cross product gives an oriented orthonormal frame. There is a unique rotation taking the standard frame to this one; hence the action is transitive at fixed $r$ and the [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) is trivial. Thus the [real rotation orbits on a complex unit quadric](../../../group-theory.md#real-rotation-orbits-on-a-complex-unit-quadric) are

$$
\boxed{M_0\cong S^2,\qquad M_r\cong SO(3)\ (r>0),\qquad M/SO(3)\cong[0,\infty).}
$$

In particular the real subgroup does not act transitively on the whole quadric. The parametrization $x=\sqrt{1+|y|^2}\,n$ with $n\in S^2$ and $y\perp n$ also identifies the quadric, as a real manifold, with the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) of $S^2$.

## 2

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use anti-Hermitian gauge potentials and the convention $D_i=\partial_i+A_i$ for the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative). Commuting these operators defines the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength):

$$
\boxed{F_{xy}=\partial_xA_y-\partial_yA_x+[A_x,A_y].}
$$

It is antisymmetric in its two spacetime indices, so $F_{xx}=F_{yy}=0$ and $F_{yx}=-F_{xy}$. In two dimensions there is therefore only one independent component, although that component is itself Lie-algebra valued.

Put $B_x=(\partial_xg)g^{-1}$ and $B_y=(\partial_yg)g^{-1}$. Differentiating $g^{-1}$ gives $\partial_i g^{-1}=-g^{-1}(\partial_i g)g^{-1}$. Equality of mixed derivatives then gives the right [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation)

$$
\partial_xB_y-\partial_yB_x=B_xB_y-B_yB_x=[B_x,B_y].
$$

Consequently the [scaled right Maurer-Cartan gauge potential](../../../relativistic-quantum-field.md#scaled-right-maurer-cartan-gauge-potential) has curvature

$$
\boxed{F_{xy}=\alpha(1+\alpha)[B_x,B_y]
=\alpha(1+\alpha)\bigl((\partial_xg)g^{-1}(\partial_yg)g^{-1}-(\partial_yg)g^{-1}(\partial_xg)g^{-1}\bigr).}
$$

Thus **$\alpha=0$ and $\alpha=-1$ give zero curvature for every smooth $g$**. At zero the potential is zero. At minus one it is a [pure gauge potential](../../../relativistic-quantum-field.md#pure-gauge-potential): transforming the zero connection by $g$ gives $A=-dg\,g^{-1}$. If the gauge Lie algebra is abelian, the [commutator](../../../lie-algebra.md#commutator) vanishes for every $\alpha$. If it contains $X,Y$ with $[X,Y]\ne0$, choose $g(x,y)=e^{xX}e^{yY}$; at the origin $B_x=X$ and $B_y=Y$. Thus in that case the two displayed values are the only choices flat for every $g$. If the potential is instead defined using $D=\partial-A$ and field components $\partial_xA_y-\partial_yA_x-[A_x,A_y]$, the same calculation reads $\alpha(1-\alpha)[B_x,B_y]$ and the nonzero pure-gauge value is $+1$. The sign convention must be specified.

For the specified [SU(2)](../../../topological-group.md#su-2-group) exponential, let $r=\sqrt{x^2+y^2}$ and, away from the origin, $n=(x/r,y/r,0)$. The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives $(n\cdot\sigma)^2=I$, so summing the exponential series yields

$$
g=\cos(r/2)I-i\sin(r/2)(n\cdot\sigma).
$$

The continuous extension at the origin is $I$. For $r>0$, the second term is zero precisely when $\sin(r/2)=0$, and hence

$$
\boxed{g=I\text{ at }r=0,\qquad g=(-1)^kI\text{ on }r=2\pi k,\quad k=1,2,\ldots.}
$$

These are infinitely many distinct circles.

At the origin, differentiating the exponential at zero gives $B_x=t_1$ and $B_y=t_2$. Since $[t_1,t_2]=t_3=-i\sigma_3/2$, the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) there is

$$
\boxed{F_{xy}(0,0)=-\frac{i}{2}\alpha(1+\alpha)\sigma_3.}
$$

To evaluate it on the circles, use polar coordinates. On $r=2\pi k$ the angular derivative of $g$ vanishes, while $B_r=-i(n\cdot\sigma)/2$. Therefore $B_x=(x/r)B_r$ and $B_y=(y/r)B_r$ commute, and **$F_{xy}=0$ everywhere on every such circle, for every $\alpha$**.

One can also see these [circular curvature zeros for a planar SU2 exponential](../../../relativistic-quantum-field.md#circular-curvature-zeros-for-a-planar-su2-exponential) from a formula valid away from the origin. Write $n=(\cos\vartheta,\sin\vartheta,0)$, $m=(-\sin\vartheta,\cos\vartheta,0)$, and $t_n=-i(n\cdot\sigma)/2$, $t_m=-i(m\cdot\sigma)/2$. Direct differentiation gives

$$
B_r=t_n,\qquad B_\vartheta=\sin r\,t_m+(1-\cos r)t_3,
$$

and hence

$$
[B_x,B_y]=\frac1r[B_r,B_\vartheta]=\frac{\sin r}{r}t_3-\frac{1-\cos r}{r}t_m.
$$

Both coefficients vanish at the positive circle radii, and the expression tends to $t_3$ at the origin, agreeing with the direct calculation.

## 3

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [weight of a representation](../../../semisimple-lie-algebra.md#weight-of-a-representation) of $SU(3)$ is a joint eigenvalue of two commuting generators spanning a [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra). Equivalently it describes the character by which the diagonal maximal torus acts on a [weight vector](../../../semisimple-lie-algebra.md#weight-vector). Use the Hermitian generators

$$
I_3=\operatorname{diag}(1/2,-1/2,0),\qquad Y=\operatorname{diag}(1/3,1/3,-2/3).
$$

Their multiples by $i$ are in the [SU(3) Lie algebra](../../../lie-algebra.md#su-3-lie-algebra). A vector with weight $(a,b)$ acquires the phase $e^{i(a\theta+b\varphi)}$ under $\exp(i\theta I_3+i\varphi Y)$. The conventional generator $H_8$ is related by $Y=2H_8/\sqrt3$; using $H_8$ instead just rescales the vertical weight coordinate.

In the defining [group representation](../../../representation-theory.md#group-representation), the coordinate vectors $e_u,e_d,e_s$ are joint eigenvectors. The [weight diagram of the defining SU(3) representation](../../../semisimple-lie-algebra.md#weight-diagram-of-the-defining-su-3-representation) therefore has

$$
\boxed{\mu_u=(1/2,1/3),\qquad\mu_d=(-1/2,1/3),\qquad\mu_s=(0,-2/3).}
$$

Complex conjugation reverses all torus phases, so the weights of $\overline{\mathbf3}$ are **$-\mu_u,-\mu_d,-\mu_s$**, each with multiplicity one. The conjugation bar is essential: the tensor product here is $\mathbf3\otimes\overline{\mathbf3}$.

Weights add in a [tensor product of group representations](../../../representation-theory.md#tensor-product-of-group-representations). Thus the nine weights of this product are $\mu_i-\mu_j$. There are three zero weights from $i=j$, and the remaining six are

$$
\boxed{(1,0),\ (-1,0),\ (1/2,1),\ (-1/2,1),\ (-1/2,-1),\ (1/2,-1).}
$$

To turn this weight calculation into a direct-sum decomposition, identify the tensor product with $\operatorname{End}(\mathbb C^3)$ by $v\otimes\overline w\mapsto vw^\dagger$. The group acts by $M\mapsto UMU^{-1}$. This gives two invariant spaces,

$$
\operatorname{End}(\mathbb C^3)=\mathbb C I\oplus\mathfrak{sl}_3(\mathbb C).
$$

The scalar line has weight zero and is the trivial [group representation](../../../representation-theory.md#group-representation) $\mathbf1$. The traceless space has the six nonzero weights just computed, represented by the off-diagonal matrix units $E_{ij}$, and two zero weights, represented by traceless diagonal matrices. Its dimension is eight and it is the complex [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) $\mathbf8$. Therefore

$$
\boxed{\mathbf3\otimes\overline{\mathbf3}=\mathbf8\oplus\mathbf1.}
$$

This proves the [octet and singlet in a fundamental SU3 tensor product](../../../representation-theory.md#octet-and-singlet-in-a-fundamental-su3-tensor-product) with the correct central weight multiplicities.

The singlet is irreducible because it is one-dimensional. For the octet, an invariant complex subspace of $\mathfrak{sl}_3$ is stable under [commutators](../../../lie-algebra.md#commutator) with the complexified [Lie algebra](../../../lie-algebra.md). Commuting Cartan generators project it into weight spaces. If it contains any nonzero root vector $E_{ij}$, commutation with $E_{ji}$ produces $E_{ii}-E_{jj}$; further [commutators](../../../lie-algebra.md#commutator) produce the opposite root and all other matrix units, hence the whole traceless algebra. If it contains only a nonzero diagonal traceless matrix $D$, two diagonal entries differ, so $[E_{ij},D]=(D_{jj}-D_{ii})E_{ij}$ supplies a root vector and reduces to the preceding case. There is no nonzero proper invariant subspace. **The octet is irreducible**, not a sum of six one-dimensional weight spaces and two singlets: the nondiagonal generators connect those spaces.

In the [quark model](../../../physics.md#quark-model), take $u,d,s$ as the defining flavour triplet and their antiquarks as the conjugate triplet. A colour-singlet quark-antiquark state with relative orbital angular momentum $L=0$ and total spin $S=0$ has $J=0$ and parity $(-1)^{L+1}=-1$. Thus this flavour decomposition classifies a [pseudoscalar meson nonet](../../../physics.md#pseudoscalar-meson-nonet): a [meson octet](../../../standard-model.md#meson-octet) and a singlet. The use of approximate [flavor symmetry](../../../standard-model.md#flavor-symmetry) is important; the strange quark is heavier, so these states need not have equal masses.

In the $(I_3,Y)$ diagram, $Y$ is [flavor hypercharge](../../../standard-model.md#flavor-hypercharge), not electroweak hypercharge. Mesons have baryon number zero, so $Y$ equals their strangeness, and electric charge is $Q=I_3+Y/2$. The outer six weight states are

$$
\begin{array}{c|c|c}
\text{state}&\text{flavour content}&(I_3,Y)\\\hline
\pi^+&u\overline d&(1,0)\\
\pi^-&d\overline u&(-1,0)\\
K^+&u\overline s&(1/2,1)\\
K^0&d\overline s&(-1/2,1)\\
K^-&s\overline u&(-1/2,-1)\\
\overline K^0&s\overline d&(1/2,-1)
\end{array}
$$

The [pions](../../../standard-model.md#pion) form an isospin triplet, completed at the centre by $\pi^0=(u\overline u-d\overline d)/\sqrt2$. The four [kaons](../../../physics.md#kaon) occupy the two hypercharge-one and two hypercharge-minus-one weights. In particular electrically neutral kaons are not at the centre of the [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram).

<a id="3/image-pseudoscalar-meson-weights-in-flavour-isospin-and-hypercharge-showing-the-two-octet-states-and-separate-singlet-at-the-centre"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-42-meson-weights.png)

**[Figure 1](#3/image-pseudoscalar-meson-weights-in-flavour-isospin-and-hypercharge-showing-the-two-octet-states-and-separate-singlet-at-the-centre). Pseudoscalar meson weights in flavour isospin and hypercharge, showing the two octet states and separate singlet at the centre**.

An orthonormal basis of the three central flavour combinations is

$$
\pi^0=\frac{u\overline u-d\overline d}{\sqrt2},\qquad
\eta_8=\frac{u\overline u+d\overline d-2s\overline s}{\sqrt6},\qquad
\eta_1=\frac{u\overline u+d\overline d+s\overline s}{\sqrt3}.
$$

The [Eta octet state](../../../standard-model.md#eta-octet-state) is the second zero weight of the octet; the [eta singlet state](../../../physics.md#eta-singlet-state) is the separate invariant scalar. Both have isospin zero, whereas the neutral pion has isospin one. All have $I_3=Y=Q=0$, so the location of a weight alone does not determine either isospin or irreducible multiplet. Their neutral flavour-diagonal $L=S=0$ states have charge conjugation $C=(-1)^{L+S}=+1$ and hence $J^{PC}=0^{-+}$.

The physical [eta and eta prime mesons](../../../physics.md#eta-and-eta-prime-mesons) are mixtures of the octet and singlet combinations, conventionally described at this level by

$$
\eta=\cos\theta\,\eta_8-\sin\theta\,\eta_1,\qquad
\eta'=\sin\theta\,\eta_8+\cos\theta\,\eta_1.
$$

Flavour breaking and the singlet axial anomaly affect their masses and mixing. The neutral pion is much lighter, about $135\,\mathrm{MeV}$, and decays predominantly to two photons. The eta has mass about $548\,\mathrm{MeV}$ and important two-photon and three-pion decay modes; the eta prime has mass about $958\,\mathrm{MeV}$ and important decays to $\eta\pi\pi$. The singlet axial anomaly explains why the eta prime is not an additional light Goldstone boson merely because the flavour tensor product contains a singlet. **The centre contains two octet directions and one singlet direction; physical eta mixing combines the latter two, leaving the isospin-one neutral pion separate to a good approximation.**

## 4

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Start with the [classification of finite-dimensional representations of SU2](../../../representation-theory.md#classification-of-finite-dimensional-representations-of-su2). Its irreducible complex [group representations](../../../representation-theory.md#group-representation) are the spin-$j$ spaces

$$
V_j=\operatorname{Sym}^{2j}\mathbb C^2,\qquad j=0,\tfrac12,1,\ldots,\qquad\dim V_j=2j+1.
$$

The central element $-I$ acts on $V_j$ as $(-1)^{2j}$. These facts follow also by realizing $V_j$ as homogeneous polynomials of degree $2j$ in two variables: the raising and lowering operators connect all of their one-dimensional weight spaces, and the highest-weight classification supplies every irreducible.

Identify Euclidean four-space with the [quaternions](../../../algebra.md#quaternion). The [unit quaternions](../../../algebra.md#unit-quaternion), each a copy of $SU(2)$, act by

$$
(a,b):q\longmapsto aqb^{-1}.
$$

The norm is multiplicative, so this is an orthogonal action. It preserves orientation because the acting group is connected. If it fixes every $q$, setting $q=1$ first gives $a=b$, and then this [quaternion](../../../algebra.md#quaternion) must commute with every [quaternion](../../../algebra.md#quaternion); a real unit [quaternion](../../../algebra.md#quaternion) is $\pm1$. The kernel is therefore $\{(1,1),(-1,-1)\}$.

For completeness, the differential is injective: if imaginary [quaternions](../../../algebra.md#quaternion) $u,v$ satisfy $uq-qv=0$ for every $q$, then $u=v$ is central and imaginary, hence zero. Both [Lie algebras](../../../lie-algebra.md) have dimension six. Thus the image contains a neighbourhood of the identity and is an open subgroup of the connected [SO(4) group](../../../linear-algebra.md#so-4-group), so it is the whole group. This proves the [Spin(4) double cover](../../../semisimple-lie-algebra.md#spin-4-double-cover)

$$
\boxed{SO(4)\cong\bigl(SU(2)_L\times SU(2)_R\bigr)/\{(I,I),(-I,-I)\}.}
$$

The covering group is simply connected since each $SU(2)$ is a three-sphere.

The [irreducible representations](../../../representation-theory.md#irreducible-representation) of a product of compact groups are tensor products of irreducibles of its two factors. One way to see this is to decompose an irreducible space into isotypic components for the first factor; the second commutes with the first, so only one isotypic component can occur. The multiplicity space must then be irreducible for the second factor. Hence the covering-group irreducibles are $V_{j_L}\otimes V_{j_R}$. By [central parity on SU2 tensor products](../../../representation-theory.md#central-parity-on-su2-tensor-products), the kernel element acts as $(-1)^{2j_L+2j_R}$. The [group representation](../../../representation-theory.md#group-representation) descends to $SO(4)$ precisely when that sign is positive. The [representations of SO(4) from two SU2 spins](../../../linear-algebra.md#representations-of-so-4-from-two-su2-spins) are therefore

$$
\boxed{(j_L,j_R),\quad j_L+j_R\in\mathbb Z,\quad\dim=(2j_L+1)(2j_R+1).}
$$

Every finite-dimensional irreducible complex [group representation](../../../representation-theory.md#group-representation) of $SO(4)$ is obtained this way. Since the group is compact, these are also all its continuous irreducible unitary [group representations](../../../representation-theory.md#group-representation), up to equivalence.

The Lie-algebra version makes the two spin labels visible locally. Choose rotation generators $J_i$ and generators $K_i$ mixing the fourth direction with the first three, normalized so that

$$
[J_i,J_j]=\epsilon_{ijk}J_k,\qquad[J_i,K_j]=\epsilon_{ijk}K_k,\qquad[K_i,K_j]=\epsilon_{ijk}J_k.
$$

Then $A_i=(J_i+K_i)/2$ and $B_i=(J_i-K_i)/2$ obey two commuting copies of $\mathfrak{su}(2)$. The [quaternion](../../../algebra.md#quaternion) quotient determines which [Lie algebra representations](../../../lie-algebra.md#lie-algebra-representation) integrate to the actual group, rather than only to its cover.

For example, $(0,0)$ is the scalar, $(1/2,1/2)$ is the four-vector, and $(1,0)$ and $(0,1)$ are the three-dimensional self-dual and anti-self-dual two-form [group representations](../../../representation-theory.md#group-representation). The half-spin spaces $(1/2,0)$ and $(0,1/2)$ belong to the cover and do not descend to $SO(4)$. Restricting to rotations fixing the real [quaternion](../../../algebra.md#quaternion) axis gives the diagonal $SU(2)$, and the [Clebsch-Gordan decomposition for SU2](../../../representation-theory.md#clebsch-gordan-decomposition-for-su2) yields

$$
V_{j_L}\otimes V_{j_R}\big|_{\mathrm{diag}\,SU(2)}\cong\bigoplus_{j=|j_L-j_R|}^{j_L+j_R}V_j,
$$

with steps of one. For a descended [group representation](../../../representation-theory.md#group-representation) these diagonal spins are integers, as required for the spatial $SO(3)$ subgroup.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The [Proper orthochronous Lorentz group](../../../special-relativity.md#proper-orthochronous-lorentz-group) is the connected Lorentz group in the question. Its double cover is $SL(2,\mathbb C)$, viewed as a real [Lie group](../../../lie-theory.md#lie-group). Identify a spacetime vector with the Hermitian matrix

$$
X=x^0I+x^a\sigma_a=\begin{pmatrix}x^0+x^3&x^1-ix^2\\x^1+ix^2&x^0-x^3\end{pmatrix},\qquad\det X=(x^0)^2-|\mathbf x|^2.
$$

The action $X\mapsto SXS^\dagger$ for $S\in SL(2,\mathbb C)$ preserves this determinant and hence the Minkowski metric. The group is connected, so its image is proper and orthochronous. Its kernel consists of $\pm I$: a matrix in the kernel first preserves $I$, hence is unitary, and then commutes with every Hermitian matrix, so is scalar; determinant one forces the two signs. Matrices in $SU(2)$ generate spatial rotations, and positive Hermitian determinant-one matrices generate boosts. Rotations and boosts generate the connected Lorentz group, so the action is onto. Polar decomposition also gives $SL(2,\mathbb C)\cong SU(2)\times\mathbb R^3$ as a manifold, proving that it is simply connected. This establishes the [Lorentz spinor double cover](../../../special-relativity.md#lorentz-spinor-double-cover).

In an anti-Hermitian rotation-generator convention, the [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra) brackets are

$$
[J_i,J_j]=\epsilon_{ijk}J_k,\qquad[J_i,K_j]=\epsilon_{ijk}K_k,\qquad[K_i,K_j]=-\epsilon_{ijk}J_k.
$$

The negative sign in the last bracket distinguishes boosts from Euclidean four-dimensional rotations. After complexification, set

$$
A_i=\frac{J_i+iK_i}{2},\qquad B_i=\frac{J_i-iK_i}{2}.
$$

A direct bracket calculation gives $[A_i,A_j]=\epsilon_{ijk}A_k$, $[B_i,B_j]=\epsilon_{ijk}B_k$ and $[A_i,B_j]=0$. Thus the [chiral decomposition of the complex Lorentz algebra](../../../semisimple-lie-algebra.md#chiral-decomposition-of-the-complex-lorentz-algebra) is

$$
\mathfrak{so}(1,3)\otimes_{\mathbb R}\mathbb C\cong\mathfrak{sl}_2(\mathbb C)\oplus\mathfrak{sl}_2(\mathbb C).
$$

Complexification matters: the real Lorentz algebra is not the compact real algebra $\mathfrak{su}(2)\oplus\mathfrak{su}(2)$.

Each spin-$j$ [homogeneous polynomial representation of SU2](../../../representation-theory.md#homogeneous-polynomial-representation-of-su2) extends from $SU(2)$ to $SL(2,\mathbb C)$ as $D_j(S)=\operatorname{Sym}^{2j}S$. Its complex-conjugate extension uses $\overline S$. The finite-dimensional irreducible complex [group representations](../../../representation-theory.md#group-representation) of the covering group are therefore

$$
D^{(j_L,j_R)}(S)=D_{j_L}(S)\otimes D_{j_R}(\overline S),\qquad j_L,j_R\in\{0,\tfrac12,1,\ldots\}.
$$

The two separate complexified Lie-algebra factors act irreducibly on the two spin spaces, so their tensor product is irreducible. Conversely an invariant complex subspace for the real group is invariant under its complexified [Lie algebra](../../../lie-algebra.md); the highest-weight classification for the two $\mathfrak{sl}_2$ factors gives exactly these tensor products. This constructs all [finite-dimensional complex Lorentz representations](../../../semisimple-lie-algebra.md#finite-dimensional-complex-lorentz-representations).

Again $-I\in SL(2,\mathbb C)$ acts by $(-1)^{2j_L+2j_R}$. Therefore the [irreducible representations](../../../representation-theory.md#irreducible-representation) of the connected Lorentz group itself, in this finite-dimensional complex category, are

$$
\boxed{(j_L,j_R),\quad j_L+j_R\in\mathbb Z,\quad\dim=(2j_L+1)(2j_R+1).}
$$

If the sum is a half-integer, the [group representation](../../../representation-theory.md#group-representation) is a [group representation](../../../representation-theory.md#group-representation) of the spin cover, or a projective [group representation](../../../representation-theory.md#group-representation) of the Lorentz group, and is not an ordinary single-valued [group representation](../../../representation-theory.md#group-representation) of the group named in the question.

The scalar $(0,0)$ and four-vector $(1/2,1/2)$ descend. The left and right [Weyl spinors](../../../relativistic-quantum-field.md#weyl-spinor), $(1/2,0)$ and $(0,1/2)$, do not. Their direct sum is a [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor), reducible under the connected group; parity exchanges its two chiral summands. The [group representations](../../../representation-theory.md#group-representation) $(1,0)$ and $(0,1)$ describe the two complex chiral parts of an antisymmetric tensor. On the rotation subgroup, self-duality of $SU(2)$ irreducibles identifies the conjugate spin space with the usual spin space, so the [Clebsch-Gordan decomposition for SU2](../../../representation-theory.md#clebsch-gordan-decomposition-for-su2) gives the same spin range $|j_L-j_R|,\ldots,j_L+j_R$ as in part (i).

These are [group representations](../../../representation-theory.md#group-representation) used for fields, and they need not be unitary for a positive-definite inner product. Indeed no nontrivial finite-dimensional [group representation](../../../representation-theory.md#group-representation) of this group is unitary: if it were, its differential would embed the simple real Lorentz algebra into an algebra of skew-Hermitian matrices. The trace form $-\operatorname{tr}(XY)$ would give an invariant positive-definite form $b$ on that algebra. Invariance and the boost brackets would then force $-b(J_3,J_3)=b([K_1,K_2],J_3)=b(K_1,[K_2,J_3])=b(K_1,K_1)$, impossible for positive-definite $b$. Equivalently nontrivial boosts in these polynomial [group representations](../../../representation-theory.md#group-representation) have real exponential rather than phase eigenvalues.

The qualification about dimension is necessary because a noncompact group also has infinite-dimensional unitary [group representations](../../../representation-theory.md#group-representation). They too can be built using $SU(2)$ spin spaces, but not by a single finite pair. For example, the [rotation content of induced Lorentz representations](../../../representation-theory.md#rotation-content-of-induced-lorentz-representations) is obtained from normalized [induced representations](../../../representation-theory.md#induced-representation) of the upper triangular subgroup of $SL(2,\mathbb C)$, with $n\in\mathbb Z$, $\rho\in\mathbb R$ and unitary characters $(a/|a|)^n|a|^{2i\rho}$ on its diagonal $(a,a^{-1})$, trivial on its unipotent part. In the compact picture this uses functions on $SU(2)$ satisfying

$$
f\bigl(k\operatorname{diag}(e^{i\vartheta},e^{-i\vartheta})\bigr)=e^{-in\vartheta}f(k).
$$

Expanding functions into $SU(2)$ matrix coefficients selects a single right-torus weight from each spin space, giving the rotation content

$$
\bigoplus_{j=|n|/2,\ |n|/2+1,\ldots}V_j.
$$

Normalized induction supplies the boost action, coupling these infinitely many rotation spaces. The central sign is $(-1)^n$, so the even-$n$ family descends to the connected Lorentz group and has integer rotation spins. This explains both the finite-dimensional field construction and why a classification of unitary [group representations](../../../representation-theory.md#group-representation) cannot simply be identified with the finite two-spin labels.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
