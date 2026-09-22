# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2003/PaperIB_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2003/PaperIB_2.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3H](#3h)
  - [Solution](#3h/solution)
- [4E](#4e)
  - [Solution](#4e/solution)
  - [i](#4e/i)
    - [Solution](#4e/i/solution)
  - [ii](#4e/ii)
    - [Solution](#4e/ii/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [Solution](#7b/a/solution)
  - [b](#7b/b)
    - [Solution](#7b/b/solution)
- [8G](#8g)
  - [Solution](#8g/solution)
- [9A](#9a)
  - [Solution](#9a/solution)
- [10F](#10f)
  - [Solution](#10f/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12H](#12h)
  - [Solution](#12h/solution)
- [13E](#13e)
  - [a](#13e/a)
    - [Solution](#13e/a/solution)
  - [b](#13e/b)
    - [Solution](#13e/b/solution)
- [14B](#14b)
  - [a](#14b/a)
    - [Solution](#14b/a/solution)
  - [b](#14b/b)
    - [Solution](#14b/b/solution)
- [15E](#15e)
  - [a](#15e/a)
    - [Solution](#15e/a/solution)
  - [b](#15e/b)
    - [Solution](#15e/b/solution)
  - [c](#15e/c)
    - [Solution](#15e/c/solution)
  - [d](#15e/d)
    - [Solution](#15e/d/solution)
- [16B](#16b)
  - [a](#16b/a)
    - [Solution](#16b/a/solution)
  - [b](#16b/b)
    - [Solution](#16b/b/solution)
  - [c](#16b/c)
    - [Solution](#16b/c/solution)
  - [d](#16b/d)
    - [Solution](#16b/d/solution)
- [17G](#17g)
  - [a](#17g/a)
    - [Solution](#17g/a/solution)
  - [b](#17g/b)
    - [Solution](#17g/b/solution)
  - [c](#17g/c)
    - [Solution](#17g/c/solution)
  - [d](#17g/d)
    - [Solution](#17g/d/solution)
- [18A](#18a)
  - [Solution](#18a/solution)

## 1F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

[Differentiability](../../../analysis.md#differentiability) at $(a,b)$ means that there is a [linear map](../../../vector-space.md#linear-map) $L:\mathbb R^2\to\mathbb R$ such that

$$
f(a+h,b+k)-f(a,b)=L(h,k)+o(\sqrt{h^2+k^2}).
$$

Necessarily $L(h,k)=f_x(a,b)h+f_y(a,b)k$ when those [partial derivatives](../../../calculus.md#partial-derivative) exist. Under the stated assumptions, apply the one-variable [mean value theorem](../../../calculus.md#mean-value-theorem) separately to the two coordinate increments:

$$
f(a+h,b+k)-f(a,b)=h f_x(a+\theta h,b+k)+k f_y(a,b+\eta k),
$$

for some intermediate $\theta,\eta\in(0,1)$, omitting a term if its increment is zero. Existence of the [partial derivatives](../../../calculus.md#partial-derivative) in a neighborhood supplies the differentiability along each segment required for that theorem. Their [continuity](../../../calculus.md#continuous-function) at $(a,b)$ makes the difference from $f_x(a,b)h+f_y(a,b)k$ bounded by $(|h|+|k|)\varepsilon(h,k)$, where $\varepsilon(h,k)\to0$. Since $|h|+|k|\le\sqrt2\sqrt{h^2+k^2}$, this is the required little-o remainder and proves [Fréchet differentiability](../../../calculus.md#frechet-differentiability).

For the particular function, $f(h,0)=f(0,k)=0$, so the defining difference quotients give **$f_x(0,0)=f_y(0,0)=0$**. However $f(t,t)=1/2$ for every $t\ne0$. It is not continuous at the origin, and therefore **not differentiable there**. This illustrates why existence of [partial derivatives](../../../calculus.md#partial-derivative) alone is insufficient.

## 2C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

Let $M_{ij}=\int_Sx_ix_j\,dS$. A [rotation matrix](../../../linear-algebra.md#rotation-matrix) $Q$ maps the unit sphere and its surface measure to themselves. Changing variables therefore gives $Q_{ip}Q_{jq}M_{pq}=M_{ij}$, so $M$ is an [isotropic second-rank tensor](../../../linear-algebra.md#isotropic-second-rank-tensor). Reflection symmetry also directly makes its off-diagonal entries zero, while interchange of coordinates makes its three diagonal entries equal. Its [trace](../../../linear-algebra.md#matrix-trace) is

$$
\sum_i M_{ii}=\int_S|x|^2\,dS=4\pi,
$$

hence $M_{ij}=(4\pi/3)\delta_{ij}$. Oddness gives $\int_Sx_i\,dS=0$. Expanding the defining product for $T$ now gives

$$
\boxed{T_{ij}(y)=\frac{4\pi}{3}\delta_{ij}+4\pi y_iy_j,
\qquad\lambda=\frac{4\pi}{3},\quad\mu=4\pi.}
$$

The action on a vector is $Tv=\lambda v+\mu y(y\cdot v)$. For $y\ne0$, its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and [eigenspaces](../../../linear-operator-theory.md#eigenspace) are therefore

$$
\boxed{\frac{4\pi}{3}+4\pi|y|^2\text{ on }\operatorname{span}\{y\},
\qquad\frac{4\pi}{3}\text{ on }y^\perp.}
$$

The latter has multiplicity two. If $y=0$, the single [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $4\pi/3$ has multiplicity three and every vector is an [eigenvector](../../../linear-operator-theory.md#eigenvector) apart from the excluded zero vector.

## 3H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3h/solution">Solution</h3>

↑ **Parent:** [3H](#3h)

Assume the known variances are positive and write $\bar x=n^{-1}\sum_ix_i$. The [likelihood](../../../statistical-modelling.md#likelihood-function) times the normal [prior distribution](../../../statistical-inference.md#prior-probability) is proportional to

$$
\exp\left\{-\frac12\left[\frac1{\sigma^2}\sum_i(x_i-\theta)^2+
\frac{(\theta-\mu)^2}{\tau^2}\right]\right\}.
$$

Collecting the quadratic and linear terms in $\theta$ completes the square with precision $v^{-1}=n/\sigma^2+1/\tau^2$ and mean $m=v(n\bar x/\sigma^2+\mu/\tau^2)$. Thus [normal-normal conjugacy](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance) gives

$$
\boxed{\theta\mid x_1,\ldots,x_n\sim N(m,v),\qquad
v=\frac{\sigma^2\tau^2}{\sigma^2+n\tau^2},\quad
m=\frac{n\tau^2\bar x+\sigma^2\mu}{\sigma^2+n\tau^2}.}
$$

For [quadratic loss](../../../statistical-inference.md#squared-error-loss), the posterior risk of reporting $a$ is $\mathbb E[(a-\theta)^2\mid x]=v+(a-m)^2$, uniquely minimized at $a=m$. For [absolute-error loss](../../../statistical-inference.md#absolute-error-loss), differentiating the posterior risk gives $2F_{\theta\mid x}(a)-1$, so its minimizer is a posterior median. The normal posterior is symmetric about $m$ and has a strictly increasing distribution function, hence that median is uniquely $m$. Therefore **both optimal point estimates equal $m$**, the [posterior mean](../../../statistical-inference.md#posterior-mean).

## 4E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4e/solution">Solution</h3>

↑ **Parent:** [4E](#4e)

For the [cofinite topology](../../../topology.md#cofinite-topology) $\tau_1$, the empty set and $\mathbb N$ are included. A nonempty union of cofinite sets is cofinite because its complement is contained in the finite complement of any one member. A finite intersection is cofinite because its complement is a finite union of finite sets; intersections involving the empty set are empty. This proves all [topology](../../../topology.md) axioms.

For the [tail topology on the natural numbers](../../../topology.md#tail-topology-on-the-natural-numbers) $\tau_2$, $\mathbb N=I_1$. Any nonempty collection of tails has a smallest starting index, so its union is that tail; a finite intersection of tails is the tail with largest starting index. Empty sets and empty-family conventions supply the remaining cases. Thus $\tau_2$ is also a [topology](../../../topology.md).

We classify [continuous maps between cofinite and tail topologies](../../../topology.md#continuous-maps-between-cofinite-and-tail-topologies). [Continuity](../../../calculus.md#continuous-function) is equivalent to

$$
E_k=\{n:f(n)\ge k\}\text{ being empty or cofinite for every }k.
$$

If $f$ has unbounded image, each $E_k$ is nonempty, hence cofinite. For every threshold $k$, eventually $f(n)\ge k$, which is exactly $f(n)\to\infty$. If the image is bounded, it is a nonempty finite subset of $\mathbb N$ and has a maximum $N$. Then $E_N$ is nonempty and cofinite, but $f(n)\le N$ always, so $f(n)=N$ except at finitely many indices. These exhaust the two possibilities and prove necessity. Their sufficiency is checked separately below.

<h3 id="4e/i">i</h3>

↑ **Parent:** [4E](#4e)

<h4 id="4e/i/solution">Solution</h4>

↑ **Parent:** [I](#4e/i)

If $f(n)\to\infty$, then for each $k$ the complement of $f^{-1}(I_k)$ contains only finitely many indices. Thus every nonempty open tail has a cofinite preimage, and the empty set has empty preimage. Hence **$f$ is continuous** from the cofinite space to the tail-[topology](../../../topology.md) space.

<h3 id="4e/ii">ii</h3>

↑ **Parent:** [4E](#4e)

<h4 id="4e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4e/ii)

Suppose $f(n)\le N$ for all $n$ and $f(n)=N$ eventually. If $k>N$, then $f^{-1}(I_k)=\varnothing$. If $k\le N$, the preimage contains all sufficiently large indices and is cofinite. Every open set therefore has open preimage, proving **$f$ is continuous**. Together with the introductory argument this proves the claimed if-and-only-if classification.

## 5B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

Eliminate the first entries of rows two, three and four using multipliers $a^3,a^2,a$. All remaining subdiagonal entries are then already zero. The unit-lower-triangular [LU decomposition](../../../numerical-analysis.md#lu-decomposition) is

$$
\boxed{L=\begin{pmatrix}1&0&0&0\\a^3&1&0&0\\a^2&0&1&0\\a&0&0&1\end{pmatrix},\quad
U=\begin{pmatrix}1&a&a^2&a^3\\0&\gamma&a\gamma&a^2\gamma\\0&0&\gamma&a\gamma\\0&0&0&\gamma\end{pmatrix}.}
$$

Multiplication verifies $LU=A$. Since $\gamma\ne0$, all pivots are nonzero. Forward substitution in $Ly=b$ gives

$$
y=(\gamma,-a^3\gamma,-a^2\gamma,0)^T.
$$

Backward substitution in $Ux=y$ gives $x_4=0$, $x_3=-a^2$, $x_2=0$, and $x_1=\gamma+a^4=1$. Thus

$$
\boxed{x=(1,0,-a^2,0)^T.}
$$

Direct substitution yields $Ax=(\gamma,0,0,a\gamma)^T$ as a check.

## 6E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

Associate to $c=(c_1,\ldots,c_n)^T$ the [polynomial](../../../polynomial.md) $p(t)=\sum_{j=1}^nc_jt^{j-1}$. The $i$th component of $Ac$ is exactly $p(a_i)$. If $Ac=0$, this [polynomial](../../../polynomial.md) of degree at most $n-1$ has $n$ distinct roots. Repeated use of the factor theorem would make $\prod_{i=1}^n(t-a_i)$ divide any nonzero such [polynomial](../../../polynomial.md), contradicting its degree. Hence $p$ is the zero [polynomial](../../../polynomial.md) and all $c_j=0$. The converse is immediate, proving **$\ker A=\{0\}$**.

A square [matrix](../../../vector-space.md#matrix) has full column [rank](../../../linear-algebra.md#rank-one-quadratic-form) if and only if its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is zero, by [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem). Its row [rank](../../../linear-algebra.md#rank-one-quadratic-form) equals its column [rank](../../../linear-algebra.md#rank-one-quadratic-form). Therefore this [Vandermonde matrix](../../../galois-theory.md#vandermonde-matrix) has row [rank](../../../linear-algebra.md#rank-one-quadratic-form) $n$, and its rows $v_1,\ldots,v_n$ are a [basis](../../../vector-space.md#basis) and **span $\mathbb R^n$**.

## 7B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/solution">Solution</h4>

↑ **Parent:** [A](#7b/a)

Take the unit circle counterclockwise and $n\ge0$. The integrand is a Laurent [polynomial](../../../polynomial.md) with its only possible singularity at zero. Its expansion is

$$
\frac1z(z-z^{-1})^{2n}
=\sum_{j=0}^{2n}(-1)^j\binom{2n}{j}z^{2n-2j-1}.
$$

The $z^{-1}$ term is the term $j=n$, so the [residue](../../../analysis.md#residue) is $(-1)^n\binom{2n}{n}$. The [residue theorem](../../../analysis.md#residue-theorem) gives

$$
\boxed{\oint_{|z|=1}(z-z^{-1})^{2n}\frac{dz}{z}
=2\pi i(-1)^n\frac{(2n)!}{(n!)^2}.}
$$

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/solution">Solution</h4>

↑ **Parent:** [B](#7b/b)

Parametrize the same contour by $z=e^{it}$, $0\le t\le2\pi$. Then $dz/z=i\,dt$ and $z-z^{-1}=2i\sin t$. Part a becomes

$$
i(-1)^n2^{2n}\int_0^{2\pi}\sin^{2n}t\,dt
=2\pi i(-1)^n\binom{2n}{n}.
$$

Canceling the nonzero common factors gives

$$
\boxed{\int_0^{2\pi}\sin^{2n}t\,dt
=\frac{2\pi}{2^{2n}}\binom{2n}{n}
=\frac{\pi(2n)!}{2^{2n-1}(n!)^2}.}
$$

## 8G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8g/solution">Solution</h3>

↑ **Parent:** [8G](#8g)

The positive-definite symmetric form $b$ is a real [inner product](../../../linear-algebra.md#inner-product). Choose a $b$-orthonormal [basis](../../../vector-space.md#basis) by the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process). The stated identity means that the [matrix](../../../vector-space.md#matrix) $K$ of $\psi$ satisfies $K^T=-K$. If $d=\dim U$, then

$$
\det K=\det K^T=\det(-K)=(-1)^d\det K.
$$

An invertible $K$ has nonzero [determinant](../../../linear-algebra.md#determinant), so **$d$ is even**.

To cover a possibly singular map, first show $\ker\psi=(\operatorname{im}\psi)^\perp$. If $x\in\ker\psi$, then $b(x,\psi y)=-b(\psi x,y)=0$ for every $y$, giving one inclusion. Conversely orthogonality to the image gives $b(\psi x,y)=0$ for all $y$, so nondegeneracy of $b$ gives $\psi x=0$. Positivity then implies $\operatorname{im}\psi\cap\ker\psi=\{0\}$.

The image is invariant under $\psi$, and its restricted map $\psi|_{\operatorname{im}\psi}$ is injective by that trivial intersection. In finite dimension it is consequently invertible. The restricted [inner product](../../../linear-algebra.md#inner-product) is positive definite and the same skew-adjoint identity holds, so the first argument applied to this restriction makes $\dim\operatorname{im}\psi$ even. Thus

$$
\boxed{\operatorname{rank}\psi\text{ is always even},}
$$

including [rank](../../../linear-algebra.md#rank-one-quadratic-form) zero. This is the [even rank of a skew-adjoint linear map](../../../functional-analysis.md#even-rank-of-a-skew-adjoint-linear-map).

## 9A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9a/solution">Solution</h3>

↑ **Parent:** [9A](#9a)

A [Hermitian operator](../../../hilbert-space.md#hermitian-operator) satisfies $\langle u,Av\rangle=\langle Au,v\rangle$ for all admissible states in its domain; in finite dimension this is $A^*=A$. For an unbounded physical observable one specifies a self-adjoint realization, rather than only a formal differential expression.

Here $p=-i\hbar\,d/dx$ and $H=-\hbar^2d^2/(2m\,dx^2)+V(x)$. For states with sufficient regularity and decay, integration by parts gives

$$
\langle u,Hv\rangle-\langle Hu,v\rangle
=-\frac{\hbar^2}{2m}[\bar u v'-\bar u'v]_{-\infty}^{\infty}=0.
$$

The multiplication term cancels because $V$ is real. Thus the [Quantum Hamiltonian](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) is Hermitian on the stated admissible domain. Equivalent boundary conditions must remove this boundary term if the system is on a bounded interval.

The [Schrödinger equation](../../../physics.md#schrodinger-equation) $i\hbar\dot\psi=H\psi$ and its conjugate imply, for a time-independent observable $A$ and normalized state,

$$
\frac d{dt}\langle A\rangle
=\frac i\hbar\langle HA-AH\rangle.
$$

This follows by differentiating both factors in $\langle\psi,A\psi\rangle$ and moving $H$ using Hermiticity. The canonical [commutator](../../../lie-algebra.md#commutator) $[x,p]=i\hbar$ gives

$$
[H,x]=-\frac{i\hbar}{m}p,\qquad [H,p]=[V,p]=i\hbar V'(x).
$$

Consequently the two [Ehrenfest theorem](../../../quantum-mechanics.md#ehrenfest-theorem) identities are

$$
\boxed{\frac d{dt}\langle x\rangle=\frac{\langle p\rangle}{m},\qquad
\frac d{dt}\langle p\rangle=-\langle V'(x)\rangle.}
$$

They require the displayed expectations and domain operations to exist; real-valuedness of a potential alone is not a proof about every possible singular operator domain.

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/solution">Solution</h3>

↑ **Parent:** [10F](#10f)

First $N(A)$ is finite: by [Cauchy-Schwarz](../../../probability-and-statistics.md#cauchy-schwarz-inequality), $\|Ax\|_2\le(\sum_{ij}a_{ij}^2)^{1/2}\|x\|_2$. It is nonnegative and absolutely homogeneous. If $N(A)=0$, every $Ae_j=0$, so every column is zero and $A=0$; the converse is immediate. The triangle inequality for the [Euclidean norm](../../../functional-analysis.md#euclidean-norm) gives $N(A+B)\le N(A)+N(B)$ after taking suprema. Thus **$N$ is a [norm](../../../functional-analysis.md#norm)**.

For any vector $x$, rescaling gives $\|Ax\|_2\le N(A)\|x\|_2$. Applying this twice gives

$$
\boxed{N(AB)\le N(A)N(B).}
$$

Furthermore $|a_{ij}|\le\|Ae_j\|_2\le N(A)$, proving the requested strict entry bound when $N(A)<\varepsilon$.

For a [polynomial](../../../polynomial.md) in [matrix](../../../vector-space.md#matrix) entries, expand each monomial at $A+H$. The terms involving exactly one entry of $H$ give a [linear map](../../../vector-space.md#linear-map) $Df(A)[H]$, with [coefficients](../../../vector-space.md#coefficient) [polynomial](../../../polynomial.md) in the entries of $A$. Every remaining term has at least two entries of $H$ and is $O(N(H)^2)$ for $N(H)\le1$, because $|h_{ij}|\le N(H)$. This proves differentiability. Its [derivative](../../../calculus.md#derivative) is continuous as an operator-valued function: each [coefficient](../../../vector-space.md#coefficient) is continuous, and for $N(H)\le1$ every $h_{ij}$ is bounded by one, so the operator-[norm](../../../functional-analysis.md#norm) difference is bounded by the sum of the [coefficient](../../../vector-space.md#coefficient) differences. Coordinate [continuity](../../../calculus.md#continuous-function) follows from the same entry bound. Hence **every such [polynomial](../../../polynomial.md) function is continuously differentiable**.

In the Leibniz expansion of $\det(I+H)$, the identity permutation supplies $1+\sum_i h_{ii}$ plus terms of degree at least two. Any nonidentity permutation moves at least two indices, so each of its terms has at least two $H$ entries. Consequently

$$
\det(I+H)=1+\operatorname{tr}H+O(N(H)^2),\qquad
\boxed{d'(I)[H]=\operatorname{tr}H.}
$$

If $A$ is invertible, multiplicativity of the [determinant](../../../linear-algebra.md#determinant) and the preceding expansion give

$$
\det(A+H)=\det A\det(I+A^{-1}H)
=\det A+\det A\operatorname{tr}(A^{-1}H)+O(N(H)^2).
$$

The adjugate identity gives $\operatorname{adj}A=\det(A)A^{-1}$. Thus $d'(A)[H]=\operatorname{tr}((\operatorname{adj}A)H)$ for invertible $A$.

For singular $A$, take invertible $A_r\to A$, using the permitted density result. Both $d'$ and the adjugate entries are continuous [polynomial](../../../polynomial.md) expressions, so taking limits for every fixed $H$ proves the [derivative of the determinant](../../../linear-algebra.md#derivative-of-the-determinant) formula on all [matrices](../../../vector-space.md#matrix):

$$
\boxed{d'(A)[H]=\operatorname{tr}((\operatorname{adj}A)H).}
$$

Here the standard adjugate is the transpose of the cofactor array, as required by $(\operatorname{adj}A)A=(\det A)I$. In components this [derivative](../../../calculus.md#derivative) is $\sum_{ij}\operatorname{cof}_{ij}(A)h_{ij}$, also valid at singular [matrices](../../../vector-space.md#matrix).

## 11C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

For an orthogonal change of Cartesian coordinates $x'_i=Q_{ij}x_j$, an ordinary [rank](../../../linear-algebra.md#rank-one-quadratic-form)-$n$ [tensor](../../../linear-algebra.md#tensor) transforms by

$$
\boxed{T'_{i_1\cdots i_n}=Q_{i_1j_1}\cdots Q_{i_nj_n}T_{j_1\cdots j_n}.}
$$

An [isotropic tensor](../../../linear-algebra.md#isotropic-tensor) is invariant under such rotations. Orthogonality gives $Q_{ip}Q_{jq}\delta_{pq}=\delta_{ij}$, so transforming any of the three products of two [Kronecker deltas](../../../linear-algebra.md#kronecker-delta) leaves it unchanged. Their linear combination with arbitrary scalar [coefficients](../../../vector-space.md#coefficient) is therefore isotropic.

For completeness, these three products exhaust the [rank](../../../linear-algebra.md#rank-one-quadratic-form)-four isotropic [tensors](../../../linear-algebra.md#tensor) in three dimensions. Half-turns about coordinate axes force a nonzero component to contain each coordinate label an even number of times. Axis interchanges then leave just the values $X=c_{1111}$, $\alpha=c_{1122}$, $\beta=c_{1212}$ and $\gamma=c_{1221}$. Rotating the first two axes by $\pi/4$ gives $X=\tfrac12X+\tfrac12(\alpha+\beta+\gamma)$, so $X=\alpha+\beta+\gamma$. These component values are exactly those of the three-delta-product expression. Thus isotropy of the elastic medium gives this form for its elasticity [tensor](../../../linear-algebra.md#tensor).

Contracting with the symmetric strain gives

$$
\sigma_{ij}=\alpha e_{kk}\delta_{ij}+\beta e_{ij}+\gamma e_{ji}
=\lambda e_{kk}\delta_{ij}+2\mu e_{ij},\qquad
\boxed{\lambda=\alpha,\quad2\mu=\beta+\gamma.}
$$

These are the [Lamé parameters](../../../continuum-mechanics.md#lame-parameter). Taking the [trace](../../../linear-algebra.md#matrix-trace) determines the scalar part of the strain:

$$
\boxed{p=\frac13e_{kk},\qquad d_{ij}=e_{ij}-p\delta_{ij},\qquad d_{ii}=0.}
$$

Since $\sum_{ij}e_{ij}^2=3p^2+\sum_{ij}d_{ij}^2$, the stored [strain energy density](../../../continuum-mechanics.md#strain-energy-density) is

$$
E=\frac\lambda2(e_{kk})^2+\mu e_{ij}e_{ij}
=\frac32(3\lambda+2\mu)p^2+\mu\sum_{ij}d_{ij}^2.
$$

A nonzero traceless test strain proves necessity of $\mu\ge0$, and a pure scalar strain proves necessity of $3\lambda+2\mu\ge0$. Conversely these two conditions make both terms nonnegative for every strain. Thus [nonnegative isotropic elastic strain energy](../../../continuum-mechanics.md#nonnegative-isotropic-elastic-strain-energy) is equivalent to

$$
\boxed{\mu\ge0,\qquad\lambda\ge-\frac23\mu.}
$$

## 12H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12h/solution">Solution</h3>

↑ **Parent:** [12H](#12h)

Model the two samples as independent multinomial counts with fixed row totals $N_A=N_B=500$ and three category probabilities. The null hypothesis is $p_{Aj}=p_{Bj}=p_j$ for every category $j$. Up to combinatorial factors the [likelihood](../../../statistical-modelling.md#likelihood-function) is $\prod_{ij}p_{ij}^{O_{ij}}$. Without the null restriction its maximizers are $O_{ij}/N_i$; under the null, maximizing $\sum_j(O_{Aj}+O_{Bj})\log p_j$ subject to $\sum_jp_j=1$ gives

$$
\widehat p_j=\frac{O_{Aj}+O_{Bj}}{1000},\qquad
E_{ij}=N_i\widehat p_j.
$$

The observed column totals are $243,281,476$, giving fitted expected counts **$(121.5,140.5,238)$ in each row**.

To derive the null distribution, put $D=O_A-O_B$. Under the null its mean is zero and covariance is $1000(\operatorname{diag}p-pp^T)$. The multivariate [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) gives, asymptotically, the standardized contrast $Z_j=D_j/\sqrt{1000p_j}$ a centered [normal distribution](../../../probability-theory.md#normal-distribution) with covariance

$$
I-uu^T,\qquad u=(\sqrt{p_1},\sqrt{p_2},\sqrt{p_3})^T,\quad u^Tu=1.
$$

This is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto a two-dimensional plane. In an orthonormal [basis](../../../vector-space.md#basis) of that plane, the two nonzero coordinates are independent standard normal variables, so $\sum_jZ_j^2$ tends to $\chi_2^2$. The pooled estimates are consistent; substituting them for $p_j$ leaves this limit unchanged by [Slutsky's theorem](../../../statistical-inference.md#slutsky-theorem). Since $O_{Aj}-E_{Aj}=D_j/2$ and $O_{Bj}-E_{Bj}=-D_j/2$, the resulting statistic is precisely the [Pearson chi-squared test of homogeneity](../../../statistical-modelling.md#pearson-chi-squared-test-of-homogeneity) statistic

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}}
=\sum_j\frac{D_j^2}{1000\widehat p_j},\qquad X^2\xrightarrow{d}\chi_2^2.
$$

This supplies the two degrees of freedom rather than treating all six cells as independent. Every fitted expected count is large, supporting the approximation.

For these data,

$$
\boxed{X^2=2\left(\frac{18.5^2}{121.5}+\frac{4.5^2}{140.5}
+\frac{14^2}{238}\right)=7.56906.}
$$

It exceeds the two-degree-of-freedom 95th percentile $5.99$, but not the 99th percentile $9.21$. Hence **reject equal score distributions at the 5% level, but not at the 1% level**. The asymptotic p-value is $\Pr(\chi_2^2\ge7.56906)=e^{-7.56906/2}\simeq0.02272$.

## 13E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13e/a">a</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/a/solution">Solution</h4>

↑ **Parent:** [A](#13e/a)

Define $F:[0,1]\to\mathbb C$ by $F(s)=se^{2\pi i/s}$ for $s>0$ and $F(0)=0$. It is continuous away from zero, and $|F(s)-F(0)|=s\to0$, so it is continuous at zero too. Its image is exactly $X\cup\{0\}$, using $s=1/t$. The interval is compact, so its continuous image is **compact**.

For any two image points $F(s_0),F(s_1)$, the explicit path

$$
\alpha(u)=F((1-u)s_0+us_1),\qquad0\le u\le1,
$$

is continuous and joins them. Thus the [reciprocal spiral with its endpoint](../../../geometry-and-topology.md#reciprocal-spiral-with-its-endpoint) is also **[path-connected](../../../geometry-and-topology.md#path-connected-space)**. Infinite winding causes no discontinuity at the endpoint because its radius tends to zero.

<h3 id="13e/b">b</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/b/solution">Solution</h4>

↑ **Parent:** [B](#13e/b)

The set $Y$ is [path-connected](../../../geometry-and-topology.md#path-connected-space) as the continuous image of $[1,\infty)$, hence connected. Its closure is $Y$ together with the unit circle. Indeed $g(k+\theta/(2\pi))\to e^{i\theta}$ as $k\to\infty$, and any convergent sequence of spiral points either has bounded parameters, giving a point of $Y$, or has parameters tending to infinity along a subsequence, giving radius one. The closure of a connected set is connected: a separation of its closure would induce a separation of the dense original set, with neither open part missing that set. The closed disk is connected and meets this closure in the unit circle; their union $Y\cup\overline D$ is therefore **connected**.

To show it is not [path-connected](../../../geometry-and-topology.md#path-connected-space), suppose a path $\alpha:[0,1]\to Y\cup\overline D$ starts in $Y$ and ends in the disk. Let $u_*$ be its first contact with the disk. The disk is closed, so this first contact exists, and $u_*>0$. Before it, the path belongs to $Y$ and has a continuous uniquely determined parameter

$$
t(u)=\frac1{|\alpha(u)|-1},\qquad\alpha(u)=g(t(u)).
$$

[Continuity](../../../calculus.md#continuous-function) at contact forces $|\alpha(u_*)|=1$, and hence $t(u)\to\infty$ as $u\uparrow u_*$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) supplies times approaching $u_*$ at which $t(u)$ is an integer, and other times at which it is an integer plus $1/2$. These times must approach contact because $t$ is bounded on every compact interval strictly before it. Along the first sequence $\alpha(u)\to1$; along the second it tends to $-1$. This contradicts [continuity](../../../calculus.md#continuous-function) at $u_*$. Thus **no path joins the spiral to the disk**, proving failure of path-[connectedness](../../../geometry-and-topology.md#connected-space) for the [spiral accumulating on a circle](../../../geometry-and-topology.md#spiral-accumulating-on-a-circle).

## 14B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14b/a">a</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/a/solution">Solution</h4>

↑ **Parent:** [A](#14b/a)

Exactness on the [polynomial](../../../polynomial.md) [basis](../../../vector-space.md#basis) $1,x,x^2$ requires

$$
a_0+a_1+a_2=0,\qquad-a_0+a_2=0,\qquad a_0+a_2=2.
$$

Solving gives

$$
\boxed{a_0=1,\qquad a_1=-2,\qquad a_2=1.}
$$

Thus the approximation is the unit-spacing centered second difference, $\mu(f)=f(-1)-2f(0)+f(1)$.

<h3 id="14b/b">b</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/b/solution">Solution</h4>

↑ **Parent:** [B](#14b/b)

The error $e(f)=f''(0)-f(-1)+2f(0)-f(1)$ is linear and annihilates all degree-at-most-two [polynomials](../../../polynomial.md). The [Peano kernel theorem](../../../numerical-analysis.md#peano-kernel-theorem) with [derivative](../../../calculus.md#derivative) order three gives

$$
e(f)=\int_{-1}^1K(t)f'''(t)\,dt,\qquad
K(t)=e_x\left(\frac{(x-t)_+^2}{2}\right).
$$

For $t\ne0$, the second [derivative](../../../calculus.md#derivative) of the truncated quadratic at $x=0$ is $\mathbf1_{\{t<0\}}$. Its values at $x=-1,0,1$ then give

$$
K(t)=\mathbf1_{\{t<0\}}+(-t)_+^2-\frac{(1-t)^2}{2}
=\begin{cases}\tfrac12(1+t)^2,&-1<t<0,\\-\tfrac12(1-t)^2,&0<t<1.\end{cases}
$$

The value at the single point $t=0$ is irrelevant to the integral. This is the [centered second-derivative Peano kernel](../../../numerical-analysis.md#centered-second-derivative-peano-kernel). Its absolute integral is

$$
\int_{-1}^1|K(t)|\,dt
=\frac12\int_{-1}^0(1+t)^2dt+\frac12\int_0^1(1-t)^2dt
=\frac13.
$$

Consequently

$$
\boxed{|e(f)|\le\frac13\|f'''\|_{C[-1,1]}.}
$$

Its changing sign explains why cubic [polynomials](../../../polynomial.md) also have zero error: their third [derivative](../../../calculus.md#derivative) is constant and $\int_{-1}^1K=0$. No fourth [derivative](../../../calculus.md#derivative) is needed for the claimed bound.

## 15E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15e/a">a</h3>

↑ **Parent:** [15E](#15e)

<h4 id="15e/a/solution">Solution</h4>

↑ **Parent:** [A](#15e/a)

By the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem), $\operatorname{nullity}A=n-\operatorname{rank}A\ge n-m>0$. Thus a first dependent column prefix exists. Minimality of $k$ makes the first $k-1$ columns independent, so $\operatorname{rank}A_{k-1}=k-1$. Adding one column cannot reduce this [rank](../../../linear-algebra.md#rank-one-quadratic-form), while nonzero [nullity](../../../linear-algebra.md#nullity-of-a-linear-map) of $A_k$ implies [rank](../../../linear-algebra.md#rank-one-quadratic-form) at most $k-1$. Hence

$$
\operatorname{rank}A_k=k-1,\qquad
\boxed{\operatorname{nullity}A_k=1.}
$$

For $k=1$ the earlier prefix is the zero-dimensional empty [matrix](../../../vector-space.md#matrix), and the same argument applies.

<h3 id="15e/b">b</h3>

↑ **Parent:** [15E](#15e)

<h4 id="15e/b/solution">Solution</h4>

↑ **Parent:** [B](#15e/b)

Choose any nonzero vector $b$ in the one-dimensional [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of $A_k$. It gives $\sum_{j=1}^ka_{ij}b_j=0$ for every row. Because no column is zero, $b$ must have at least two nonzero entries: a relation supported at a single index would make that column zero.

Suppose, contrary to the claim, that $A_k\operatorname{diag}(\lambda_1,\ldots,\lambda_k)b=0$. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is spanned by $b$, so there is a scalar $c$ with $\lambda_jb_j=cb_j$ for every $j$. At the two nonzero entries this gives two equal weights $\lambda_j=c$, contradicting their distinctness. Thus **the weighted sum is nonzero in at least one row**. This proves that [distinct diagonal weights break a first column dependence](../../../vector-space.md#distinct-diagonal-weights-break-a-first-column-dependence). Some entries of $b$ may be zero; only two nonzero entries are needed.

<h3 id="15e/c">c</h3>

↑ **Parent:** [15E](#15e)

<h4 id="15e/c/solution">Solution</h4>

↑ **Parent:** [C](#15e/c)

Assume for contradiction that $n>m$. Apply part b to the [matrix](../../../vector-space.md#matrix) of the given relation [coefficients](../../../vector-space.md#coefficient), whose columns are nonzero. For its first dependent prefix choose $b_1,\ldots,b_k$ with

$$
\sum_{j=1}^ka_{ij}b_j=0\quad\text{for all }i,
\qquad z_i:=\sum_{j=1}^ka_{ij}\lambda_jb_j\text{ not all zero}.
$$

Multiply the $j$th given vector relation by $b_j$ and sum. Interchanging the finite sums gives

$$
0=\sum_{i=1}^m\left(\sum_{j=1}^ka_{ij}b_j\right)v_i
+\sum_{i=1}^m\left(\sum_{j=1}^ka_{ij}\lambda_jb_j\right)w_i
=\sum_{i=1}^mz_iw_i.
$$

The $w_i$ are a [basis](../../../vector-space.md#basis), so all $z_i$ must be zero, contradicting part b. Therefore **$n\le m$**.

<h3 id="15e/d">d</h3>

↑ **Parent:** [15E](#15e)

<h4 id="15e/d/solution">Solution</h4>

↑ **Parent:** [D](#15e/d)

Choose a fixed reference [basis](../../../vector-space.md#basis) and let $V,W$ have columns $v_i,w_i$. Both [matrices](../../../vector-space.md#matrix) are invertible. The vectors $v_i+\lambda w_i$ are dependent exactly when $\det(V+\lambda W)=0$. This is a [polynomial](../../../polynomial.md) in $\lambda$ of degree $m$, whose leading [coefficient](../../../vector-space.md#coefficient) is $\det W\ne0$. A nonzero degree-$m$ [polynomial](../../../polynomial.md) has at most $m$ distinct real roots. Thus **there are at most $m$ exceptional parameters**. This is the [determinant](../../../linear-algebra.md#determinant) argument for the [matrix pencil](../../../vector-space.md#matrix-pencil) $V+\lambda W$.

## 16B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16b/a">a</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/a/solution">Solution</h4>

↑ **Parent:** [A](#16b/a)

Use $\widehat f(\lambda)=(2\pi)^{-1/2}\int_{\mathbb R}e^{-i\lambda x}f(x)\,dx$. The transform statement requires sufficient decay and regularity for the transform and its [derivatives](../../../calculus.md#derivative); functions in the [Schwartz space](../../../fourier-analysis.md#schwartz-space) suffice, and all the functions constructed below belong to that space. Integration by parts twice and differentiation under the integral give

$$
\widehat{f''}=-\lambda^2\widehat f,\qquad
\widehat{x^2f}=-\widehat f''.
$$

Transforming the differential equation therefore gives

$$
\boxed{\widehat f''(\lambda)-\lambda^2\widehat f(\lambda)=\mu\widehat f(\lambda).}
$$

The differential equation by itself does not ensure that an ordinary [Fourier transform](../../../analysis.md#fourier-transform) exists: $f=e^{x^2/2}$ solves it with $\mu=1$ but grows too rapidly. Thus the usual transformability assumptions are implicit in this part.

<h3 id="16b/b">b</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/b/solution">Solution</h4>

↑ **Parent:** [B](#16b/b)

Set $f=p(x)e^{-x^2/2}$. Differentiating gives

$$
f''-x^2f=[p''-2xp'-p]e^{-x^2/2}.
$$

Thus the [polynomial](../../../polynomial.md) must satisfy $p''-2xp'-(\mu+1)p=0$. If it has degree $n$ and nonzero leading [coefficient](../../../vector-space.md#coefficient), comparison of highest powers gives $\mu=-(2n+1)$. For this value the equation becomes the [Hermite differential equation](../../../analysis.md#hermite-differential-equation)

$$
p''-2xp'+2np=0.
$$

Write $p=\sum_{j=0}^na_jx^j$, with [coefficients](../../../vector-space.md#coefficient) beyond $n$ zero. Comparing powers yields

$$
(j+2)(j+1)a_{j+2}+2(n-j)a_j=0.
$$

The equation at $j=n-1$ forces $a_{n-1}=0$, and downward recurrence removes all terms of the opposite parity and determines all same-parity terms from $a_n$. Taking $a_n=1$ produces the explicit [polynomial](../../../polynomial.md)

$$
p_n(x)=\sum_{r=0}^{\lfloor n/2\rfloor}
\frac{(-1)^r n!}{4^r r!(n-2r)!}x^{n-2r}.
$$

It satisfies every [coefficient](../../../vector-space.md#coefficient) equation, so existence as well as uniqueness up to a nonzero scalar is proved. Hence

$$
\boxed{\mu_n=-(2n+1),\qquad f_n=p_ne^{-x^2/2}.}
$$

The monic $p_n$ is $2^{-n}$ times the usual physicists' [Hermite polynomial](../../../numerical-analysis.md#hermite-polynomial).

<h3 id="16b/c">c</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/c/solution">Solution</h4>

↑ **Parent:** [C](#16b/c)

Multiplication by $x$ transforms to $i\,d/d\lambda$. Write $p_n(x)=\sum_{j=0}^na_jx^j$ and use $\widehat g=cg$ for the Gaussian $g=e^{-x^2/2}$. Then

$$
\widehat{f_n}(\lambda)=c\sum_{j=0}^na_ji^j\frac{d^j}{d\lambda^j}e^{-\lambda^2/2}
=q_n(\lambda)e^{-\lambda^2/2}.
$$

Successive differentiation of the Gaussian gives a [polynomial](../../../polynomial.md) of degree $j$ with leading term $(-1)^j\lambda^j$ multiplying that same Gaussian. Thus $q_n$ has leading [coefficient](../../../vector-space.md#coefficient) $ca_n(-i)^n\ne0$. This proves **$q_n$ is a [polynomial](../../../polynomial.md) of degree exactly $n$**, rather than merely at most $n$.

<h3 id="16b/d">d</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/d/solution">Solution</h4>

↑ **Parent:** [D](#16b/d)

By part a the transformed function solves the same equation with $\mu_n$, and by part c its [polynomial](../../../polynomial.md) factor has degree $n$. The uniqueness proved in part b therefore gives $q_n=c_np_n$. Comparing their leading [coefficients](../../../vector-space.md#coefficient) gives

$$
\boxed{\widehat{f_n}=c(-i)^nf_n.}
$$

For the unitary convention used above, the Gaussian integral gives $c=1$, so **$c_n=(-i)^n$**. With the unnormalized phase-$e^{-i\lambda x}$ convention, $c=\sqrt{2\pi}$ instead. This proves that [Hermite functions are Fourier eigenfunctions](../../../numerical-analysis.md#hermite-functions-are-fourier-eigenfunctions), with the normalization-dependent scalar fully specified.

## 17G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17g/a">a</h3>

↑ **Parent:** [17G](#17g)

<h4 id="17g/a/solution">Solution</h4>

↑ **Parent:** [A](#17g/a)

A Hermitian two-by-two [matrix](../../../vector-space.md#matrix) has the form

$$
A=\begin{pmatrix}\alpha&z\\\bar z&\delta\end{pmatrix},\qquad
\alpha,\delta\in\mathbb R,\quad z\in\mathbb C.
$$

Addition and real scalar multiplication preserve this condition, and the two diagonal entries plus the real and imaginary parts of $z$ give four independent real coordinates. Thus **$S$ is a real four-dimensional vector space**. The [trace](../../../linear-algebra.md#matrix-trace) product is real because $\overline{\operatorname{tr}(AB)}=\operatorname{tr}(BA)=\operatorname{tr}(AB)$; this also proves symmetry of $b$.

Directly, $\operatorname{tr}(A^2)=\alpha^2+\delta^2+2|z|^2$ and $(\operatorname{tr}A)^2=\alpha^2+2\alpha\delta+\delta^2$. Hence

$$
\boxed{b(A,A)=|z|^2-\alpha\delta=-\det A.}
$$

Since $\operatorname{tr}I=2$ and $\operatorname{tr}(AI)=\operatorname{tr}A$,

$$
\boxed{b(A,I)=-\frac12\operatorname{tr}A.}
$$

<h3 id="17g/b">b</h3>

↑ **Parent:** [17G](#17g)

<h4 id="17g/b/solution">Solution</h4>

↑ **Parent:** [B](#17g/b)

The displayed [matrices](../../../vector-space.md#matrix) are the three [Pauli matrices](../../../algebra.md#pauli-matrices), in the order $\sigma_3,\sigma_1,\sigma_2$. They satisfy $\operatorname{tr}A_i=0$ and $\operatorname{tr}(A_iA_j)=2\delta_{ij}$. Every [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) has a unique expression $aI+\sum_iv_iA_i$ with all four [coefficients](../../../vector-space.md#coefficient) real. Therefore they form a [basis](../../../vector-space.md#basis) together with $I$.

The preceding [trace](../../../linear-algebra.md#matrix-trace) identities give $b(I,I)=-1$, $b(I,A_i)=0$, and $b(A_i,A_j)=\delta_{ij}$. The Gram [matrix](../../../vector-space.md#matrix) is thus

$$
\boxed{\operatorname{diag}(-1,1,1,1).}
$$

Consequently **[rank](../../../linear-algebra.md#rank-one-quadratic-form) $=4$ and inertia signature $(3,1)$**. If signature is defined as the number of positive squares minus the number of negative squares, its value is $2$. This is the [Hermitian matrix representation of Minkowski four-vectors](../../../special-relativity.md#hermitian-matrix-representation-of-minkowski-four-vectors), with the negative-[determinant](../../../linear-algebra.md#determinant) sign convention.

<h3 id="17g/c">c</h3>

↑ **Parent:** [17G](#17g)

<h4 id="17g/c/solution">Solution</h4>

↑ **Parent:** [C](#17g/c)

Taking [traces](../../../linear-algebra.md#matrix-trace) in the defining equation gives $\operatorname{tr}C+\overline{\operatorname{tr}C}=2\operatorname{tr}C$, so the [trace](../../../linear-algebra.md#matrix-trace) is real. Put $a=\operatorname{tr}C/2$. Then $K=C-aI$ is traceless and satisfies $K^*=-K$, so $-iK$ is a traceless [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). Hence every element has a unique representation

$$
C=aI+i\sum_jv_jA_j,\qquad a,v_j\in\mathbb R.
$$

Conversely each such [matrix](../../../vector-space.md#matrix) satisfies the defining equation. This proves **$Q$ is a real four-dimensional vector space**, with [basis](../../../vector-space.md#basis) $I,iA_1,iA_2,iA_3$.

Substitution into the given map gives

$$
\boxed{\Phi\left(aI+i\sum_jv_jA_j\right)=aI-\sum_jv_jA_j.}
$$

Its values are Hermitian, and it acts on real coordinates by $(a,v_1,v_2,v_3)\mapsto(a,-v_1,-v_2,-v_3)$. This invertible real linear coordinate transformation proves the required isomorphism. The inverse sends $aI+\sum_ju_jA_j$ to $aI-i\sum_ju_jA_j$.

<h3 id="17g/d">d</h3>

↑ **Parent:** [17G](#17g)

<h4 id="17g/d/solution">Solution</h4>

↑ **Parent:** [D](#17g/d)

Let $r=\operatorname{tr}C$, $s=\operatorname{tr}D$, and $\beta=(1-i)/2$. Their [traces](../../../linear-algebra.md#matrix-trace) are real by part c, and $\Phi(C)=\beta rI+iC$. Thus $\operatorname{tr}\Phi(C)=(2\beta+i)r=r$. Expanding the product and using $2\beta^2+2i\beta=1$ gives

$$
\operatorname{tr}(\Phi(C)\Phi(D))=rs-\operatorname{tr}(CD).
$$

Therefore

$$
\boxed{b(\Phi(C),\Phi(D))
=\frac12[rs-\operatorname{tr}(CD)-rs]
=-\frac12\operatorname{tr}(CD)=c(C,D).}
$$

In particular the [trace](../../../linear-algebra.md#matrix-trace) expression is real and symmetric on $Q$. Under the coordinates $C=aI+i\mathbf v\cdot\mathbf A$, $D=dI+i\mathbf w\cdot\mathbf A$, it is $-ad+\mathbf v\cdot\mathbf w$. Thus the [trace form on scalar-plus-skew-Hermitian two-by-two matrices](../../../special-relativity.md#trace-form-on-scalar-plus-skew-hermitian-two-by-two-matrices) has **[rank](../../../linear-algebra.md#rank-one-quadratic-form) $4$, inertia $(3,1)$**, or numerical signature $2$, agreeing with $b$ under the real isomorphism.

## 18A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18a/solution">Solution</h3>

↑ **Parent:** [18A](#18a)

Take fixed $E>0$ and define $k=\sqrt{2mE}/\hbar$. For sufficiently large $V_0$, the barrier region has $\kappa=\sqrt{2m(V_0-E)}/\hbar$ and solves $\psi''=\kappa^2\psi$. Solving this constant-[coefficient](../../../vector-space.md#coefficient) equation gives the exact transfer relation

$$
\begin{pmatrix}\psi(a)\\\psi'(a)\end{pmatrix}
=\begin{pmatrix}\cosh(\kappa a)&\sinh(\kappa a)/\kappa\\
\kappa\sinh(\kappa a)&\cosh(\kappa a)\end{pmatrix}
\begin{pmatrix}\psi(0)\\\psi'(0)\end{pmatrix}.
$$

In the specified limit, $a=U/V_0$ and $\kappa a\to0$, while

$$
\kappa^2a\to\frac{2mU}{\hbar^2}=:\eta.
$$

The transfer [matrix](../../../vector-space.md#matrix) therefore tends to $\begin{pmatrix}1&0\\\eta&1\end{pmatrix}$. As the two boundaries collapse to the origin, this proves [continuity](../../../calculus.md#continuous-function) and the [derivative](../../../calculus.md#derivative) jump for a [delta potential](../../../quantum-mechanics.md#delta-potential):

$$
\psi(0+)=\psi(0-),\qquad
\psi'(0+)-\psi'(0-)=\eta\psi(0).
$$

The vanishing exterior phase shift $e^{ika}\to1$ introduces no further factor.

Write the incoming and reflected waves as $e^{ikx}+r e^{-ikx}$ on the left and the transmitted wave as $t e^{ikx}$ on the right. Matching gives

$$
t=1+r,\qquad ikt-ik(1-r)=\eta t,
\qquad t=\frac{2ik}{2ik-\eta}=\frac1{1+i\eta/(2k)}.
$$

The denominator is nonzero for real $\eta$ and $k>0$, so the limiting matching system is well defined. The [probability currents](../../../quantum-mechanics.md#probability-current) on either side have the same factor $\hbar k/m$, making the transmission probability $|t|^2$. Thus [scattering by a delta potential](../../../quantum-mechanics.md#scattering-by-a-delta-potential) gives

$$
\boxed{T=\frac1{1+\eta^2/(4k^2)}
=\left(1+\frac{mU^2}{2E\hbar^2}\right)^{-1}.}
$$

The limit retains a finite reflection probability despite the barrier's vanishing width because its integrated strength remains finite.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
