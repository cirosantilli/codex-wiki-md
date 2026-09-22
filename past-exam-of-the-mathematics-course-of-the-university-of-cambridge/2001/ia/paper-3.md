# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2001/PaperIA_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2001/PaperIA_3.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3C](#3c)
  - [Solution](#3c/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5F](#5f)
  - [Solution](#5f/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7E](#7e)
  - [Solution](#7e/solution)
- [8D](#8d)
  - [i](#8d/i)
    - [Solution](#8d/i/solution)
  - [ii](#8d/ii)
    - [Solution](#8d/ii/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
- [10A](#10a)
  - [Solution](#10a/solution)
- [11B](#11b)
  - [Solution](#11b/solution)
- [12B](#12b)
  - [Solution](#12b/solution)

## 1F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

Put $t=\operatorname{tr}A=a+d$ and $\delta=\det A=ad-bc$. Direct [matrix](../../../vector-space.md#matrix) multiplication gives the two-dimensional [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) identity $A^2-tA+\delta I=0$. If $A^2=0$, [determinant](../../../linear-algebra.md#determinant) multiplicativity gives $\delta^2=0$, hence $\delta=0$. The identity then says $tA=0$. If $A=0$, its [trace](../../../linear-algebra.md#matrix-trace) is zero; otherwise a nonzero entry forces $t=0$. Thus $d=-a$ and $bc=ad=-a^2$.

Conversely, those two scalar relations give $t=\delta=0$, so the same [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) identity implies $A^2=0$. Therefore

$$
\boxed{A^2=0\iff d=-a\text{ and }bc=-a^2.}
$$

This is the [square-zero criterion for a two-by-two matrix](../../../linear-operator-theory.md#square-zero-criterion-for-a-two-by-two-matrix). If $A^3=0$, [determinant](../../../linear-algebra.md#determinant) multiplicativity first gives $\delta^3=0$, hence $\delta=0$. Now $A^2=tA$ and $A^3=t^2A$. Either $A=0$, or a nonzero entry gives $t^2=0$ and hence $t=0$; in both cases $A^2=0$. The converse follows by multiplying $A^2=0$ by $A$. Consequently **$A^3=0\iff A^2=0$**. A nonzero [nilpotent matrix](../../../linear-operator-theory.md#nilpotent-matrix) of this size therefore has nilpotency index two.

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

A [Möbius transformation](../../../group-theory.md#mobius-transformation) is $M_A(z)=(az+b)/(cz+d)$ with $\Delta=ad-bc\ne0$. On the [Riemann sphere](../../../complex-analysis.md#riemann-sphere), a zero denominator represents infinity, and $M_A(\infty)=a/c$ when $c\ne0$; when $c=0$, infinity is fixed. The numerator and denominator cannot vanish together because $\Delta\ne0$.

The [matrix](../../../vector-space.md#matrix) $A=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$ acts on homogeneous coordinates $[z:1]$, so composition satisfies $M_A\circ M_B=M_{AB}$. The product is invertible since $\det(AB)=\det A\det B\ne0$, proving closure. Composition is associative because these are maps of the sphere. The identity is $z\mapsto z$, and

$$
M_A^{-1}(z)=\frac{dz-b}{-cz+a}
$$

is again a [Möbius transformation](../../../group-theory.md#mobius-transformation). Thus the transformations form a [group](../../../group.md). Nonzero scalar multiples of a [matrix](../../../vector-space.md#matrix) give the same transformation, but the identity and inverse assertions concern the transformations themselves.

Write $T_q(z)=z+q$, $S_k(z)=kz$ with $k\ne0$, and $H(z)=1/z$. If $c=0$, then $a,d\ne0$ and $M_A=T_{b/d}\circ S_{a/d}$. If $c\ne0$, division gives

$$
\frac{az+b}{cz+d}=\frac ac-\frac{\Delta/c^2}{z+d/c}.
$$

Hence the [Möbius translation-scaling-inversion factorization](../../../group-theory.md#mobius-translation-scaling-inversion-factorization) is

$$
\boxed{M_A=T_{a/c}\circ S_{-\Delta/c^2}\circ H\circ T_{d/c}\quad(c\ne0).}
$$

The scaling coefficient is nonzero. At $z=-d/c$ the reciprocal sends the translated zero to infinity; at infinity it sends infinity to zero. Thus the factorization holds on the entire [Riemann sphere](../../../complex-analysis.md#riemann-sphere), including both exceptional points, and proves the stated generating property.

## 3C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3c/solution">Solution</h3>

↑ **Parent:** [3C](#3c)

For a differentiable scalar function and a differentiable curve, the multivariable [chain rule](../../../calculus.md#chain-rule) is

$$
\boxed{\frac{d}{dt}f(x(t),y(t))=f_x\frac{dx}{dt}+f_y\frac{dy}{dt}.}
$$

Let $L=x\partial_x-2y\partial_y$. Choose $u=\alpha(x)y$ to be an invariant of the [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics). Then $Lu=y\{x\alpha'(x)-2\alpha(x)\}$, so $x\alpha'=2\alpha$ and a convenient choice is **$\alpha(x)=x^2$**. For $v=y/x$, the [chain rule](../../../calculus.md#chain-rule) gives $Lv=-3v$. Thus, writing the unknown in the new coordinates,

$$
Lf=(Lu)f_u+(Lv)f_v=-3v f_v=6f.
$$

Integrating with $u$ fixed yields

$$
\boxed{f=v^{-2}F(u)=\frac{x^2}{y^2}F(x^2y),\qquad xy\ne0,}
$$

where $F$ is an arbitrary differentiable function on the relevant interval. This gives all local solutions on each patch where the specified change of variables is invertible: its [Jacobian determinant](../../../calculus.md#jacobian-determinant) is $\partial(u,v)/\partial(x,y)=3y$.

The axes need care because $v$ is undefined at $x=0$ and the Jacobian vanishes at $y=0$. Reparameterizing $F(u)=u^2G(u)$ gives the simpler chart expression

$$
\boxed{f(x,y)=x^6G(x^2y)\quad(x\ne0).}
$$

It is the general solution on either component $x>0$ or $x<0$, including $y=0$ when $G$ is differentiable there. Indeed $(x,u=x^2y)$ is a nonsingular [coordinate chart](../../../differential-geometry.md#manifold-chart) for $x\ne0$, and the [weighted Euler first-order equation](../../../partial-differential-equation.md#weighted-euler-first-order-equation) reduces to $x\partial_xf|_u=6f$.

For a patch crossing $x=0$ with $y\ne0$, the characteristic invariant $w=x\sqrt{|y|}$ instead gives $f=|y|^{-3}K(w)$, with an arbitrary differentiable function on each sign component of $y$. These chart descriptions must agree on overlaps. On the axes the original equation gives $f(x,0)=C_\pm x^6$ and $f(0,y)=D_\pm|y|^{-3}$ on their separate components; a solution defined smoothly through the origin must have $f(0,0)=0$ and compatible smooth limits, in particular $D_\pm=0$. No boundary data select a particular arbitrary function.

## 4A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

Consider the globally smooth potential $\Phi(x,y,z)=xy^2\sin(xz)$. Direct differentiation gives

$$
\Phi_x=y^2\sin(xz)+xy^2z\cos(xz)=u,\qquad
\Phi_y=2xy\sin(xz)=v,\qquad
\Phi_z=x^2y^2\cos(xz)=w.
$$

Thus the [differential one-form](../../../differential-form.md#one-form) is the [exact differential](../../../differential-form.md#exact-differential) $d\Phi$, proving exactness rather than only checking a necessary condition on its partial derivatives. Along any piecewise differentiable path, the [chain rule](../../../calculus.md#chain-rule) gives $u\,dx+v\,dy+w\,dz=d\Phi$. The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) therefore makes the [line integral](../../../calculus.md#line-integral) depend only on its endpoints:

$$
\boxed{\int_{(0,0,0)}^{(\pi/2,1,1)}(u\,dx+v\,dy+w\,dz)
=\Phi(\pi/2,1,1)-\Phi(0,0,0)=\frac\pi2.}
$$

## 5F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5f/solution">Solution</h3>

↑ **Parent:** [5F](#5f)

An [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $C$ is a scalar $\lambda$ for which a nonzero vector $v$ satisfies $Cv=\lambda v$. Equivalently, $\det(\lambda I-C)=0$, because the homogeneous linear system has a nontrivial solution exactly when its coefficient [matrix](../../../vector-space.md#matrix) is singular. This [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is the monic quadratic

$$
\lambda^2-(\operatorname{tr}C)\lambda+\det C.
$$

A nonzero quadratic has at most two distinct roots, proving the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) bound. [Eigenvalues](../../../linear-operator-theory.md#eigenvalue) and diagonalization are taken over $\mathbb C$, also for a [matrix](../../../vector-space.md#matrix) with real entries.

For the [matrix commutator](../../../lie-algebra.md#commutator), the cyclic [trace](../../../linear-algebra.md#matrix-trace) identity follows directly from its entries:

$$
\operatorname{tr}(AB)=\sum_{i,j}A_{ij}B_{ji}
=\sum_{i,j}B_{ij}A_{ji}=\operatorname{tr}(BA).
$$

Hence **$\operatorname{tr}[A,B]=0$**. Factoring the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) as $(\lambda-\lambda_1)(\lambda-\lambda_2)$ and comparing the coefficient of $\lambda$ gives **$\operatorname{tr}C=\lambda_1+\lambda_2$**, with the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) counted with algebraic multiplicity. If both [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are zero, [trace](../../../linear-algebra.md#matrix-trace) and [determinant](../../../linear-algebra.md#determinant) are zero. The [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) then gives **$C^2=0$**; no diagonalizability assumption is needed.

Now put $M=[A,B]$. Since its [trace](../../../linear-algebra.md#matrix-trace) is zero, its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is $\lambda^2+\det M$ and the [scalar square of a traceless two-by-two matrix](../../../linear-algebra.md#scalar-square-of-a-traceless-two-by-two-matrix) identity gives

$$
\boxed{[A,B]^2=\alpha I,\qquad \alpha=-\det[A,B]
=\frac12\operatorname{tr}([A,B]^2).}
$$

This proves the scalar-square assertion for both real and complex entries. If $\det M=0$, it gives $M^2=0$. If $\det M\ne0$, the two [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are the distinct nonzero numbers $\pm\sqrt{-\det M}$. Their eigenvectors are [linearly independent](../../../vector-space.md#linear-independence): a nonzero vector cannot satisfy two different [eigenvalue](../../../linear-operator-theory.md#eigenvalue) equations. They form a [basis](../../../vector-space.md#basis), making $M$ a [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix). Thus **either the commutator is diagonalizable over $\mathbb C$ or its square is zero**. These alternatives need not be disjoint, since the zero [matrix](../../../vector-space.md#matrix) has both properties. Over $\mathbb R$ the diagonalization assertion would require real [eigenvalues](../../../linear-operator-theory.md#eigenvalue); complex diagonalization is essential to the unrestricted statement.

## 6E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

A left [group action](../../../group-theory.md#group-action) of $G$ on a set $X$ is a map $(g,x)\mapsto g\cdot x$ satisfying $e\cdot x=x$ and $(gh)\cdot x=g\cdot(h\cdot x)$. The [group orbit](../../../group-theory.md#orbit-of-a-group-action) of $x$ is $G\cdot x=\{g\cdot x:g\in G\}$, and its [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) is $G_x=\{g\in G:g\cdot x=x\}$. The [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) contains the identity, is closed under products, and contains $g^{-1}$ whenever it contains $g$, so it is indeed a [subgroup](../../../group.md#subgroup).

The [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) for a finite [group](../../../group.md) says

$$
\boxed{|G|=|G\cdot x|\,|G_x|.}
$$

To prove it, map a left [coset](../../../group-theory.md#coset) $gG_x$ to $g\cdot x$. This is well-defined because every element of $G_x$ fixes $x$. Conversely, $g\cdot x=h\cdot x$ precisely when $h^{-1}g\in G_x$, which is precisely equality of the two [cosets](../../../group-theory.md#coset). Thus this map is a [bijection](../../../function.md#bijection) between the [cosets](../../../group-theory.md#coset) and the [group orbit](../../../group-theory.md#orbit-of-a-group-action). Each [coset](../../../group-theory.md#coset) has $|G_x|$ elements, by the [bijection](../../../function.md#bijection) $k\mapsto gk$, and the [cosets](../../../group-theory.md#coset) partition $G$, giving the formula.

Apply this to the [rotational symmetry group of a cube](../../../group-theory.md#rotational-symmetry-group-of-a-cube) acting on its six faces. The action is transitive: rotations through right angles about coordinate axes can send the top face to each of the other faces. A rotation fixing a face must fix its outward normal, so it rotates about the axis through that face's center and the opposite face's center. Preservation of its square boundary permits exactly four angles modulo $2\pi$: $0,\pi/2,\pi,3\pi/2$. All four preserve the cube, so this face [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) has order four. The [group](../../../group.md) is finite because a rotation permutes the six face normals and is determined by their images. The [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) gives

$$
\boxed{|\operatorname{Rot}(\text{cube})|=6\times4=24.}
$$

These are orientation-preserving rotations; reflections are not being counted.

## 7E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7e/solution">Solution</h3>

↑ **Parent:** [7E](#7e)

[Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) states that for a [subgroup](../../../group.md#subgroup) $H$ of a finite [group](../../../group.md) $G$, $|G|=[G:H]|H|$; in particular $|H|$ divides $|G|$. This follows by partitioning $G$ into [cosets](../../../group-theory.md#coset), each in [bijection](../../../function.md#bijection) with $H$.

If $|G|=p$ is prime, take any $g\ne e$. Its [cyclic subgroup](../../../group.md#cyclic-subgroup) has order dividing $p$, but its order is not one. Thus it has order $p$ and equals $G$. Hence

$$
\boxed{\text{Every group of order }p\text{ is cyclic and isomorphic to }C_p.}
$$

This describes a single [group isomorphism](../../../algebra.md#group-isomorphism) type for each prime.

Now let $G=\langle x\rangle$ have order $n$, and let $H$ be any [subgroup](../../../group.md#subgroup). Choose the least positive integer $d$ with $x^d\in H$; this exists because $x^n=e\in H$, even when $H$ is trivial. Divide $n=qd+r$ with $0\le r<d$. Since $x^r=x^n(x^d)^{-q}\in H$, minimality forces $r=0$, so $d$ divides $n$. Likewise, dividing an exponent $k=qd+r$ for any $x^k\in H$ shows $r=0$. Therefore $H=\langle x^d\rangle$.

Conversely, for each divisor $d$ of $n$, $\langle x^d\rangle$ is a [subgroup](../../../group.md#subgroup) of order $n/d$. The least positive exponent property makes $d$ unique. This proves the complete [subgroups and quotients of a cyclic group](../../../group.md#subgroups-and-quotients-of-a-cyclic-group) classification:

$$
\boxed{H=\langle x^d\rangle\ (d\mid n),\quad |H|=n/d;
\qquad H_m=\langle x^{n/m}\rangle\text{ is the unique subgroup of order }m\ (m\mid n).}
$$

The choices $d=n$ and $d=1$ include the trivial [subgroup](../../../group.md#subgroup) and the whole [group](../../../group.md).

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/i">i</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/i/solution">Solution</h4>

↑ **Parent:** [I](#8d/i)

Compose [permutations](../../../combinatorics.md#permutation) from right to left. The indicated cycle lengths immediately give $X^3=P^2=Q^2=e$. Under [conjugation](../../../group-theory.md#conjugation), $X^{-1}(ab)X=(X^{-1}a\ X^{-1}b)$. Since $X^{-1}$ sends $1,2,3$ to $3,1,2$ and fixes $4$,

$$
\boxed{X^{-1}PX=(31)(24)=Q,\qquad
X^{-1}QX=(32)(14)=(14)(23)=PQ.}
$$

Direct composition also gives $PQ=QP=(14)(23)$. Thus $V=\{e,P,Q,PQ\}$ is a [Klein four-group](../../../finite-group-theory.md#klein-four-group). [Conjugation](../../../group-theory.md#conjugation) by $X$ cycles its three nonidentity elements, so $X$ normalizes $V$.

The [cosets](../../../group-theory.md#coset) $V,VX,VX^2$ have four elements each and are distinct. If two coincided, a nontrivial power of $X$ would belong to $V$, impossible because it has order three whereas every nonidentity element of $V$ has order two. Hence the [subgroup](../../../group.md#subgroup) generated by $X,P,Q$ contains at least twelve elements. These generators are [even permutations](../../../finite-group-theory.md#even-permutation), so the [subgroup](../../../group.md#subgroup) lies in the [alternating group](../../../finite-group-theory.md#alternating-group) $A_4$, whose order is $4!/2=12$; multiplying by one fixed transposition pairs even and odd [permutations](../../../combinatorics.md#permutation) to justify this count. Therefore

$$
\boxed{A_4=\langle X,P,Q\rangle.}
$$

The calculation also describes $A_4$ as the [semidirect product](../../../group-theory.md#semidirect-product) $V\rtimes\langle X\rangle$, with the order-three factor permuting the three involutions.

<h3 id="8d/ii">ii</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8d/ii)

The [direct product of groups](../../../group-theory.md#direct-product-of-groups) uses componentwise multiplication:

$$
(g,h)(g',h')=(gg',hh'),\qquad e=(e_G,e_H),\qquad
(g,h)^{-1}=(g^{-1},h^{-1}).
$$

Associativity follows in each factor. The maps $g\mapsto(g,e_H)$ and $h\mapsto(e_G,h)$ are injective [group homomorphisms](../../../group-theory.md#group-homomorphism) onto [subgroups](../../../group.md#subgroup), giving the required copies of $G$ and $H$.

Use the PDF's convention that the subscript in $D_n$ is the [group](../../../group.md) order. Write the hexagon [group](../../../group.md) as $D_{12}=\langle r,s\mid r^6=s^2=e,\ srs=r^{-1}\rangle$ and the triangle [group](../../../group.md) as $D_6=\langle a,b\mid a^3=b^2=e,\ bab=a^{-1}\rangle$. Let $z$ generate $C_2$. In $D_{12}$, $r^2$ has order three and $s$ conjugates it to its inverse, so $\langle r^2,s\rangle$ is a copy of $D_6$. The element $r^3$ has order two and is central, since $sr^3s=r^{-3}=r^3$.

Define

$$
\Phi(a^ib^j,z^k)=r^{2i+3k}s^j,
\qquad 0\le i<3,\quad 0\le j,k<2.
$$

The generator relations are preserved and $r^3$ commutes with the other images, so $\Phi$ is a [group homomorphism](../../../group-theory.md#group-homomorphism) from the direct product. The six residues $2i+3k$ are distinct modulo six: reduction modulo two first determines $k$, then reduction modulo three determines $i$. Together with $j$, they give all twelve distinct normal forms $r^ms^j$ in $D_{12}$. Thus $\Phi$ is bijective and

$$
\boxed{D_{12}\cong D_6\times C_2.}
$$

This is the [dihedral splitting when the half-rotation order is odd](../../../finite-group-theory.md#dihedral-splitting-when-the-half-rotation-order-is-odd) with half-rotation order three.

Finally, $D_{12}$ contains an element of order six, namely $r$. The even cycle types on four symbols are the identity, a 3-cycle, and two disjoint transpositions; their orders are respectively one, three and two. Therefore $A_4$ has no element of order six. Since a [group isomorphism](../../../algebra.md#group-isomorphism) preserves element orders,

$$
\boxed{D_{12}\not\cong A_4.}
$$

## 9C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

At a [critical point](../../../analysis.md#critical-point) $x_0$ of a twice continuously differentiable real function, the [Taylor expansion](../../../calculus.md#taylor-expansion) is

$$
f(x_0+h)=f(x_0)+\frac12h^THh+o(|h|^2),\qquad H=\nabla^2f(x_0).
$$

The [Hessian matrix](../../../calculus.md#hessian-matrix) is real symmetric, so an orthogonal eigenbasis diagonalizes its [quadratic form](../../../linear-algebra.md#quadratic-form). If every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is positive, that form is bounded below by a positive multiple of $|h|^2$, which dominates the remainder and gives a strict [local minimum](../../../analysis.md#local-minimum). If every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is negative, the same argument gives a strict [local maximum](../../../analysis.md#local-maximum). If both signs occur, displacement along the corresponding eigenvectors produces values above and below $f(x_0)$, so the point is a [saddle point of a scalar function](../../../analysis.md#saddle-point-of-a-scalar-function). These exhaust a nonsingular [Hessian matrix](../../../calculus.md#hessian-matrix).

A singular [Hessian matrix](../../../calculus.md#hessian-matrix) does not always make the classification impossible: nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of both signs still give a saddle. If the [Hessian matrix](../../../calculus.md#hessian-matrix) is positive or negative semidefinite, higher-order terms in its null directions must be examined. For example, $x^2+y^4$ and $x^2-y^4$ have the same [Hessian matrix](../../../calculus.md#hessian-matrix) $\operatorname{diag}(2,0)$ at zero, but the first has a strict minimum and the second a saddle. The function $x^2$ has a non-strict minimum along a whole line.

For the given polynomial,

$$
f_x=2x(\alpha-3y+4x^2),\qquad f_y=2y-3x^2.
$$

A stationary point has $y=3x^2/2$ and then $x(2\alpha-x^2)=0$. Hence the origin is always critical, and two additional points exist exactly for $\alpha>0$:

$$
\boxed{(x,y)=(\pm\sqrt{2\alpha},3\alpha).}
$$

The [Hessian matrix](../../../calculus.md#hessian-matrix) is

$$
H=\begin{pmatrix}2\alpha-6y+24x^2&-6x\\-6x&2\end{pmatrix}.
$$

At the origin it is $\operatorname{diag}(2\alpha,2)$, giving a strict [local minimum](../../../analysis.md#local-minimum) for $\alpha>0$ and a saddle for $\alpha<0$. At either extra [critical point](../../../analysis.md#critical-point) it has [determinant](../../../linear-algebra.md#determinant) $64\alpha-36(2\alpha)=-8\alpha<0$, so both extra points are saddles.

At $\alpha=0$, complete the square:

$$
f(x,y)=\left(y-\frac32x^2\right)^2-\frac14x^4.
$$

Along $x=0$ it is positive away from zero, whereas along $y=3x^2/2$ it is negative away from zero. Thus the origin remains a degenerate saddle despite its nonnegative [Hessian matrix](../../../calculus.md#hessian-matrix). This is the [parabolic quartic critical-point classification](../../../analysis.md#parabolic-quartic-critical-point-classification). The complete result is

$$
\boxed{\begin{array}{c|c}
\alpha<0&(0,0)\text{ is the only critical point, a saddle}\\
\alpha=0&(0,0)\text{ is the only critical point, a degenerate saddle}\\
\alpha>0&(0,0)\text{ is a strict local minimum; }(\pm\sqrt{2\alpha},3\alpha)\text{ are saddles}.
\end{array}}
$$

For $\alpha>0$ the [local minimum](../../../analysis.md#local-minimum) is not global, since along the same parabola $f=\alpha x^2-x^4/4\to-\infty$.

## 10A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10a/solution">Solution</h3>

↑ **Parent:** [10A](#10a)

For a one-to-one continuously differentiable change of variables with nonzero [Jacobian determinant](../../../calculus.md#jacobian-determinant), the [change of variables formula](../../../calculus.md#change-of-variables-formula) rule is

$$
\iint_D F(x,y)\,dx\,dy
=\iint_E F(x(u,v),y(u,v))
\left|\det\frac{\partial(x,y)}{\partial(u,v)}\right|\,du\,dv,
$$

where $E$ is the transformed region and the inverse map covers $D$ once. The absolute value is required even if the coordinate map reverses orientation.

Here $x,y$ are positive. For $u=y/x$, $v=xy$, the inverse is $x=\sqrt{v/u}$ and $y=\sqrt{uv}$. On the first portion of $D$, the bounds give $v\ge1$, $u\le4$ and $v\le u$ because $x\le1$. Together these give $1\le v\le u\le4$; conversely these inequalities imply $1/2\le x\le1$ and the original bounds. On the second portion, they give $u\ge1$, $v\le4$ and $v\ge u$, hence $1\le u\le v\le4$, with the converse following similarly. The two triangles combine into the rectangle **$E=\{1\le u\le4,\ 1\le v\le4\}$**, sharing only the diagonal corresponding to $x=1$.

The Jacobian is

$$
\det\frac{\partial(u,v)}{\partial(x,y)}
=\det\begin{pmatrix}-y/x^2&1/x\\y&x\end{pmatrix}=-\frac{2y}{x}=-2u,
\qquad
\left|\det\frac{\partial(x,y)}{\partial(u,v)}\right|=\frac1{2u}.
$$

Also $xy^3=uv^2$ and $x^2+y^2=v(1+u^2)/u$. The transformed integral consequently factors:

$$
\iint_D\frac{4xy^3}{x^2+y^2}\,dx\,dy
=\int_1^4\int_1^4\frac{2uv}{1+u^2}\,dv\,du
=\left[\frac{v^2}{2}\right]_1^4
\left[\log(1+u^2)\right]_1^4.
$$

Therefore

$$
\boxed{\iint_D\frac{4xy^3}{x^2+y^2}\,dx\,dy=\frac{15}{2}\log\frac{17}{2}.}
$$

## 11B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11b/solution">Solution</h3>

↑ **Parent:** [11B](#11b)

The [divergence theorem](../../../calculus.md#divergence-theorem) states that a continuously differentiable [vector field](../../../calculus.md#vector-field) on a bounded region $V$ satisfies

$$
\int_V\nabla\cdot\mathbf u\,dV=\int_{\partial V}\mathbf u\cdot\mathbf n\,dS,
$$

with outward [unit normal](../../../differential-geometry.md#unit-normal) $\mathbf n$ and a sufficiently regular boundary; piecewise smooth boundaries are also allowed. For $\mathbf u=\mathbf c\,\Omega$ with constant $\mathbf c$, the left side is $\mathbf c\cdot\int_V\nabla\Omega\,dV$ and the right side is $\mathbf c\cdot\int_{\partial V}\Omega\mathbf n\,dS$. Equality for every constant vector gives the [gradient volume-to-boundary identity](../../../calculus.md#gradient-volume-to-boundary-identity)

$$
\boxed{\int_V\nabla\Omega\,dV=\int_{\partial V}\Omega\,d\mathbf S.}
$$

For the cone and its cap, the volume has $0\le z\le1$ and $0\le r\le\sqrt3z$ in [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system). Its volume is $\int_0^1\pi(\sqrt3z)^2\,dz=\pi$. Since $\nabla\Omega=-\mathbf e_z$,

$$
\int_V\nabla\Omega\,dV=-\pi\mathbf e_z.
$$

The cap at $z=1$ has area $3\pi$, outward normal $\mathbf e_z$ and $\Omega=a-1$, so its contribution to the [surface integral](../../../calculus.md#surface-integral) is $3\pi(a-1)\mathbf e_z$.

Parameterize the side by $\mathbf R(r,\theta)=(r\cos\theta,r\sin\theta,r/\sqrt3)$, $0\le r\le\sqrt3$, $0\le\theta<2\pi$. The outward [vector area element](../../../differential-geometry.md#vector-area-element) is

$$
d\mathbf S=(\mathbf R_\theta\times\mathbf R_r)\,dr\,d\theta
=\left(\frac r{\sqrt3}\mathbf e_r-r\mathbf e_z\right)dr\,d\theta,
$$

pointing radially outward and downward from the region above the cone. The radial part integrates to zero around the circle. The vertical part of the side integral is

$$
-2\pi\int_0^{\sqrt3}\left(a-\frac r{\sqrt3}\right)r\,dr\,\mathbf e_z
=(-3\pi a+2\pi)\mathbf e_z.
$$

Adding cap and side gives

$$
\boxed{\int_{\partial V}(a-z)\,d\mathbf S
=\{3\pi(a-1)-3\pi a+2\pi\}\mathbf e_z
=-\pi\mathbf e_z
=\int_V\nabla(a-z)\,dV.}
$$

The apex and circular rim have zero surface area. Alternatively, removing a tiny apex neighborhood and taking its radius to zero justifies applying the smooth-boundary theorem there; the additional flux vanishes because the scalar field is bounded.

## 12B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12b/solution">Solution</h3>

↑ **Parent:** [12B](#12b)

Let $\phi_1,\phi_2$ be two sufficiently regular solutions with the same source and boundary data, and set $w=\phi_1-\phi_2$. Then $\nabla^2w=0$ and $\alpha\partial_nw+w=0$. [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) gives

$$
\int_V|\nabla w|^2\,dV
=\int_{\partial V}w\,\partial_nw\,dS
=-\int_{\partial V}\alpha(\partial_nw)^2\,dS\le0.
$$

The left side is nonnegative, so it vanishes. Thus $w$ is constant on each connected component. Its [normal derivative](../../../differential-geometry.md#normal-derivative) is zero, and the [boundary condition](../../../differential-equation.md#boundary-condition) then forces that constant to be zero. This proves **at most one solution**. The [Poisson uniqueness with a nonnegative Robin normal coefficient](../../../differential-equation.md#poisson-uniqueness-with-a-nonnegative-robin-normal-coefficient) proof never divides by $\alpha$, so it includes the points or boundary portions where $\alpha=0$.

For the exponential-sine modes, direct differentiation gives

$$
\partial_x^2(e^{\pm\ell x}\sin\ell y)=\ell^2e^{\pm\ell x}\sin\ell y,
\qquad
\partial_y^2(e^{\pm\ell x}\sin\ell y)=-\ell^2e^{\pm\ell x}\sin\ell y.
$$

Their sum is zero, so both modes are [harmonic functions](../../../partial-differential-equation.md#harmonic-function) for every real $\ell$.

For the square, the horizontal Dirichlet data suggest [separation of variables](../../../partial-differential-equation.md#separation-of-variables) in the form $\phi(x,y)=F(x)\sin(ky)$, where the positive integer $k$ makes the sine vanish at both horizontal edges. The [Laplace equation](../../../partial-differential-equation.md#laplace-equation) gives $F''-k^2F=0$, hence $F=A\cosh(kx)+B\sinh(kx)$. At $x=0$, the outward normal points in the negative $x$ direction. The [Robin boundary condition](../../../differential-equation.md#robin-boundary-condition) is therefore $F(0)-F'(0)=0$, or $A=kB$. The right edge requires $F(\pi)=1$, fixing the remaining coefficient. The resulting [separated Laplace mode with a Robin edge](../../../partial-differential-equation.md#separated-laplace-mode-with-a-robin-edge) is

$$
\boxed{\phi(x,y)=\frac{k\cosh(kx)+\sinh(kx)}{k\cosh(k\pi)+\sinh(k\pi)}\sin(ky).}
$$

The denominator is positive for $k>0$. The function satisfies the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) and all four [boundary conditions](../../../differential-equation.md#boundary-condition) directly; for example its left-edge value and $x$ derivative agree, giving the correct outward-normal Robin sign. It extends regularly to the corners.

On the left edge the uniqueness coefficient is $\alpha=1$; on the other three edges it is $\alpha=0$ with the prescribed Dirichlet value. The same [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) argument applies to the square's piecewise smooth boundary, whose corners have zero boundary measure. Thus **this is the unique regular solution**, or equivalently the unique finite-energy solution with these boundary traces. Unbounded corner singularities are outside that boundary-value class.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
