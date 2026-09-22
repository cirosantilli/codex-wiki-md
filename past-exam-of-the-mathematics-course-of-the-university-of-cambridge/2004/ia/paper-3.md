# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2004/PaperIA_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2004/PaperIA_3.pdf)

**Table of contents**

- [1D](#1d)
  - [Solution](#1d/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3C](#3c)
  - [i](#3c/i)
    - [Solution](#3c/i/solution)
  - [ii](#3c/ii)
    - [Solution](#3c/ii/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
  - [i](#5d/i)
    - [Solution](#5d/i/solution)
  - [ii](#5d/ii)
    - [Solution](#5d/ii/solution)
  - [iii](#5d/iii)
    - [Solution](#5d/iii/solution)
  - [iv](#5d/iv)
    - [Solution](#5d/iv/solution)
- [6D](#6d)
  - [Solution](#6d/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
  - [i](#9c/i)
    - [Solution](#9c/i/solution)
  - [ii](#9c/ii)
    - [Solution](#9c/ii/solution)
  - [iii](#9c/iii)
    - [Solution](#9c/iii/solution)
  - [iv](#9c/iv)
    - [Solution](#9c/iv/solution)
  - [v](#9c/v)
    - [Solution](#9c/v/solution)
- [10C](#10c)
  - [Solution](#10c/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12C](#12c)
  - [Solution](#12c/solution)

## 1D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1d/solution">Solution</h3>

↑ **Parent:** [1D](#1d)

For a [subgroup](../../../group.md#subgroup) $H$ of a finite [group](../../../group.md) $G$, [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) states $|G|=[G:H]|H|$. Thus a subgroup's order, and in particular the [order of a group element](../../../group-theory.md#order-of-a-group-element), divides $|G|$.

For $|G|=10$, if every element had order one or two, the [order of a finite group of exponent two](../../../group.md#order-of-a-finite-group-of-exponent-two) would make $|G|$ a power of two, a contradiction. Hence an element has order five or ten. In the latter case **$G$ is the cyclic group $C_{10}$**. Otherwise choose $a$ of order five. Its [cyclic subgroup](../../../group.md#cyclic-subgroup) $H=\langle a\rangle$ has index two and is therefore a [normal subgroup](../../../group-theory.md#normal-subgroup).

In the noncyclic case an element $b$ outside $H$ has order two: its order divides ten, it cannot have order ten, and an element of order five has trivial image in the order-two [quotient group](../../../group-theory.md#quotient-group) $G/H$. Every element of $G$ is then $a^j$ or $a^jb$. [Conjugation](../../../group-theory.md#conjugation) by $b$ restricts to an [automorphism](../../../algebra.md#automorphism) of $H$, say $bab^{-1}=a^r$. Since $b^2=1$, $r^2\equiv1\pmod5$, so $r=1$ or $-1$ modulo five.

For $r=1$, the generators commute and $ab$ has order ten, yielding the cyclic case. For $r=-1$, these are the relations of the [dihedral group](../../../finite-group-theory.md#dihedral-group) of the pentagon. The [classification of groups of order ten](../../../finite-group-theory.md#classification-of-groups-of-order-ten) is therefore **exactly $C_{10}$ and $D_{10}$**, where the subscript on $D_{10}$ denotes its order. They are not [isomorphic](../../../algebra.md#isomorphism) because one is [Abelian](../../../group.md#abelian-group) and the other is not.

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

The [Möbius group](../../../group-theory.md#mobius-group) consists of maps $z\mapsto(az+b)/(cz+d)$ with $ad-bc\ne0$, acting on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere) $\widehat{\mathbb C}=\mathbb C\cup\{\infty\}$. Proportional matrices represent the same map. Thus it is $\mathrm{PGL}_2(\mathbb C)$, equivalently $\mathrm{PSL}_2(\mathbb C)$ after normalizing the determinant. A zero denominator gives the image $\infty$, while $\infty$ maps to $a/c$ when $c\ne0$ and stays at infinity when $c=0$.

Fixing both zero and infinity forces $b=c=0$, leaving $z\mapsto\lambda z$ with $\lambda\ne0$. Composition multiplies the parameters, giving a bijective [group homomorphism](../../../group-theory.md#group-homomorphism) from the [multiplicative group of nonzero complex numbers](../../../group.md#complex-multiplicative-group) to this [pointwise stabilizer](../../../group-theory.md#pointwise-stabilizer).

For the other pair, take $T(z)=z/(1-z)$, which sends zero to zero and one to infinity. Conjugate the scaling subgroup by this [Möbius transformation](../../../group-theory.md#mobius-transformation):

$$
\boxed{T^{-1}(\lambda T(z))=\frac{\lambda z}{1+(\lambda-1)z},\qquad \lambda\in\mathbb C^*.}
$$

Every map fixing zero and one arises this way. Composition again multiplies $\lambda$, proving **both subgroups are isomorphic to $\mathbb C^*$**. This is the [Möbius pointwise stabilizer of two points](../../../group-theory.md#mobius-pointwise-stabilizer-of-two-points); conjugation changes the selected fixed points without changing its group structure.

## 3C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3c/i">i</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/i/solution">Solution</h4>

↑ **Parent:** [I](#3c/i)

Use the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) and sum over repeated indices. The [contraction of two Levi-Civita symbols](../../../calculus.md#contraction-of-two-levi-civita-symbols) and the [product rule](../../../calculus.md#product-rule) give

$$
\begin{aligned}
[\nabla\times(F\times G)]_i
&=\epsilon_{ijk}\partial_j(\epsilon_{k\ell m}F_\ell G_m)\\
&=\partial_j(F_iG_j-F_jG_i)\\
&=F_i\partial_jG_j-G_i\partial_jF_j+G_j\partial_jF_i-F_j\partial_jG_i.
\end{aligned}
$$

Reading the four terms as [divergence](../../../calculus.md#divergence) and directional derivatives proves the [curl of a cross product](../../../calculus.md#curl-of-a-cross-product) identity

$$
\boxed{\nabla\times(F\times G)=F(\nabla\cdot G)-G(\nabla\cdot F)+(G\cdot\nabla)F-(F\cdot\nabla)G.}
$$

<h3 id="3c/ii">ii</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3c/ii)

The [contraction of two Levi-Civita symbols](../../../calculus.md#contraction-of-two-levi-civita-symbols) gives $[F\times(\nabla\times G)]_i=F_j\partial_iG_j-F_j\partial_jG_i$. Similarly $[G\times(\nabla\times F)]_i=G_j\partial_iF_j-G_j\partial_jF_i$. Add the two directional-derivative terms to cancel the last terms, leaving

$$
F_j\partial_iG_j+G_j\partial_iF_j=\partial_i(F_jG_j).
$$

The [product rule](../../../calculus.md#product-rule) has therefore proved the [gradient of a dot product](../../../calculus.md#gradient-of-a-dot-product) identity

$$
\boxed{\nabla(F\cdot G)=(F\cdot\nabla)G+(G\cdot\nabla)F+F\times(\nabla\times G)+G\times(\nabla\times F).}
$$

## 4C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

For a regular [space curve](../../../topology.md#space-curve) parametrized by [arc length](../../../riemannian-geometry.md#arc-length) $s$, its [curvature](../../../differential-geometry.md#curvature) is $\kappa=\|dT/ds\|$, where $T=dx/ds$ is the unit tangent. Differentiating the given parametrization gives

$$
x'(t)=\frac{e^t}{2}(\cos t-\sin t,\ \sin t+\cos t,\ \sqrt2),\qquad \|x'(t)\|=e^t.
$$

The curve approaches the origin as $t\to-\infty$; the origin is a limiting endpoint. Its [arc length](../../../riemannian-geometry.md#arc-length) measured from that endpoint is $s=\int_{-\infty}^t e^u\,du=e^t$, so

$$
\boxed{x(s)=\left(\frac s2\cos\log s,\ \frac s2\sin\log s,\ \frac s{\sqrt2}\right),\qquad s>0.}
$$

This is a [logarithmic conical helix](../../../topology.md#logarithmic-conical-helix). Its unit tangent and derivative are

$$
T(s)=\frac12(\cos\log s-\sin\log s,\ \sin\log s+\cos\log s,\ \sqrt2),\qquad T'(s)=\frac1{2s}(-\sin\log s-\cos\log s,\ \cos\log s-\sin\log s,\ 0).
$$

Consequently,

$$
\boxed{\kappa(s)=\frac1{\sqrt2\,s}.}
$$

The infinitely many turns near the limiting origin have finite total [arc length](../../../riemannian-geometry.md#arc-length), while the [curvature](../../../differential-geometry.md#curvature) diverges there.

## 5D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

Use $D_{12}$ for the [dihedral group](../../../finite-group-theory.md#dihedral-group) of order twelve and write each element uniquely as $g^j$ or $g^jh$, $0\leq j<6$. The [classification of subgroups of a dihedral group](../../../finite-group-theory.md#classification-of-subgroups-of-a-dihedral-group) organizes the complete list: rotational subgroups are cyclic, and a subgroup containing a reflection is generated by its rotational part and one reflection. The individual lists and quotients follow below.

<h3 id="5d/i">i</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/i/solution">Solution</h4>

↑ **Parent:** [I](#5d/i)

The [involutions in an even dihedral group](../../../finite-group-theory.md#involutions-in-an-even-dihedral-group) are the half-turn $g^3$ and the six reflections $g^jh$. Thus the seven order-two [subgroups](../../../group.md#subgroup) are

$$
\boxed{\langle g^3\rangle,\qquad\langle g^jh\rangle\quad(j=0,1,2,3,4,5).}
$$

The half-turn is central, so **only $\langle g^3\rangle$ is normal**. Indeed $g(g^jh)g^{-1}=g^{j+2}h$, a different reflection; an order-two subgroup has only one nonidentity element, so each reflection subgroup fails the [normal subgroup](../../../group-theory.md#normal-subgroup) condition.

<h3 id="5d/ii">ii</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5d/ii)

The remaining proper [subgroups](../../../group.md#subgroup) are

$$
\boxed{\{1\},\quad\langle g^2\rangle,\quad\langle g\rangle,\quad\langle g^3,g^jh\rangle\ (j=0,1,2),\quad\langle g^2,g^jh\rangle\ (j=0,1).}
$$

Their orders are respectively one, three, six, four and six. The order-four groups are [Klein four-groups](../../../finite-group-theory.md#klein-four-group); the last two are [dihedral groups](../../../finite-group-theory.md#dihedral-group) of order six, isomorphic to $S_3$.

For completeness, if $H$ contains a reflection, write $H\cap\langle g\rangle=\langle g^d\rangle$ with $d\mid6$. Any other reflection differs from a chosen $g^jh$ by an element of this rotational subgroup, so $H=\langle g^d,g^jh\rangle$ with $j$ specified modulo $d$. The choices $d=1,2,3,6$ give respectively the whole group, the two order-six groups, the three order-four groups and the six reflection groups already listed. This proves there are no omitted subgroups.

Thus **there are eight remaining proper subgroups**. The printed count nine includes one too many; nine would be correct if the whole group were included with these remaining subgroups. Altogether $G$ has sixteen subgroups, fifteen proper.

<h3 id="5d/iii">iii</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5d/iii)

The proper [normal subgroups](../../../group-theory.md#normal-subgroup) and their [quotient groups](../../../group-theory.md#quotient-group) are as follows. Here the trivial subgroup is included as a proper subgroup.

- $N=\{1\}$ gives $G/N\cong D_{12}$.
- $N=\langle g^3\rangle$ gives $G/N\cong S_3$: the rotation has order three and the reflection inverts it.
- $N=\langle g^2\rangle$ gives $G/N\cong C_2\times C_2$: the two generators now have order two and commute.
- $N=\langle g\rangle$ gives $G/N\cong C_2$.
- $N=\langle g^2,h\rangle$ or $\langle g^2,gh\rangle$ gives $G/N\cong C_2$.

The rotational subgroups are preserved by reflection conjugation, and the last three order-six subgroups are normal by index two. The three order-four groups are not normal, since conjugation by $g$ changes the reflection exponent by two, which is nonzero modulo three. Part [solution](#5d/i/solution) excluded the reflection subgroups. These observations, together with the complete subgroup list, prove the normal-subgroup list is exhaustive.

<h3 id="5d/iv">iv</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5d/iv)

The rotation $g$ has order six. The possible [cycle types](../../../finite-group-theory.md#cycle-type) in the [alternating group](../../../finite-group-theory.md#alternating-group) $A_4$ are the identity, a three-cycle, and a product of two disjoint transpositions; their orders are one, three and two. Since a [group isomorphism](../../../algebra.md#group-isomorphism) preserves the [order of a group element](../../../group-theory.md#order-of-a-group-element), **$D_{12}$ is not isomorphic to $A_4$**.

## 6D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6d/solution">Solution</h3>

↑ **Parent:** [6D](#6d)

A real three-by-three [matrix](../../../vector-space.md#matrix) represents a proper [rotation](../../../riemannian-geometry.md#rotation-mathematics) in the standard orthonormal basis precisely when $A^TA=I$ and $\det A=1$, that is, when $A\in\mathrm{SO}(3)$. For the supplied integer numerator $B=3A$, direct multiplication gives $B^TB=9I$ and $\det B=27$, verifying both conditions.

The rotation axis is the [eigenspace](../../../linear-operator-theory.md#eigenspace) for [eigenvalue](../../../linear-operator-theory.md#eigenvalue) one. Solving $(A-I)n=0$ gives $n_3=0$ and $n_2=2n_1$, so

$$
\boxed{n=\frac1{\sqrt5}(1,2,0)^T}
$$

is a unit axis vector; its negative describes the same axis. On its perpendicular plane the [rotation matrix](../../../linear-algebra.md#rotation-matrix) has eigenvalues $e^{i\theta}$ and $e^{-i\theta}$. The [rotation trace formula](../../../linear-algebra.md#trace-of-a-three-dimensional-rotation) therefore gives $\operatorname{tr}A=1+2\cos\theta$. Since the trace is $-1/3$,

$$
\boxed{\cos\theta=-\frac23.}
$$

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

Let $Az=\lambda z$ with $z\ne0$, allowing complex [eigenvectors](../../../linear-operator-theory.md#eigenvector). A real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) is [Hermitian](../../../hilbert-space.md#hermitian-operator), so $z^*Az$ is real and $\lambda=z^*Az/(z^*z)$ is real. For eigenvectors $u,v$ of distinct real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda,\mu$, self-adjointness gives $\lambda u^*v=u^*Av=\mu u^*v$, hence $u^*v=0$. Thus the distinct eigenspaces are [orthogonal](../../../linear-algebra.md#orthogonal-vectors).

Here $A=3I-J$, where $J$ is the all-ones matrix. Since $J(1,1,1)^T=3(1,1,1)^T$ and $J$ vanishes on the plane of coordinate sum zero,

$$
\boxed{\lambda=0:\ E_0=\operatorname{span}\{(1,1,1)^T\};\qquad\lambda=3:\ E_3=\operatorname{span}\{(1,-1,0)^T,(1,1,-2)^T\}.}
$$

Every nonzero vector in the indicated eigenspace is an eigenvector. The repeated eigenvalue three has a two-dimensional eigenspace.

A [complex symmetric nilpotent matrix](../../../linear-algebra.md#complex-symmetric-nilpotent-matrix) provides the requested counterexample:

$$
\boxed{N=\begin{pmatrix}1&i\\i&-1\end{pmatrix},\qquad N\ne0,\quad N^T=N,\quad N^2=0.}
$$

Its characteristic polynomial is $\lambda^2$, so its only eigenvalue is zero. **It is not diagonalizable**: a diagonalizable matrix with only zero eigenvalues would itself be zero. Complex symmetry $N^T=N$ is weaker than the Hermitian condition $N^*=N$.

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

Expanding the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) along the first column gives

$$
\begin{aligned}
\chi_A(\lambda)&=(\lambda-3)\left[(\lambda-4+s)(\lambda-4s+1)+4(s-1)^2\right]\\
&=\boxed{(\lambda-3)^2(\lambda-3s)}.
\end{aligned}
$$

For $s\ne1$, solving the two nullspace equations gives

$$
\boxed{E_3=\operatorname{span}\{(1,0,0)^T,(0,2,1)^T\},\qquad E_{3s}=\operatorname{span}\{(1,s-1,2s-2)^T\}.}
$$

These are all the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and [eigenvectors](../../../linear-operator-theory.md#eigenvector), with nonzero vectors understood. The three displayed spanning vectors form an [eigenbasis](../../../linear-operator-theory.md#eigenbasis), so $A$ is [diagonalizable](../../../linear-operator-theory.md#diagonalizable-matrix).

At $s=1$, the sole eigenvalue is three, with algebraic multiplicity three but the same two-dimensional $E_3$. Thus **$A$ is diagonalizable exactly when $s\ne1$**. Indeed, at the exceptional parameter, $A=3I+N$ with $N\ne0$ and $N^2=0$, so its [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) has one block of size two and one of size one. This illustrates how an [eigenvalue collision](../../../linear-operator-theory.md#eigenvalue-collision) can destroy diagonalizability without changing the two-dimensional eigenspace.

## 9C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

Set $r=\sqrt{x^2+y^2}$. The bound $|xy|\leq r^2/2$ and $|x^2-y^2|\leq r^2$ give $|f(x,y)|\leq r^2/2$. Hence $f\to0$ at the origin, proving [continuity](../../../calculus.md#continuous-function), and $|f(x,y)|/r\to0$, proving [Fréchet differentiability](../../../calculus.md#frechet-differentiability) there with **derivative equal to the zero linear map**.

Along the coordinate axes, direct difference quotients give

$$
\boxed{f_x(0,y)=-y,\qquad f_y(x,0)=x.}
$$

These formulas include the origin. Therefore the two [mixed partial derivatives](../../../calculus.md#mixed-partial-derivative) differ:

$$
\boxed{\partial_y(\partial_x f)(0,0)=-1,\qquad\partial_x(\partial_y f)(0,0)=1.}
$$

The explicit operator order removes any ambiguity about the notation for mixed derivatives. Also $f_{xx}(0,0)=f_{yy}(0,0)=0$, since the first derivatives restricted to their own axes vanish identically.

All four second-order [partial derivatives](../../../calculus.md#partial-derivative) are discontinuous at the origin. Away from it,

$$
f_{xx}(x,y)=\frac{4xy^3(-x^2+3y^2)}{(x^2+y^2)^3},\qquad f_{yy}(x,y)=-\frac{4yx^3(-y^2+3x^2)}{(x^2+y^2)^3}.
$$

Along $x=y\ne0$ these are one and minus one, rather than their zero values at the origin. Meanwhile $\partial_y\partial_xf(x,0)=1$ for $x\ne0$, whereas its value at the origin is minus one; and $\partial_x\partial_yf(0,y)=-1$ for $y\ne0$, whereas its origin value is one. This gives a concrete [unequal mixed partial derivatives](../../../calculus.md#unequal-mixed-partial-derivatives) example despite differentiability of the original function.

<h3 id="9c/i">i</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/i/solution">Solution</h4>

↑ **Parent:** [I](#9c/i)

**True.** [Differentiability implies continuity](../../../analysis.md#differentiability-implies-continuity).

<h3 id="9c/ii">ii</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9c/ii)

**False.** [Partial derivatives do not imply continuity](../../../calculus.md#partial-derivatives-do-not-imply-continuity); derivatives along coordinate axes need not control nearby non-axis approaches.

<h3 id="9c/iii">iii</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#9c/iii)

**False.** [Directional derivatives do not imply differentiability](../../../calculus.md#directional-derivatives-do-not-imply-differentiability); the resulting dependence on direction need not be a linear derivative.

<h3 id="9c/iv">iv</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#9c/iv)

**False.** [Differentiability does not imply continuous derivatives](../../../analysis.md#differentiability-does-not-imply-continuous-derivatives).

<h3 id="9c/v">v</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/v/solution">Solution</h4>

↑ **Parent:** [V](#9c/v)

**False.** [Unequal mixed partial derivatives](../../../calculus.md#unequal-mixed-partial-derivatives) can exist when the continuity hypotheses of [Clairaut's theorem](../../../calculus.md#symmetry-of-second-derivatives) fail.

## 10C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10c/solution">Solution</h3>

↑ **Parent:** [10C](#10c)

An [exact differential](../../../differential-form.md#exact-differential) is a one-form equal to $d\Phi$ for a single-valued scalar function $\Phi$ on the domain. In Euclidean coordinates this means its vector coefficients form $\nabla\Phi$. Integrating the first component of $F$ with respect to $x$, then matching the other components, gives

$$
\boxed{\Phi(x,y,z)=z^3(e^x-e^y)+x^3(e^y-e^z)+C.}
$$

Differentiating checks all three components. Since the domain $\mathbb R^3$ is connected, two such potentials differ only by a constant, so this is the most general potential.

At both specified endpoints the nonconstant terms vanish. The [fundamental theorem for line integrals](../../../calculus.md#fundamental-theorem-for-line-integrals) gives **zero for the line integral along every path joining the two points**.

For the planar field, choose a continuous lift $\theta(t)$ of the polar angle along a curve avoiding the origin. Differentiating the angle gives

$$
G\cdot dx=\frac{-y\,dx+x\,dy}{x^2+y^2}=d\theta.
$$

On the closed curve the angle increases by $2\pi$ times its [winding number](../../../complex-analysis.md#winding-number). Thus

$$
\boxed{\oint_CG\cdot dx=2\pi.}
$$

The angle differential is locally exact but not globally exact on the [punctured plane](../../../complex-analysis.md#punctured-complex-plane): the angle lift need not return to its initial value. This is the [nonexact angular one-form](../../../differential-form.md#nonexact-angular-one-form), whose nonzero closed-path integral obstructs a global potential.

## 11C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

Choose zero [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass) at infinity. Apply [superposition](../../../vector-space.md#superposition-principle) to a uniform sphere of positive density and the two voids represented by spheres of negative density. The [shell theorem](../../../physics.md#spherical-shell-theorem) makes every component act as a point mass outside the large sphere. With $c_2=(1/2,0,0)$ and $c_3=(-1/4,0,0)$,

$$
\boxed{\Phi(x)=-\frac{4\pi G\rho}{3}\left[\frac1{|x|}-\frac{1/8}{|x-c_2|}-\frac{1/64}{|x-c_3|}\right],\qquad |x|>1.}
$$

The volume factors are the cubes of the three radii.

Inside the smaller void, the large sphere and the removed small sphere have interior fields $-Cx$ and $+C(x-c_3)$, where $C=4\pi G\rho/3$. They combine into the [uniform gravitational field in an off-center spherical cavity](../../../classical-mechanics.md#uniform-gravitational-field-in-an-off-center-spherical-cavity), $-Cc_3=C(1/4,0,0)$. The point is outside the other void's sphere, whose removed mass contributes a repulsive field. Thus

$$
\mathbf g(x)=C\left[\frac14e_1+\frac18\frac{x-c_2}{|x-c_2|^3}\right].
$$

An equilibrium must lie on the line through the two centers. Write $x=qe_1$ with $-1/2<q<0$. Its equation is $1/4-1/[8(1/2-q)^2]=0$, giving

$$
\boxed{x_*=(1/2-1/\sqrt2,0,0).}
$$

This point is inside the smaller void, but it is not stable. Let $d=|x_*-c_2|=1/\sqrt2$. The field's [Jacobian matrix](../../../calculus.md#jacobian-matrix) has eigenvalues

$$
-\frac{C}{4d^3},\qquad\frac{C}{8d^3},\qquad\frac{C}{8d^3}.
$$

The axial displacement is restoring, while transverse displacements accelerate away from equilibrium. Therefore **there is no point in that void where a test particle remains stably at rest**. The [cavity equilibrium destabilized by a second void](../../../classical-mechanics.md#cavity-equilibrium-destabilized-by-a-second-void) is a saddle; existence of a zero force is insufficient for stability.

<a id="11c/image-the-two-spherical-voids-and-the-unstable-equilibrium-inside-the-smaller-void"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-3-cavity-equilibrium.png)

**[Figure 1](#11c/image-the-two-spherical-voids-and-the-unstable-equilibrium-inside-the-smaller-void). The two spherical voids and the unstable equilibrium inside the smaller void**.

## 12C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12c/solution">Solution</h3>

↑ **Parent:** [12C](#12c)

For a continuously differentiable [vector field](../../../calculus.md#vector-field) on a volume and its boundary, the [divergence theorem](../../../calculus.md#divergence-theorem) equates $\int_V\nabla\cdot F\,dV$ to the outward flux $\int_{\partial V}F\cdot n\,dS$. For the given field, $\nabla\cdot F=5(x^2+y^2+z^2)=5r^2$, so

$$
\int_V\nabla\cdot F\,dV=4\pi\int_0^R5r^4\,dr=4\pi R^5.
$$

On the sphere, $n=(x,y,z)/R$, and

$$
F\cdot n=\frac{x^4+y^4+z^4+2x^2y^2+2y^2z^2+2z^2x^2}{R}=\frac{r^4}{R}=R^3.
$$

Thus the surface flux is also **$4\pi R^5$**, verifying the theorem by explicit calculation.

Apply the [product rule](../../../calculus.md#product-rule) to $\nabla\cdot(\phi\nabla\psi)=\phi\Delta\psi+\nabla\phi\cdot\nabla\psi$, then apply the [divergence theorem](../../../calculus.md#divergence-theorem). This proves [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity):

$$
\int_V(\phi\Delta\psi+\nabla\phi\cdot\nabla\psi)\,dV=\int_S\phi\,\partial_n\psi\,dS.
$$

Swap $\phi$ and $\psi$ and subtract. The gradient products cancel, giving [Green's second identity](../../../partial-differential-equation.md#green-second-identity):

$$
\int_V(\phi\Delta\psi-\psi\Delta\phi)\,dV=\int_S(\phi\,\partial_n\psi-\psi\,\partial_n\phi)\,dS.
$$

For uniqueness, set $w=\phi_1-\phi_2$. It is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) with zero [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition). Under the stated smoothness assumptions, [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) with $\phi=\psi=w$ gives $\int_V|\nabla w|^2dV=0$. Thus $w$ is constant on each connected component, and its boundary value makes every constant zero. **The two solutions agree throughout $V$.** This is [Dirichlet uniqueness for the Poisson equation](../../../analysis.md#dirichlet-uniqueness-for-the-poisson-equation). For classical solutions merely continuous up to the boundary and twice continuously differentiable in the interior, the [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) gives the same conclusion without requiring boundary derivatives.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
