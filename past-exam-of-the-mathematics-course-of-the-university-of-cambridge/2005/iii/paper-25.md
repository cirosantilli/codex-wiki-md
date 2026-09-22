# Paper 25

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper25.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper25.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use tangent vectors, rather than the affine tangent plane, to differentiate. Every skew-symmetric [matrix](../../../vector-space.md#matrix) $A$ gives a curve $X\exp(tA)$ in the [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group). Its first derivative under $f$ is $\operatorname{tr}(CXA)$. The trace pairing annihilates every skew-symmetric [matrix](../../../vector-space.md#matrix) precisely when $CX$ is symmetric: choosing $A$ with only entries $a_{ij}=-a_{ji}$ tests each off-diagonal antisymmetric entry. Thus criticality is equivalent to $Y=CX$ being symmetric.

Since $X$ is orthogonal, $YY^T=C^2$, so at a [critical point](../../../analysis.md#critical-point) $Y^2=C^2$. Consequently $Y$ commutes with $C^2$. The diagonal entries $c_i^2$ are distinct, and the equation $YC^2=C^2Y$ gives $(c_j^2-c_i^2)y_{ij}=0$ for $i\ne j$. Hence $Y$ and $X$ are diagonal. Orthogonality and the determinant constraint give exactly

$$
\boxed{D=\operatorname{diag}(\varepsilon_1,\ldots,\varepsilon_n),\qquad\varepsilon_i\in\{1,-1\},\quad\prod_i\varepsilon_i=1.}
$$

Conversely each such $D$ makes $CD$ symmetric, so this list is complete.

To calculate the [Hessian matrix](../../../calculus.md#hessian-matrix), use local coordinates $X=\exp(A)D$ with $A^T=-A$; the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) is a local coordinate map near zero. Its quadratic term gives

$$
\operatorname{Hess}_D f(A,A)=\operatorname{tr}(CA^2D)=-\sum_{i<j}(c_i\varepsilon_i+c_j\varepsilon_j)a_{ij}^2,
$$

because $(A^2)_{ii}=-\sum_{j\ne i}a_{ij}^2$. There are no mixed quadratic terms. For $i<j$, $c_j>c_i>0$, so $c_i\varepsilon_i+c_j\varepsilon_j$ has the sign of $\varepsilon_j$ and is never zero. Every listed [critical point](../../../analysis.md#critical-point) is therefore nondegenerate, with [Morse index](../../../differential-geometry.md#morse-index)

$$
\boxed{\operatorname{ind}(D)=\#\{(i,j):i<j,\ \varepsilon_j=1\}=\sum_{j:\varepsilon_j=1}(j-1).}
$$

This is the [trace height on the special orthogonal group](../../../linear-algebra.md#trace-height-on-the-special-orthogonal-group) calculation; the rotations in the hint select the individual coordinates $a_{ij}$.

For $n=3$, the signs $(+--),(-+-),(--+),(+++)$ have indices $0,1,2,3$ respectively. A [Morse function](../../../differential-geometry.md#morse-function) on a compact closed [manifold](../../../topology.md#topological-manifold) has [Euler characteristic](../../../homology.md#euler-characteristic) equal to the alternating number of [critical points](../../../analysis.md#critical-point), by its [Morse handle-attachment theorem](../../../differential-geometry.md#morse-handle-attachment-theorem) and resulting finite [CW complex](../../../algebraic-topology.md#cw-complex). Hence

$$
\boxed{\chi(SO(3))=1-1+1-1=0.}
$$

## 2

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The usual compact closed-manifold hypothesis is needed for the first assertion, or a proper bounded-below Morse exhaustion in an appropriate noncompact version. As literally printed without any such condition, $f(x)=x$ on $\mathbb R$ is a [Morse function](../../../differential-geometry.md#morse-function) with no [critical points](../../../analysis.md#critical-point), while $b_0=1$. We prove the intended closed-manifold statement, which applies to the [surface](../../../topology.md#topological-surface) product later in the question.

By the [Morse handle-attachment theorem](../../../differential-geometry.md#morse-handle-attachment-theorem), crossing an index-$i$ [critical point](../../../analysis.md#critical-point) attaches an $i$-handle, and no topological change occurs between critical levels. Retraction to the [core disks of handles](../../../topology.md#core-disk-of-a-handle) gives a [CW complex](../../../algebraic-topology.md#cw-complex) model with $c_i$ cells in dimension $i$. Its [cellular chain complex](../../../homology.md#cellular-chain-complex) has $C_i\cong\mathbb Z^{c_i}$. Tensor with $\mathbb Q$, which computes the ranks $b_i$ of integral [homology](../../../homology.md). Since [homology](../../../homology.md) is a quotient of a [vector subspace](../../../vector-space.md#vector-subspace) of $C_i\otimes\mathbb Q$, **$b_i\le c_i$**. This argument has not used the [Morse inequalities](../../../differential-geometry.md#morse-inequalities).

The strong [Morse inequalities](../../../differential-geometry.md#morse-inequalities) and top-dimensional equality are

$$
\boxed{\sum_{i=0}^j(-1)^{j-i}c_i\ge\sum_{i=0}^j(-1)^{j-i}b_i\quad(0\le j\le m),\qquad\sum_{i=0}^m(-1)^ic_i=\sum_{i=0}^m(-1)^ib_i.}
$$

Their weak form is $c_i\ge b_i$. To see the algebra behind the strong form, put $r_i=\operatorname{rank}_{\mathbb Q}\partial_i$ in the [Morse chain complex](../../../differential-geometry.md#morse-chain-complex), with $r_0=r_{m+1}=0$. The kernel-image dimensions give $c_i=b_i+r_i+r_{i+1}$, so the alternating difference at $j$ is exactly $r_{j+1}\ge0$. Conversely, given the strong inequalities, denote those alternating differences by $S_j$, with $S_{-1}=0$. Then $c_j-b_j=S_j+S_{j-1}\ge0$, proving that they imply every weak inequality.

They are **not equivalent as numerical restrictions**. For the [Betti numbers](../../../homology.md#betti-number) $b=(1,0,0,1)$ of $S^3$, the formal counts $c=(2,0,0,2)$ satisfy all weak inequalities and the Euler equality, but at $j=1$ give $c_1-c_0=-2<-1=b_1-b_0$. They therefore cannot be the counts of a [Morse function](../../../differential-geometry.md#morse-function) on $S^3$; the strong inequalities detect that additional obstruction.

If all the strong inequalities are equalities, all $r_i$ vanish and $c_i=b_i$. An integer boundary [matrix](../../../vector-space.md#matrix) with rational rank zero is the zero [matrix](../../../vector-space.md#matrix). Thus the integral complex itself has zero differential, not merely its rationalization. Consequently

$$
\boxed{H_i(M;\mathbb Z)\cong\mathbb Z^{c_i}=\mathbb Z^{b_i}\quad(0\le i\le m),}
$$

and higher [homology](../../../homology.md) vanishes. In particular there is no [homology](../../../homology.md) torsion. This is an integral consequence of a [Perfect Morse function](../../../differential-geometry.md#perfect-morse-function), rather than just an assertion about ranks.

For $\Sigma_g$, the integral [homology](../../../homology.md) is free with [Betti numbers](../../../homology.md#betti-number) $(1,2g,1)$. The [Künneth theorem](../../../cohomology.md#kunneth-theorem) therefore has no torsion terms, and the product's [Poincaré polynomial](../../../homology.md#poincare-polynomial) is

$$
(1+2gt+t^2)^2=1+4gt+(4g^2+2)t^2+4gt^3+t^4.
$$

Summing the weak inequalities yields the lower bound

$$
\boxed{\#\operatorname{Crit}(F)\ge4g^2+8g+4=(2g+2)^2\quad\text{for Morse }F.}
$$

Choose a [surface](../../../topology.md#topological-surface) [Morse function](../../../differential-geometry.md#morse-function) $h$ with one minimum, $2g$ saddles and one maximum. It can be built from one [closed disk](../../../topology.md#closed-disc), the standard $2g$ [one-handles](../../../topology.md#one-handle), and a closing [closed disk](../../../topology.md#closed-disc), using the local forms $u^2+v^2$, $-u^2+v^2$, and $-u^2-v^2$ at the [handle](../../../topology.md#handle) centres. Regular collars interpolate between the [handles](../../../topology.md#handle) without new [critical points](../../../analysis.md#critical-point). Now set $F(x,y)=h(x)+h(y)$. Its [critical points](../../../analysis.md#critical-point) are the ordered pairs of those of $h$, and its [Hessian matrix](../../../calculus.md#hessian-matrix) is a block direct sum; the indices add. This [product of Morse functions](../../../differential-geometry.md#product-of-morse-functions) has exactly **$(2g+2)^2$ [critical points](../../../analysis.md#critical-point)** and realizes every displayed Betti count. Small bumps constant near the critical pairs can separate their values without altering the [Hessians](../../../calculus.md#hessian-matrix) or creating new [critical points](../../../analysis.md#critical-point).

The same minimum does **not** apply to arbitrary [smooth functions](../../../analysis.md#smooth-function). Here is an explicit finite-critical-point counterexample, avoiding any assumption that degeneracy leaves the Morse lower bound intact. On $T^2=(\mathbb R/\pi\mathbb Z)^2$, take

$$
h_0(u,v)=\sin u\sin v\sin(u-v).
$$

It is well defined because shifting either coordinate by $\pi$ reverses two of its factors. Its derivatives are $\sin v\sin(2u-v)$ and $\sin u\sin(u-2v)$. If either $\sin u$ or $\sin v$ vanishes, both derivatives vanish only at $(0,0)$. Otherwise $2u-v$ and $u-2v$ must be multiples of $\pi$, giving exactly $(\pi/3,2\pi/3)$ and $(2\pi/3,\pi/3)$ in addition to the origin. At the first point the [Hessian](../../../calculus.md#hessian-matrix) is $\sqrt3\bigl(\begin{smallmatrix}1&-1/2\\-1/2&1\end{smallmatrix}\bigr)$, positive definite; at the second it is its negative. They are a minimum and maximum. The origin is an isolated degenerate [monkey saddle](../../../analysis.md#monkey-saddle), with leading term $uv(u-v)$. Thus this [three-critical-point function on a torus](../../../topology.md#three-critical-point-function-on-a-torus) has exactly three [critical points](../../../analysis.md#critical-point).

For $g>1$, perform [connected-sum gluing of functions](../../../differential-geometry.md#connected-sum-gluing-of-functions) between this [torus](../../../topology.md#torus) and a perfect Morse [surface](../../../topology.md#topological-surface) of genus $g-1$: delete a small neighbourhood of the [torus](../../../topology.md#torus) maximum and of the other [surface](../../../topology.md#topological-surface)'s minimum, and join their regular boundary circles by a monotone cylinder. Collar coordinates ensure nonzero differential throughout the neck, so precisely those two [critical points](../../../analysis.md#critical-point) are lost and none are added. The result on $\Sigma_g$ has $3+[2(g-1)+2]-2=2g+1$ [critical points](../../../analysis.md#critical-point), retaining the degenerate point. For $g=1$, simply use $h_0$. Calling this [smooth function](../../../analysis.md#smooth-function) $\widetilde h$ and the earlier perfect [Morse function](../../../differential-geometry.md#morse-function) $h$, the smooth product $\widetilde h(x)+h(y)$ has

$$
\boxed{(2g+1)(2g+2)<(2g+2)^2}
$$

[critical points](../../../analysis.md#critical-point). This explicitly proves the negative answer to the unrestricted smooth-minimum question; it does not assert that this smaller illustrative count is sharp.

<a id="2/image-the-explicit-three-critical-point-torus-function-and-the-local-merger-of-two-morse-saddles-into-one-degenerate-saddle"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-25-critical-points.png)

**[Figure 1](#2/image-the-explicit-three-critical-point-torus-function-and-the-local-merger-of-two-morse-saddles-into-one-degenerate-saddle). The explicit three-critical-point torus function and the local merger of two Morse saddles into one degenerate saddle**.

## 3

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a framed embedding $S^{\lambda-1}\times D^{m+1-\lambda}\hookrightarrow M^m$, index-$\lambda$ [surgery on a smooth manifold](../../../topology.md#surgery-on-a-smooth-manifold) removes the interior of that region and replaces it by $D^\lambda\times S^{m-\lambda}$. Their common boundary is $S^{\lambda-1}\times S^{m-\lambda}$, along which the framing specifies the gluing. This is a $(\lambda,m+1-\lambda)$ surgery. Its trace is an $(m+1)$-dimensional [cobordism](../../../geometry-and-topology.md#cobordism) obtained by attaching the [handle](../../../topology.md#handle) $D^\lambda\times D^{m+1-\lambda}$ to $M\times[0,1]$ along the outgoing boundary.

In the present [surface](../../../topology.md#topological-surface) case, $\lambda=2$ and $m=2$. The operation removes an annulus around the embedded curve $\gamma$ and caps its two boundary circles by [closed disks](../../../topology.md#closed-disc). Since $[\gamma]=pa+qb\ne0$, the curve cannot separate the oriented [torus](../../../topology.md#torus): a separating curve is the oriented boundary of one of the complementary subsurfaces and is therefore null-homologous. Thus it is a [nonseparating curve](../../../geometry-and-topology.md#nonseparating-curve), and the cut-open [surface](../../../topology.md#topological-surface) $F$ is connected with two boundary components. Its [Euler characteristic](../../../homology.md#euler-characteristic) is zero, since both the removed annulus and the gluing circles have [Euler characteristic](../../../homology.md#euler-characteristic) zero. Capping adds two, so the resulting oriented closed connected [surface](../../../topology.md#topological-surface) has $\chi(M)=2$. By the allowed [surface](../../../topology.md#topological-surface) classification it is a [sphere](../../../geometry-and-topology.md#sphere). Therefore

$$
\boxed{H_0(M;\mathbb Z)=\mathbb Z,\qquad H_1(M;\mathbb Z)=0,\qquad H_2(M;\mathbb Z)=\mathbb Z,\qquad H_i(M;\mathbb Z)=0\ (i>2).}
$$

Equivalently the classification shows that $F$ is a cylinder. The argument is conditional on the asserted embedding existing; it does not assign a surgery [manifold](../../../topology.md#topological-manifold) to a nonexistent embedded curve.

Choose an arc in this connected cylinder joining its two boundary circles and close it by an arc crossing the removed annulus. After smoothing the joints, its closed curve $\delta$ meets $\gamma$ transversely exactly once. If $[\delta]=ra+sb$, then their [algebraic intersection number of curves on an oriented surface](../../../topology.md#algebraic-intersection-number-of-curves-on-an-oriented-surface) is

$$
[\gamma]\cdot[\delta]=ps-qr=\pm1.
$$

This proves that $[\gamma]$ is a [primitive homology class](../../../homology.md#primitive-homology-class) and forces $\gcd(p,q)=1$.

Conversely, if $\gcd(p,q)=1$, the map

$$
\mathbb R/\mathbb Z\longrightarrow(\mathbb R/\mathbb Z)^2,\qquad t\longmapsto(pt,qt)
$$

is an immersion with the required [homology](../../../homology.md) class. If its values at $t,s$ coincide, then $p(t-s)$ and $q(t-s)$ are integers; [Bézout's identity](../../../algebra.md#bezout-identity) gives $t-s\in\mathbb Z$. It is therefore injective and, by compactness, an embedded circle. An explicit annular thickening is

$$
\iota(t,u)=(pt-q\delta u,\ qt+p\delta u)\pmod{\mathbb Z^2},\qquad u\in[-1,1],\quad0<\delta<\frac1{2(p^2+q^2)}.
$$

The determinant of its coordinate derivatives is $\delta(p^2+q^2)\ne0$. If two image points coincide, solving for the difference in the normal coordinate shows that $\delta(u-u')$ is an integer multiple of $1/(p^2+q^2)$. The strict choice of $\delta$ forces that integer to be zero, so $u=u'$ and then $t=t'$ modulo one. This supplies the actual required embedding, not just a [homology](../../../homology.md) class. Hence

$$
\boxed{\text{a positive }(p,q)\text{-curve exists if and only if }\gcd(p,q)=1.}
$$

## 4

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Choose real constants $a_0<a_1<\cdots<a_m$ and define the smooth homogeneous quotient

$$
\boxed{f([x_0:\cdots:x_m])=\frac{\sum_{j=0}^ma_jx_j^2}{\sum_{j=0}^mx_j^2}.}
$$

It is unchanged by nonzero rescaling, so it is well defined on [Real projective space](../../../algebraic-topology.md#real-projective-space). On the unit [sphere](../../../geometry-and-topology.md#sphere) its differential vanishes on the [tangent space](../../../differential-geometry.md#tangent-space) precisely when $Ax$ is proportional to $x$, where $A=\operatorname{diag}(a_0,\ldots,a_m)$. The entries are distinct, so the only critical projective lines are $p_i=[e_i]$. In the affine chart $x_i=1$, write $u_j=x_j/x_i$ for $j\ne i$. Then

$$
f=a_i+\frac{\sum_{j\ne i}(a_j-a_i)u_j^2}{1+\sum_{j\ne i}u_j^2}.
$$

Its [Hessian](../../../calculus.md#hessian-matrix) at zero is diagonal with entries $2(a_j-a_i)$. Exactly $i$ are negative, and none vanish. Thus this is a [Morse function](../../../differential-geometry.md#morse-function) with **one [critical point](../../../analysis.md#critical-point) $p_i$ of index $i$ for every $0\le i\le m$**.

Choose the quotient of the round metric on the unit [sphere](../../../geometry-and-topology.md#sphere). The downward [gradient flow](../../../analysis.md#gradient-flow) has [sphere](../../../geometry-and-topology.md#sphere) equation $\dot x_j=-2(a_j-f(x))x_j$ and projective solution

$$
[x_0(t):\cdots:x_m(t)]=[e^{-2a_0t}x_0(0):\cdots:e^{-2a_mt}x_m(0)].
$$

Normalization to the unit [sphere](../../../geometry-and-topology.md#sphere) supplies the common positive factor. As $t\to+\infty$, the smallest index with nonzero coordinate dominates; as $t\to-\infty$, the largest dominates. Consequently

$$
W^u(p_i)=\{x_i\ne0,\ x_j=0\ (j>i)\}\cong\mathbb R^i,\qquad W^s(p_i)=\{x_i\ne0,\ x_j=0\ (j<i)\}\cong\mathbb R^{m-i}.
$$

These are its [unstable manifolds](../../../dynamical-systems.md#unstable-manifold) and [stable manifolds](../../../dynamical-systems.md#stable-manifold). If $j\ge k$, the tangent directions in $W^u(p_j)$ allow coordinates $0,\ldots,j$, and those in $W^s(p_k)$ allow $k,\ldots,m$, modulo the common projective line. Together they span the full [tangent space](../../../differential-geometry.md#tangent-space) at every intersection. If $j<k$ the intersection is empty. Thus the flow is a [Morse-Smale gradient flow](../../../analysis.md#morse-smale-gradient-flow), with no generic perturbation needed.

Orient each unstable [manifold](../../../topology.md#topological-manifold) using its affine coordinates. The [Morse-Smale complex](../../../differential-geometry.md#morse-smale-complex) has $C_i=\mathbb Z p_i$; its differential counts oriented unparametrized connecting trajectories of index difference one. A trajectory from $p_i$ to $p_{i-1}$ has only coordinates $x_{i-1},x_i$ nonzero, and there are exactly two, distinguished by the sign of $x_{i-1}/x_i$. Each sign branch is a single orbit modulo time translation.

To calculate their signs rather than merely count two, use the characteristic [closed disk](../../../topology.md#closed-disc) of the unstable cell: the closed upper hemisphere of $S^i$ with $x_i\ge0$, followed by projection onto $\mathbb{RP}^i$. Its interior is $W^u(p_i)$, and its boundary map is the antipodal double cover $S^{i-1}\to\mathbb{RP}^{i-1}$. After collapsing $\mathbb{RP}^{i-2}$, its degree on the $(i-1)$-cell is the sum of the degrees of the two sheets. Comparing the sheets by the [antipodal map](../../../homology.md#antipodal-map) on $S^{i-1}$ gives relative orientation $(-1)^i$: it is induced by $-I$ on $\mathbb R^i$, whose determinant is $(-1)^i$. Thus the two trajectory signs add to $1+(-1)^i$, up to the choice of generator orientations. The [projective quadratic Morse complex](../../../differential-geometry.md#projective-quadratic-morse-complex) is therefore

$$
\boxed{C_i=\mathbb Z\ (0\le i\le m),\qquad\partial_i=\begin{cases}2,&i\text{ even},\\0,&i\text{ odd}.\end{cases}}
$$

In particular $\partial_1=0$, as required for the connected one-dimensional skeleton. The signed trajectory count agrees with this attaching-map incidence calculation, so it computes integral rather than only mod-two [homology](../../../homology.md).

For $m\ge1$, taking kernels modulo images gives

$$
\boxed{H_k(\mathbb{RP}^m;\mathbb Z)=\begin{cases}\mathbb Z,&k=0,\\\mathbb Z/2,&0<k<m\text{ and }k\text{ odd},\\\mathbb Z,&k=m\text{ and }m\text{ odd},\\0,&\text{otherwise}.\end{cases}}
$$

For example, an odd interior-degree generator has zero outgoing differential but twice itself is the image from the next degree; an even positive-degree differential is injective. At the top there is no incoming differential, leaving a copy of $\mathbb Z$ exactly when $m$ is odd. For $m=0$ the space is one point and only $H_0=\mathbb Z$ remains. This recovers the [cellular homology of real projective space](../../../algebraic-topology.md#cellular-homology-of-real-projective-space) by explicitly constructing its [Morse-Smale complex](../../../differential-geometry.md#morse-smale-complex) and signs.

## 5

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The smooth [h-cobordism theorem](../../../geometry-and-topology.md#h-cobordism-theorem) states: if $(W;M_0,M_1)$ is a compact smooth [h-cobordism](../../../geometry-and-topology.md#h-cobordism), $\dim W\ge6$, and its connected boundary [manifolds](../../../topology.md#topological-manifold) are simply connected, then there is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $W\cong M_0\times[0,1]$ restricting to the prescribed identification on $M_0$. In particular $M_0$ and $M_1$ are [diffeomorphic](../../../geometry-and-topology.md#diffeomorphism). Being an [h-cobordism](../../../geometry-and-topology.md#h-cobordism) means that both inclusions $M_i\hookrightarrow W$ are [homotopy equivalences](../../../algebraic-topology.md#homotopy-equivalence); their fundamental groups then also identify with that of $W$.

The homotopy-equivalence condition is necessary for a [trivial cobordism](../../../geometry-and-topology.md#trivial-cobordism): each end of a cylinder is a deformation retract, by $(x,t)\mapsto(x,(1-s)t)$ for the incoming end and $(x,t)\mapsto(x,(1-s)t+s)$ for the outgoing end. Its [relative homology](../../../homology.md#relative-homology) with respect to either end is consequently zero. Compactness is also necessary for a product with a closed compact end. The dimensional bound and simple connectivity are not necessary for an individual [cobordism](../../../geometry-and-topology.md#cobordism) to be a product. The cylinder $S^2\times[0,1]$ is a simply connected [trivial cobordism](../../../geometry-and-topology.md#trivial-cobordism) of dimension three; and, in the theorem's dimension range, $(S^1\times S^4)\times[0,1]$ is a six-dimensional [trivial cobordism](../../../geometry-and-topology.md#trivial-cobordism) with [fundamental group](../../../algebraic-topology.md#fundamental-group) $\mathbb Z$. These prove the two non-necessity assertions explicitly, while the inclusion argument proves necessity of the h-condition.

For the remaining claims, use a [cobordism Morse function](../../../differential-geometry.md#cobordism-morse-function): its two regular boundary levels are zero and one, and all [critical points](../../../analysis.md#critical-point) are interior. An arbitrary function with unrelated boundary values would not have the relative handle-count property. The relative [Morse chain complex](../../../differential-geometry.md#morse-chain-complex) for $(W,M_0)$ has one generator per [critical point](../../../analysis.md#critical-point), in its [Morse index](../../../differential-geometry.md#morse-index). Thus

$$
\chi(W,M_0)=\sum_{r\in\operatorname{Crit}(f)}(-1)^{\operatorname{ind}(r)}.
$$

A [trivial cobordism](../../../geometry-and-topology.md#trivial-cobordism) has zero [relative homology](../../../homology.md#relative-homology), hence zero relative [Euler characteristic](../../../homology.md#euler-characteristic). Modulo two the displayed sum is the number of [critical points](../../../analysis.md#critical-point). An odd number makes it odd, and therefore nonzero. This proves **an odd-critical-point [cobordism](../../../geometry-and-topology.md#cobordism) is not trivial**.

With precisely two [critical points](../../../analysis.md#critical-point) of indices $\lambda\le\mu$, a [trivial cobordism](../../../geometry-and-topology.md#trivial-cobordism) requires the two-generator relative complex to be acyclic over $\mathbb Z$. Equal indices leave a rank-two [homology](../../../homology.md) group; a gap of more than one leaves both generators with zero possible differential. Therefore **$\mu=\lambda+1$ is necessary**. The remaining two-term complex is

$$
0\longrightarrow\mathbb Z q\xrightarrow{\times a}\mathbb Z p\longrightarrow0.
$$

Choose a transverse [gradient-like vector field](../../../differential-geometry.md#gradient-like-vector-field). A nonzero differential requires the index-$\mu$ point to be above the index-$\lambda$ point; otherwise no descending connecting trajectories exist. In a common regular level between them, the [belt sphere](../../../topology.md#belt-sphere) $S_U(p)$ has dimension $d-\lambda-1$, and the [attaching sphere](../../../topology.md#attaching-sphere) $S_L(q)$ has dimension $\mu-1=\lambda$, where $d=\dim W$. Their dimensions add to $d-1$, the level's dimension, so their transverse intersection consists of points. Each intersection is one descending trajectory from $q$ to $p$, modulo time translation. Orient the [attaching sphere](../../../topology.md#attaching-sphere) and use an [orientation of a vector space](../../../linear-algebra.md#orientation-of-a-vector-space) on the [handle](../../../topology.md#handle) core to coorient the [belt sphere](../../../topology.md#belt-sphere); the resulting signed count is the cellular boundary coefficient

$$
a=S_U(p)\cdot S_L(q).
$$

The two [homology](../../../homology.md) groups are the kernel and cokernel of multiplication by $a$. They vanish precisely when $a$ is a unit of $\mathbb Z$. Consequently

$$
\boxed{\mu=\lambda+1,\qquad S_U(p)\cdot S_L(q)=\pm1}
$$

are necessary. This proves the [two-critical-point obstruction to a trivial cobordism](../../../differential-geometry.md#two-critical-point-obstruction-to-a-trivial-cobordism); it makes an algebraic incidence statement and does not assume that an algebraic count of one automatically supplies geometric [handle](../../../topology.md#handle) cancellation.

For an explicit nontrivial [cobordism](../../../geometry-and-topology.md#cobordism) from $S^3$ to itself, attach two zero-framed [two-handles](../../../topology.md#two-handle) to the outgoing end of $S^3\times[0,1]$ along the standard [Hopf link](../../../knot-theory.md#hopf-link). Its two components are unknots with linking number one. This realizes two successive $(2,2)$ surgeries, as suggested by the hint. The outgoing boundary is again $S^3$, and this can be checked geometrically: the Hopf-link exterior is $T^2\times[0,1]$, and each component's zero-framing longitude is the other's meridian. Filling along these two slopes glues two solid [tori](../../../topology.md#torus) with meridians intersecting once, the standard genus-one Heegaard decomposition of $S^3$. Thus [zero surgery on the Hopf link](../../../knot-theory.md#zero-surgery-on-the-hopf-link) does return the three-sphere, not just an unspecified [homology](../../../homology.md) [sphere](../../../geometry-and-topology.md#sphere).

The trace has only the two added index-two [handles](../../../topology.md#handle). Its relative cellular complex has $C_2(W,S^3)=\mathbb Z^2$ and all other groups zero, so

$$
\boxed{H_2(W,S^3;\mathbb Z)=\mathbb Z^2\ne0.}
$$

It cannot be a product cylinder. Equivalently this trace is $S^2\times S^2$ with two disjoint open four-balls removed: the usual [handle](../../../topology.md#handle) presentation of $S^2\times S^2$ has one [zero-handle](../../../topology.md#zero-handle), the two zero-framed Hopf-linked [two-handles](../../../topology.md#two-handle), and one four-handle. Removing the bottom and top balls exposes the two three-sphere ends. The relative-homology calculation alone already proves **the requested [cobordism](../../../geometry-and-topology.md#cobordism) is nontrivial**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
