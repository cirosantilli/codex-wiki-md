# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2003/PaperIA_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2003/PaperIA_3.pdf)

**Table of contents**

- [1A](#1a)
  - [Solution](#1a/solution)
- [2B](#2b)
  - [Solution](#2b/solution)
- [3A](#3a)
  - [Solution](#3a/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5E](#5e)
  - [a](#5e/a)
    - [Solution](#5e/a/solution)
  - [b](#5e/b)
    - [Solution](#5e/b/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7B](#7b)
  - [i](#7b/i)
    - [Solution](#7b/i/solution)
  - [ii](#7b/ii)
    - [Solution](#7b/ii/solution)
- [8B](#8b)
  - [a](#8b/a)
    - [Solution](#8b/a/solution)
  - [b](#8b/b)
    - [Solution](#8b/b/solution)
- [9A](#9a)
  - [Solution](#9a/solution)
- [10A](#10a)
  - [Solution](#10a/solution)
- [11A](#11a)
  - [a](#11a/a)
    - [Solution](#11a/a/solution)
  - [b](#11a/b)
    - [Solution](#11a/b/solution)
- [12A](#12a)
  - [Solution](#12a/solution)

## 1A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1a/solution">Solution</h3>

↑ **Parent:** [1A](#1a)

Use the standard ordered [basis](../../../vector-space.md#basis) $(\mathbf e_1,\mathbf e_2,\mathbf e_3)$ for both maps. The [reflection in a hyperplane](../../../linear-algebra.md#reflection-in-a-hyperplane) interchanges the second and third coordinates, so its [matrix](../../../vector-space.md#matrix) is

$$
\boxed{A=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix}}.
$$

Orient the rotation axis along $\mathbf n=(1,1,1)/\sqrt3$ and use the right-hand convention. The [rotation matrix](../../../linear-algebra.md#rotation-matrix) for angle $2\pi/3$ sends $\mathbf e_1$ to $\mathbf e_2$, $\mathbf e_2$ to $\mathbf e_3$, and $\mathbf e_3$ to $\mathbf e_1$. For example, the [Rodrigues rotation formula](../../../mathematics.md#rodrigues-rotation-formula) gives

$$
R\mathbf e_1=\cos\frac{2\pi}{3}\,\mathbf e_1+\sin\frac{2\pi}{3}(\mathbf n\times\mathbf e_1)+\left(1-\cos\frac{2\pi}{3}\right)(\mathbf n\cdot\mathbf e_1)\mathbf n=\mathbf e_2.
$$

Multiplying the [rotation matrix](../../../linear-algebra.md#rotation-matrix) by the dilation factor gives

$$
\boxed{B=2R=\begin{pmatrix}0&0&2\\2&0&0\\0&2&0\end{pmatrix}}.
$$

Direct multiplication gives $A^2=I$, $B^2=4\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix}$ and $B^3=8I$. Hence **$B^3=8A^2$**. If the opposite axis orientation is chosen, $B=2R^T$ also has cube $8I$. Independently of coordinates, two applications of the [reflection](../../../linear-algebra.md#reflection-mathematics) give the identity, while three applications of the rotation-dilation give a full turn and dilation by $2^3$. Every [basis](../../../vector-space.md#basis) represents these resulting maps by $I$ and $8I$. Thus the equality even holds when the two [matrices](../../../vector-space.md#matrix) are expressed in different [bases](../../../vector-space.md#basis).

## 2B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2b/solution">Solution</h3>

↑ **Parent:** [2B](#2b)

Let $H,K$ be the [normal subgroups](../../../group-theory.md#normal-subgroup) of orders $3,5$. Their intersection is a [subgroup](../../../group.md#subgroup) of both, so [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) makes its order divide both $3$ and $5$; hence $H\cap K=\{1\}$. For $h\in H$ and $k\in K$, normality shows that $hkh^{-1}k^{-1}$ belongs to both $H$ and $K$. It must be the identity, so $hk=kh$. This proves the needed instance of [normal subgroups of coprime order commute](../../../group-theory.md#normal-subgroups-of-coprime-order-commute).

Choose nonidentity $h\in H$ and $k\in K$. Their orders are $3$ and $5$, since these orders divide the respective prime subgroup orders. If $(hk)^m=1$, commutativity gives $h^m=k^{-m}\in H\cap K$, so $3\mid m$ and $5\mid m$. Conversely $(hk)^{15}=1$. Thus the [product of commuting elements of coprime order](../../../group-theory.md#product-of-commuting-elements-of-coprime-order) gives **an element $hk$ of order $15$**.

For the counterexample, take the [dihedral group](../../../finite-group-theory.md#dihedral-group) of symmetries of a regular pentagon:

$$
\boxed{D_5=\langle r,s\mid r^5=s^2=1,\ srs=r^{-1}\rangle}.
$$

Its ten elements are $r^j$ and $sr^j$, $0\le j<5$. Nonidentity rotations have order $5$, and $(sr^j)^2=r^{-j}r^j=1$, so all [reflections](../../../linear-algebra.md#reflection-mathematics) have order $2$. **There is no element of order $10$.**

## 3A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3a/solution">Solution</h3>

↑ **Parent:** [3A](#3a)

The curve is a [hyperbola](../../../geometry-and-topology.md#hyperbola) with two branches, vertices $(0,1)$ and $(0,-1)$, and asymptotes $y=\pm x$. It is symmetric under [reflection](../../../linear-algebra.md#reflection-mathematics) in either coordinate axis. The requested sketch marks both vertices:

<a id="3a/image-two-branches-of-the-hyperbola-with-its-asymptotes-and-the-points-of-minimum-radius-of-curvature"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-3-hyperbola.png)

**[Figure 1](#3a/image-two-branches-of-the-hyperbola-with-its-asymptotes-and-the-points-of-minimum-radius-of-curvature). Two branches of the hyperbola, with its asymptotes and the points of minimum radius of curvature**.

Parametrize the branches by $x=\sinh t$, $y=\pm\cosh t$, for $t\in\mathbb R$. The squared speed is $\dot x^2+\dot y^2=\cosh^2t+\sinh^2t=\cosh2t$, and $|\dot x\ddot y-\ddot x\dot y|=|\cosh^2t-\sinh^2t|=1$. The reciprocal of the [curvature of a plane curve](../../../differential-geometry.md#curvature-of-a-plane-curve) is therefore

$$
\boxed{\mathcal R(t)=(\cosh2t)^{3/2}=(1+2x^2)^{3/2}}.
$$

Since $\cosh2t\ge1$, with equality only at $t=0$, **the least radius is $1$, attained at $(0,1)$ and $(0,-1)$**.

## 4A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

Suppose $\phi_1,\phi_2$ are two sufficiently regular solutions with the same [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition), and put $w=\phi_1-\phi_2$. Then $\Delta w=0$ in $V$ and $w=0$ on its boundary. Apply the [divergence theorem](../../../calculus.md#divergence-theorem) to $w\nabla w$:

$$
\int_V\bigl(|\nabla w|^2+w\Delta w\bigr)\,dV=\int_S w\,\partial_nw\,dS=0.
$$

Thus $\nabla w=0$ throughout $V$, so $w$ is constant on each connected component. Its zero boundary values force every such constant to be zero. This proves **uniqueness of the Dirichlet solution**, without assuming its existence.

For a prescribed [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition), the difference instead has $\partial_nw=0$. The same energy argument still gives $\nabla w=0$, but does not fix the constant. Consequently **the solution is unique up to an additive constant on each connected component**. A value at one point, or the integral mean, fixes the constant on a connected region. There is also a necessary compatibility condition: if $g=\partial_n\phi$ on $S$, the [divergence theorem](../../../calculus.md#divergence-theorem) gives

$$
\boxed{\int_S g\,dS=\int_V\Delta\phi\,dV=0}.
$$

It is required on each component if the region is disconnected. Data failing this condition admit no harmonic solution. This is the homogeneous-source instance of the [Neumann Poisson problem](../../../partial-differential-equation.md#neumann-poisson-problem).

## 5E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5e/a">a</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/a/solution">Solution</h4>

↑ **Parent:** [A](#5e/a)

Move the origin to the [centroid](../../../geometry-and-topology.md#centroid) and write the four vertex vectors as $r_1,r_2,r_3,r_4$. Their sum is zero. The [midpoints](../../../mathematical-optimization.md#midpoint) of the first opposite-edge pair have vectors $(r_1+r_2)/2$ and $(r_3+r_4)/2=-(r_1+r_2)/2$, so their distances from the [centroid](../../../geometry-and-topology.md#centroid) are equal. The same argument applies to the other two opposite-edge pairs.

Choose the three [midpoint](../../../mathematical-optimization.md#midpoint) distances as $u=|r_1+r_2|/2$, $v=|r_1+r_3|/2$, $w=|r_1+r_4|/2$. Expanding the [dot products](../../../linear-algebra.md#dot-product),

$$
4(u^2+v^2+w^2)=3|r_1|^2+\sum_{j=2}^4|r_j|^2+2r_1\cdot\sum_{j=2}^4r_j=\sum_{i=1}^4|r_i|^2.
$$

Identifying these four norms with the vertex distances proves the [tetrahedron centroid-to-midpoint sum of squares](../../../geometry-and-topology.md#tetrahedron-centroid-to-midpoint-sum-of-squares):

$$
\boxed{u^2+v^2+w^2=\frac14(a^2+b^2+c^2+d^2)}.
$$

The proof uses no orthogonality or regularity assumption on the [tetrahedron](../../../geometry-and-topology.md#tetrahedron).

<h3 id="5e/b">b</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/b/solution">Solution</h4>

↑ **Parent:** [B](#5e/b)

Put $v=x-a$ and decompose it into axial and perpendicular parts, $v=(v\cdot n)n+v_\perp$. For the nondegenerate semi-angle $0<\alpha<\pi/2$, the equation is equivalent to

$$
|v_\perp|^2\cos^2\alpha=(v\cdot n)^2\sin^2\alpha,\qquad |v_\perp|=|v\cdot n|\tan\alpha.
$$

Thus each plane perpendicular to $n$ at axial distance $s$ from $a$ meets the surface in a circle of radius $|s|\tan\alpha$. Both signs of $s$ are allowed, and $s=0$ gives the vertex. This proves that it is a [double circular cone](../../../geometry-and-topology.md#double-circular-cone) with the specified vertex and axis; $\alpha$ is the angle each generator makes with either direction of the axis.

For the intersection calculation, define the symmetric [matrix](../../../vector-space.md#matrix) $Q=\cos^2\alpha\,I-nn^T$. The two equations are $(x-a_i)^TQ(x-a_i)=0$. Their difference gives

$$
-2x\cdot Q(a_1-a_2)+a_1\cdot Qa_1-a_2\cdot Qa_2=0.
$$

With $b=a_1-a_2$ and $m=(a_1+a_2)/2$, symmetry of $Q$ makes the last two terms $2m\cdot Qb$. Hence the [intersection plane of parallel congruent double cones](../../../geometry-and-topology.md#intersection-plane-of-parallel-congruent-double-cones) is

$$
\boxed{(Qb)\cdot(x-m)=0}.
$$

The unnormalized [normal vector](../../../differential-geometry.md#normal-vector) is $v=Qb=b\cos^2\alpha-n(n\cdot b)$. Expanding its squared norm gives

$$
|v|^2=|b|^2\cos^4\alpha+(n\cdot b)^2(1-2\cos^2\alpha).
$$

Equivalently, if $b=b_\perp+(n\cdot b)n$, this is $\cos^4\alpha|b_\perp|^2+\sin^4\alpha(n\cdot b)^2>0$. Thus normalization is legitimate and yields

$$
\boxed{N=\frac{b\cos^2\alpha-n(n\cdot b)}{\sqrt{|b|^2\cos^4\alpha+(n\cdot b)^2(1-2\cos^2\alpha)}}}.
$$

The assumption of a genuine cone matters: at the degenerate limits $\alpha=0$ or $\pi/2$, the surface collapses respectively to an axis or a plane and this normal need not exist.

## 6E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

Write the row components as $E_{ai}=(e_a)_i$. Expanding the [cross product](../../../vector-space.md#cross-product) in components,

$$
(e_1\times e_2)\cdot e_3=\epsilon_{ijk}(e_1)_i(e_2)_j(e_3)_k
$$

equals the alternating six-term expansion of the [determinant](../../../linear-algebra.md#determinant) of $E$. Therefore **$(e_1\times e_2)\cdot e_3=\det E$**.

Geometrically, $|e_1\times e_2|$ is the area of the parallelogram spanned by $e_1,e_2$, and its direction is perpendicular to that plane. A nonzero [scalar triple product](../../../linear-algebra.md#scalar-triple-product) means both that this area is nonzero and that $e_3$ has a nonzero component normal to the plane. Thus the vectors are [linearly independent](../../../vector-space.md#linear-independence) and form a [basis](../../../vector-space.md#basis) of $\mathbb R^3$, without needing to be orthogonal. Equivalently, their parallelepiped has nonzero volume.

The entries of $E\hat E^T$ are $e_a\cdot\hat e_b$, so the required duality is exactly $E\hat E^T=I$. Since $E$ is invertible, this has the unique solution

$$
\boxed{\hat E^T=E^{-1},\qquad \hat E=E^{-T}}.
$$

Its [determinant](../../../linear-algebra.md#determinant) is $1/\det E\ne0$, so its rows are again a [basis](../../../vector-space.md#basis). Put $\Delta=(e_1\times e_2)\cdot e_3$. The [cross product](../../../vector-space.md#cross-product) $e_2\times e_3$ is perpendicular to $e_2,e_3$, and its [dot product](../../../linear-algebra.md#dot-product) with $e_1$ is $\Delta$. Consequently the [reciprocal basis](../../../linear-algebra.md#reciprocal-basis) is

$$
\boxed{\hat e_1=\frac{e_2\times e_3}{\Delta},\qquad \hat e_2=\frac{e_3\times e_1}{\Delta},\qquad \hat e_3=\frac{e_1\times e_2}{\Delta}}.
$$

These vectors have precisely the required [dot products](../../../linear-algebra.md#dot-product), so uniqueness identifies them with the rows of $E^{-T}$.

For the final request, an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of rows gives $EE^T=I$. If instead the reciprocal rows are [orthonormal](../../../linear-algebra.md#orthonormal-set), then $\hat E\hat E^T=I$ and substitution of $\hat E=E^{-T}$ gives $E^{-T}E^{-1}=I$, again implying $EE^T=I$. Thus in either case **$E$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix)** and $\hat E=E$.

The further printed claim that $E$ must be a [rotation matrix](../../../linear-algebra.md#rotation-matrix) is false without an orientation assumption. The [matrix](../../../vector-space.md#matrix) $E=\operatorname{diag}(1,1,-1)$ has orthonormal rows and is its own [reciprocal basis](../../../linear-algebra.md#reciprocal-basis) [matrix](../../../vector-space.md#matrix), but $\det E=-1$: it is a [reflection](../../../linear-algebra.md#reflection-mathematics). By the [orientation of an orthonormal reciprocal basis](../../../linear-algebra.md#orientation-of-an-orthonormal-reciprocal-basis), the corrected conclusion is

$$
\boxed{E\in O(3),\qquad E\text{ is a rotation matrix if and only if }\det E=+1.}
$$

A right-handed original ordered [basis](../../../vector-space.md#basis) supplies exactly this missing condition.

## 7B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7b/i">i</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/i/solution">Solution</h4>

↑ **Parent:** [I](#7b/i)

If all three points are finite, define the [Möbius transformation](../../../group-theory.md#mobius-transformation)

$$
\boxed{g(z)=\frac{\beta-\gamma}{\beta-\alpha}\,\frac{z-\alpha}{z-\gamma}}.
$$

Its numerator vanishes at $\alpha$, its pole is at $\gamma$, and substitution of $\beta$ gives $1$. The three points are distinct, so the numerator and denominator are not proportional and the associated $2\times2$ [matrix](../../../vector-space.md#matrix) has nonzero [determinant](../../../linear-algebra.md#determinant).

If one point is infinite, the limiting formulas are

$$
\boxed{\begin{array}{c|c}
\text{infinite point}&g(z)\\\hline
\alpha=\infty&(\beta-\gamma)/(z-\gamma)\\
\beta=\infty&(z-\alpha)/(z-\gamma)\\
\gamma=\infty&(z-\alpha)/(\beta-\alpha)
\end{array}}.
$$

In each case the finite values and the limit at infinity give $g(\alpha)=0$, $g(\beta)=1$, $g(\gamma)=\infty$, and the corresponding [determinant](../../../linear-algebra.md#determinant) is nonzero. Distinctness permits at most one of the points to be infinite. Hence **every ordered triple of distinct points on the Riemann sphere can be normalized to $(0,1,\infty)$**.

<h3 id="7b/ii">ii</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7b/ii)

Each element of $H$ permutes the three-point set, giving a [group homomorphism](../../../group-theory.md#group-homomorphism) $\rho:H\to S_3$. To prove injectivity, let an element fix all three points. Conjugate it by the normalizing [Möbius transformation](../../../group-theory.md#mobius-transformation) from part (i). The conjugate fixes $0,1,\infty$. A [Möbius transformation](../../../group-theory.md#mobius-transformation) $z\mapsto(az+b)/(cz+d)$ fixing $0$ has $b=0$, and fixing infinity has $c=0$. It is then $z\mapsto kz$; fixing $1$ forces $k=1$. Thus the conjugate, and hence the original transformation, is the identity. The [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is trivial.

For surjectivity, let $(x_1,x_2,x_3)=(\alpha,\beta,\gamma)$ and choose any permutation $\sigma$. Let $g$ normalize the ordered triple $(x_1,x_2,x_3)$ and let $g_\sigma$ normalize $(x_{\sigma(1)},x_{\sigma(2)},x_{\sigma(3)})$. Then $g_\sigma^{-1}g$ sends $x_j$ to $x_{\sigma(j)}$, lies in $H$, and induces the chosen permutation. Thus $\rho$ is onto and

$$
\boxed{H\cong S_3}.
$$

For the normalized set, the six [Möbius transformations permuting three points](../../../group-theory.md#mobius-transformations-permuting-three-points) are $z$, $1-z$, $1/z$, $1/(1-z)$, $z/(z-1)$, and $(z-1)/z$. Conjugating by $g$ gives the corresponding six maps for the original set.

## 8B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8b/a">a</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/a/solution">Solution</h4>

↑ **Parent:** [A](#8b/a)

Using the monic convention for the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial), expand the [determinant](../../../linear-algebra.md#determinant) along the last column:

$$
\boxed{\chi_A(t)=\det(tI-A)=(t-2)\det\begin{pmatrix}t&-1\\1&t-2\end{pmatrix}=(t-2)(t-1)^2}.
$$

For the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $1$, the equations $(A-I)v=0$ give $v_2=v_1$ and $v_3=0$. Thus every corresponding nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector) is a nonzero multiple of $(1,1,0)^T$. For the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $2$, the first two equations give $v_2=2v_1$ and $v_1=0$, so every corresponding nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector) is a nonzero multiple of $(0,0,1)^T$. Therefore

$$
\boxed{E_1=\operatorname{span}\{(1,1,0)^T\},\qquad E_2=\operatorname{span}\{(0,0,1)^T\}}.
$$

These [eigenspaces](../../../linear-operator-theory.md#eigenspace) together have dimension $2$, so they cannot provide an [eigenvector](../../../linear-operator-theory.md#eigenvector) [basis](../../../vector-space.md#basis) of $\mathbb R^3$. **The [matrix](../../../vector-space.md#matrix) is not diagonalizable**; the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $1$ has algebraic multiplicity $2$ but geometric multiplicity $1$.

<h3 id="8b/b">b</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/b/solution">Solution</h4>

↑ **Parent:** [B](#8b/b)

The [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) has only the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\mu$. If $A$ is [diagonalizable](../../../linear-operator-theory.md#diagonalizable-matrix), there is an invertible [matrix](../../../vector-space.md#matrix) $P$ and a diagonal [matrix](../../../vector-space.md#matrix) $D$ with $A=PDP^{-1}$. Every diagonal entry of $D$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue), hence equals $\mu$. Thus $D=\mu I$ and $A=P(\mu I)P^{-1}=\mu I$. Conversely, $\mu I$ is already diagonal in every [basis](../../../vector-space.md#basis). Hence

$$
\boxed{A\text{ is diagonalizable}\quad\Longleftrightarrow\quad A=\mu I}.
$$

This argument uses the existence of an [eigenvector](../../../linear-operator-theory.md#eigenvector) [basis](../../../vector-space.md#basis) rather than merely the repeated root of the polynomial; repeated [eigenvalues](../../../linear-operator-theory.md#eigenvalue) alone do not imply diagonalizability.

## 9A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9a/solution">Solution</h3>

↑ **Parent:** [9A](#9a)

Orient the triangular boundary from $P=(1,0,0)$ to $Q=(0,1,0)$ to $R=(0,0,1)$ and back to $P$. This orientation corresponds to the positive [normal vector](../../../differential-geometry.md#normal-vector) $(Q-P)\times(R-P)=(1,1,1)$. The cyclic coordinate rotation $(x,y,z)\mapsto(z,x,y)$ sends the three directed edges to one another and transforms the [vector field](../../../calculus.md#vector-field) by the same rotation. Since rotations preserve [dot products](../../../linear-algebra.md#dot-product), the three edge contributions to the [line integral](../../../calculus.md#line-integral) are equal.

On the first edge use $x=1-t$, $y=t$, $z=0$, $0\le t\le1$. Then

$$
A\cdot\frac{d\mathbf x}{dt}=(-t^2,(1-t)^2,t^2-(1-t)^2)\cdot(-1,1,0)=t^2+(1-t)^2.
$$

Its integral is $2/3$, so the required [circulation](../../../fluid-mechanics.md#circulation-physics) is

$$
\boxed{\oint_C A\cdot d\mathbf x=3\cdot\frac23=2}.
$$

For a sufficiently smooth [vector field](../../../calculus.md#vector-field) on an oriented piecewise smooth surface $T$, with induced boundary orientation on $C=\partial T$, the [Stokes theorem](../../../calculus.md#stokes-theorem) states

$$
\int_T(\nabla\times A)\cdot n\,dS=\oint_C A\cdot d\mathbf x.
$$

Therefore the requested [surface integral](../../../calculus.md#surface-integral), with all normal components positive, is also **$2$**.

To verify it directly, parametrize the triangle by $\mathbf r(y,z)=(1-y-z,y,z)$ on $y\ge0$, $z\ge0$, $y+z\le1$. Its two tangent vectors are $\mathbf r_y=(-1,1,0)$ and $\mathbf r_z=(-1,0,1)$, giving the [vector area element](../../../differential-geometry.md#vector-area-element)

$$
\boxed{d\mathbf S=(\mathbf r_y\times\mathbf r_z)\,dy\,dz=(1,1,1)\,dy\,dz}.
$$

Differentiation of the [vector field](../../../calculus.md#vector-field) gives $\nabla\times A=2(y+z,z+x,x+y)$. On the triangle $x+y+z=1$, so its [dot product](../../../linear-algebra.md#dot-product) with $(1,1,1)$ is $4$. Consequently

$$
\int_T(\nabla\times A)\cdot d\mathbf S=\int_0^1\int_0^{1-y}4\,dz\,dy=2,
$$

confirming both the magnitude and the orientation sign.

## 10A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10a/solution">Solution</h3>

↑ **Parent:** [10A](#10a)

For the printed integration formula, $J$ must mean the [Jacobian determinant](../../../calculus.md#jacobian-determinant) of the inverse coordinate map:

$$
\boxed{J=\frac{\partial(x,y,z)}{\partial(u,v,w)}=\det\begin{pmatrix}x_u&x_v&x_w\\y_u&y_v&y_w\\z_u&z_v&z_w\end{pmatrix}}.
$$

If instead one calls $\partial(u,v,w)/\partial(x,y,z)$ the forward Jacobian, its [determinant](../../../linear-algebra.md#determinant) is $1/J$ where the derivative is invertible. This convention distinction resolves the direction of the arrow in the printed wording.

To derive the [change of variables formula](../../../calculus.md#change-of-variables-formula), a small rectangular cell of side lengths $du,dv,dw$ maps under the inverse transformation, to first order, to a parallelepiped with edge vectors $\mathbf r_u\,du$, $\mathbf r_v\,dv$, $\mathbf r_w\,dw$. Its volume is the absolute [scalar triple product](../../../linear-algebra.md#scalar-triple-product) of those vectors:

$$
dx\,dy\,dz=|\mathbf r_u\cdot(\mathbf r_v\times\mathbf r_w)|\,du\,dv\,dw=|J|\,du\,dv\,dw.
$$

For a one-to-one continuously differentiable coordinate map with continuously differentiable inverse, summing these local volume contributions and taking the partition limit gives

$$
\boxed{\int_D f(x,y,z)\,dx\,dy\,dz=\int_\Delta f(x(u,v,w),y(u,v,w),z(u,v,w))\,|J|\,du\,dv\,dw}.
$$

The absolute value removes an orientation reversal; injectivity ensures that each volume element is counted once.

For positive semi-axes, take $u=x/a$, $v=y/b$, $w=z/c$. The [solid ellipsoid](../../../geometry-and-topology.md#solid-ellipsoid) becomes the unit ball and the inverse [Jacobian determinant](../../../calculus.md#jacobian-determinant) is $abc$. Thus

$$
\int_Dx^2\,dV=a^3bc\int_{u^2+v^2+w^2\le1}u^2\,du\,dv\,dw.
$$

Rotational symmetry gives equal integrals of $u^2,v^2,w^2$ over the ball. Their sum is the integral of $r^2$, so [spherical coordinates](../../../calculus.md#spherical-coordinate-system) give $\int u^2\,dV=\frac13\int_0^1 4\pi r^4\,dr=4\pi/15$. The [Cartesian second moment of a solid ellipsoid](../../../geometry-and-topology.md#cartesian-second-moment-of-a-solid-ellipsoid) is therefore

$$
\boxed{\int_Dx^2\,dx\,dy\,dz=\frac{4\pi}{15}a^3bc}.
$$

## 11A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11a/a">a</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/a/solution">Solution</h4>

↑ **Parent:** [A](#11a/a)

Use [suffix notation](../../../linear-algebra.md#einstein-notation), summing repeated indices. The [contraction of two Levi-Civita symbols](../../../calculus.md#contraction-of-two-levi-civita-symbols) gives

$$
[F\times(\nabla\times G)]_i=\epsilon_{ijk}F_j\epsilon_{k\ell m}\partial_\ell G_m=F_j\partial_iG_j-F_j\partial_jG_i.
$$

Adding the [directional derivative](../../../calculus.md#directional-derivative) $(F\cdot\nabla)G_i=F_j\partial_jG_i$ cancels the second term. Interchanging $F,G$ gives another pair whose sum is $G_j\partial_iF_j$. The total right-hand side is therefore

$$
F_j\partial_iG_j+G_j\partial_iF_j=\partial_i(F_jG_j),
$$

the $i$th component of the [gradient](../../../calculus.md#gradient) of the [dot product](../../../linear-algebra.md#dot-product). Since this holds for each component, the [dot-product gradient identity](../../../calculus.md#dot-product-gradient-identity) is proved:

$$
\boxed{\nabla(F\cdot G)=(F\cdot\nabla)G+(G\cdot\nabla)F+F\times(\nabla\times G)+G\times(\nabla\times F)}.
$$

It holds for any continuously differentiable [vector fields](../../../calculus.md#vector-field); no irrotationality assumption is used.

<h3 id="11a/b">b</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/b/solution">Solution</h4>

↑ **Parent:** [B](#11a/b)

Take $E$ to be continuously differentiable everywhere on $\mathbb R^3$, as in the question. Its zero [curl](../../../calculus.md#curl) says $\partial_iE_j=\partial_jE_i$. Construct a [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field) explicitly by

$$
\phi(x)=-\int_0^1E(tx)\cdot x\,dt.
$$

All segments lie in $\mathbb R^3$. Differentiating under the integral and using the symmetry of the derivatives,

$$
\partial_i\phi=-\int_0^1[E_i(tx)+t x_j\partial_iE_j(tx)]\,dt=-\int_0^1[E_i(tx)+t x_j\partial_jE_i(tx)]\,dt=-\int_0^1\frac{d}{dt}[tE_i(tx)]\,dt=-E_i(x).
$$

Hence **$E=-\nabla\phi$**. This [radial integral potential for a curl-free field](../../../calculus.md#radial-integral-potential-for-a-curl-free-field) also works on a star-shaped domain after translating its centre. On an arbitrary domain, zero [curl](../../../calculus.md#curl) only guarantees local potentials; the everywhere-on-$\mathbb R^3$ interpretation is important for this global assertion.

For the given field, put $q=e^{-x^2z}$. The three pairs of derivatives entering its [curl](../../../calculus.md#curl) are

$$
\partial_yE_z=2x^2yq=\partial_zE_y,\qquad \partial_zE_x=2xy^2(1-x^2z)q=\partial_xE_z,\qquad \partial_xE_y=4xyzq=\partial_yE_x.
$$

Thus the field is [irrotational](../../../calculus.md#irrotational-vector-field). To find its potential using $E_y=-\partial_y\phi$, integrate $\partial_y\phi=2yq$ to get $\phi=y^2q+\psi(x,z)$. Comparison with $E_x=-\partial_x\phi$ gives $\psi_x=0$, and comparison with $E_z=-\partial_z\phi$ gives $\psi_z=0$. Therefore

$$
\boxed{\phi(x,y,z)=y^2e^{-x^2z}+C}.
$$

Differentiating this expression reproduces all three components with the required minus sign; the only freedom on the connected domain is the additive constant.

## 12A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

For a sufficiently regular [vector field](../../../calculus.md#vector-field) $F$ on a bounded region $V$ with piecewise smooth boundary $S$, the [divergence theorem](../../../calculus.md#divergence-theorem) states

$$
\int_V\nabla\cdot F\,dV=\int_S F\cdot n\,dS,
$$

where $n$ is the outward unit [normal vector](../../../differential-geometry.md#normal-vector). Apply it to $F=fk$ for an arbitrary constant vector $k$. Since $\nabla\cdot(fk)=k\cdot\nabla f$, it gives

$$
k\cdot\int_V\nabla f\,dV=k\cdot\int_S f n\,dS.
$$

Equality for every constant $k$ proves the [vector gradient form of the divergence theorem](../../../calculus.md#vector-gradient-form-of-the-divergence-theorem):

$$
\boxed{\int_V\nabla f\,dV=\int_S f\,d\mathbf S}.
$$

Applying the same [divergence theorem](../../../calculus.md#divergence-theorem) directly to $G$, with $\nabla\cdot G=\rho$, proves the flux law

$$
\boxed{\int_SG\cdot d\mathbf S=\int_V\rho\,dV}.
$$

This is the Gauss flux law for the prescribed source density, obtained directly from the [divergence theorem](../../../calculus.md#divergence-theorem). For the piecewise source in this problem the divergence relation is understood away from the interface, or almost everywhere; applying the theorem separately to the two sides gives the same law because the normal field is continuous across the interface and the internal boundary fluxes cancel.

For the radial field, its normal component on a sphere of radius $r$ is the constant $G(r)$, so its total flux is $4\pi r^2G(r)$. For $0<r\le a$ the enclosed source is $4\pi\rho_0r^3/3$; for $r>a$ it is $4\pi\rho_0a^3/3$. Thus the [origin-regular spherical Poisson flux law](../../../geometry-and-topology.md#origin-regular-spherical-poisson-flux-law) gives

$$
\boxed{G(x)=\begin{cases}\dfrac{\rho_0}{3}x,&r\le a,\\\dfrac{\rho_0a^3}{3r^3}x,&r>a.\end{cases}}
$$

The value at $r=0$ is the continuous value zero. A singular inverse-square radial addition is excluded by the source equation throughout space, including the origin: it would add a point source there.

Since $G=\nabla f$, radial integration gives $f_r=\rho_0r/3$ inside and $f_r=\rho_0a^3/(3r^2)$ outside. The decay condition fixes the exterior constant, giving $f=-\rho_0a^3/(3r)$ for $r\ge a$. Integrating inside gives $f=\rho_0r^2/6+C_0$, and matching at $r=a$ yields $C_0=-\rho_0a^2/2$. Hence the [potential of a uniform spherical source](../../../geometry-and-topology.md#potential-of-a-uniform-spherical-source) is

$$
\boxed{f(x)=\begin{cases}\dfrac{\rho_0}{6}(r^2-3a^2),&r\le a,\\-\dfrac{\rho_0a^3}{3r},&r\ge a.\end{cases}}
$$

Both $f$ and its radial derivative are continuous at $a$; there is no surface source hidden in the matching.

For any ball centred at the origin, the [gradient](../../../calculus.md#gradient) $G(x)$ is odd under $x\mapsto-x$, so its volume integral vanishes by symmetry. On the bounding sphere, $f$ is constant and outward normals at antipodal points are opposite, so $\int_S f n\,dS=0$ as well. **Both sides of the vector [gradient](../../../calculus.md#gradient) identity are therefore zero**, for radii below, above, or equal to $a$.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
