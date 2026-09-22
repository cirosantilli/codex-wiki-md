# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2016/paperia_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2016/paperia_1.pdf)

**Table of contents**

- [1A](#1a)
  - [i](#1a/i)
    - [Solution](#1a/i/solution)
  - [ii](#1a/ii)
    - [Solution](#1a/ii/solution)
  - [iii](#1a/iii)
    - [Solution](#1a/iii/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3D](#3d)
  - [Solution](#3d/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5A](#5a)
  - [a](#5a/a)
    - [Solution](#5a/a/solution)
  - [b](#5a/b)
    - [Solution](#5a/b/solution)
  - [c](#5a/c)
    - [Solution](#5a/c/solution)
- [6B](#6b)
  - [Solution](#6b/solution)
- [7B](#7b)
  - [Solution](#7b/solution)
- [8C](#8c)
  - [a](#8c/a)
    - [Solution](#8c/a/solution)
  - [b](#8c/b)
    - [Solution](#8c/b/solution)
- [9E](#9e)
  - [Solution](#9e/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11D](#11d)
  - [a](#11d/a)
    - [Solution](#11d/a/solution)
  - [b](#11d/b)
    - [Solution](#11d/b/solution)
- [12F](#12f)
  - [Solution](#12f/solution)

## 1A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1a/i">i</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/i/solution">Solution</h4>

↑ **Parent:** [I](#1a/i)

The [quadratic formula](../../../polynomial.md#quadratic-formula) gives

$$
z=-\frac b2\pm\frac i2\sqrt{4-b^2},
$$

so both [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) have [real part](../../../complex-analysis.md#real-part) $-b/2$. Writing $z=x+iy$, the [complex exponential function](../../../calculus.md#complex-exponential-function) satisfies $e^z=e^x(\cos y+i\sin y)$, and hence its [modulus](../../../complex-analysis.md#modulus) is $e^x$. Therefore

$$
|e^z|=e^{-b/2}<1
\quad\Longleftrightarrow\quad b>0.
$$

Intersecting this condition with the allowed parameter interval gives the answer **for either root**:

$$
\boxed{0<b\le2.}
$$

The endpoint $b=2$ is included: the repeated [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) is $z=-1$, whose exponential has [modulus](../../../complex-analysis.md#modulus) $e^{-1}<1$.

<h3 id="1a/ii">ii</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1a/ii)

Write the [complex number](../../../complex-analysis.md#complex-number) as $z=x+iy$. Since $iz=-y+ix$, the [modulus of the complex exponential](../../../calculus.md#modulus-of-the-complex-exponential) gives

$$
|e^{iz}|=e^{-y}.
$$

This equals one precisely when $y=0$. The [quadratic formula](../../../polynomial.md#quadratic-formula) shows that the [imaginary part](../../../complex-analysis.md#imaginary-part) of either root is $\pm\sqrt{4-b^2}/2$. Consequently the roots are real exactly at the two endpoints:

$$
\boxed{b=-2\ \text{or}\ b=2.}
$$

**Both endpoints satisfy the condition.** The repeated roots are respectively $1$ and $-1$; their multiples by $i$ have exponentials on the [unit circle](../../../complex-analysis.md#complex-unit-circle).

<h3 id="1a/iii">iii</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1a/iii)

Using the exponential definition of the [hyperbolic cosine](../../../calculus.md#hyperbolic-cosine) and the [complex exponential function](../../../calculus.md#complex-exponential-function),

$$
\cosh(x+iy)=\cosh x\cos y+i\sinh x\sin y.
$$

Thus

$$
\operatorname{Im}(\cosh z)=\sinh x\,\sin y,
\qquad x=-\frac b2,\qquad y=\pm\frac{\sqrt{4-b^2}}2.
$$

For real $x$, the [hyperbolic sine](../../../calculus.md#hyperbolic-sine) vanishes only at $x=0$. Also $|y|\le1<\pi$, so the only zero of [sine](../../../geometry-and-topology.md#sine) available to $y$ is $y=0$. The product therefore vanishes exactly when $b=0$ or $4-b^2=0$:

$$
\boxed{b\in\{-2,0,2\}.}
$$

**There are three possible parameter values.** At $b=0$ the roots are $\pm i$ and $\cosh(\pm i)=\cos1$ is real; at $b=\pm2$ the roots themselves are real.

## 2C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

A counterclockwise planar [rotation matrix](../../../linear-algebra.md#rotation-matrix) has the form

$$
R_\theta=
\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix},
\qquad\theta\in\mathbb R.
$$

To recover this form from preservation of the [Euclidean norm](../../../functional-analysis.md#euclidean-norm), let $\mathbf u,\mathbf v$ be the columns of $R$. Applying the norm condition to the two coordinate [unit vectors](../../../vector-space.md#unit-vector) gives $|\mathbf u|=|\mathbf v|=1$. Applying it to their sum gives

$$
2=|\mathbf u+\mathbf v|^2
=|\mathbf u|^2+2\mathbf u\cdot\mathbf v+|\mathbf v|^2,
$$

so $\mathbf u\cdot\mathbf v=0$. The columns are an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), and $R^TR=I$: $R$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix).

Write $\mathbf u=(\cos\theta,\sin\theta)^T$. There are two perpendicular [unit vectors](../../../vector-space.md#unit-vector) available for $\mathbf v$, namely $\pm(-\sin\theta,\cos\theta)^T$. The first gives [determinant](../../../linear-algebra.md#determinant) $1$, the second $-1$. The positive determinant hypothesis selects the first. **A norm-preserving planar map with positive determinant is a rotation.**

For the commutation condition, write

$$
A=\begin{pmatrix}a&b\\c&d\end{pmatrix}.
$$

Direct [matrix multiplication](../../../vector-space.md#matrix-multiplication) gives

$$
AJ=\begin{pmatrix}b&-a\\d&-c\end{pmatrix},
\qquad
JA=\begin{pmatrix}-c&-d\\a&b\end{pmatrix}.
$$

Equality forces $c=-b$ and $d=a$, so, with $u=a$ and $v=-b$,

$$
A=\begin{pmatrix}u&-v\\v&u\end{pmatrix}=uI+vJ.
$$

If $u=v=0$, take $\lambda=0$ and $R=I$. Otherwise set $\lambda=\sqrt{u^2+v^2}>0$ and choose $\cos\theta=u/\lambda$, $\sin\theta=v/\lambda$. Then

$$
\boxed{A=\lambda R_\theta,\qquad\lambda=\sqrt{u^2+v^2}.}
$$

This describes the [centralizer of a planar quarter-turn](../../../linear-algebra.md#centralizer-of-a-planar-quarter-turn). Its nonzero elements act as a rotation followed by a uniform scaling, just as multiplication by a nonzero [complex number](../../../complex-analysis.md#complex-number) does.

## 3D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3d/solution">Solution</h3>

↑ **Parent:** [3D](#3d)

A [sequence](../../../real-analysis.md#sequence) $(x_n)$ is a [convergent sequence](../../../real-analysis.md#convergent-sequence) with limit $x$ if

$$
\forall\varepsilon>0\ \exists N\in\mathbb N\
\forall n\ge N:\quad |x_n-x|<\varepsilon.
$$

The index $N$ may depend on $\varepsilon$, but must work for every later term.

Fix $\varepsilon>0$. Choose $N$ such that $|x_i-x|<\varepsilon/2$ for $i\ge N$, and put

$$
C=\sum_{i=1}^{N-1}|x_i-x|.
$$

This is a fixed finite number. For $n\ge N$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\left|\frac1n\sum_{i=1}^nx_i-x\right|
\le\frac1n\sum_{i=1}^n|x_i-x|
\le\frac Cn+\frac{n-N+1}{n}\frac{\varepsilon}{2}
\le\frac Cn+\frac{\varepsilon}{2}.
$$

Choose $n$ sufficiently large that $C/n<\varepsilon/2$ as well. The error is then less than $\varepsilon$, proving

$$
\boxed{\frac1n\sum_{i=1}^nx_i\longrightarrow x.}
$$

**Taking successive arithmetic averages preserves the limit.** This is the [Cesaro theorem for convergent sequences](../../../real-analysis.md#cesaro-theorem-for-convergent-sequences): any troublesome initial terms contribute only a fixed numerator divided by $n$.

## 4F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

Every counted point has [integer](../../../number-theory.md#integer) coordinates and lies in the square $[-n,n]^2$, while the origin is always counted. Hence

$$
1\le a_n\le(2n+1)^2.
$$

No precise circle-area estimate is needed; this elementary bound controls the growth of the [power series](../../../real-analysis.md#power-series) coefficients.

The [comparison test for series](../../../real-analysis.md#comparison-test-for-series) states that if $0\le u_n\le v_n$, convergence of $\sum v_n$ implies convergence of $\sum u_n$. Equivalently, divergence of the smaller nonnegative series forces divergence of the larger one.

For $|z|=r<1$,

$$
\sum_{n=0}^\infty|a_nz^n|
\le\sum_{n=0}^\infty(2n+1)^2r^n.
$$

For $0<r<1$, the ratio of successive terms on the right tends to $r<1$, so the [ratio test](../../../real-analysis.md#ratio-test) and the [comparison test for series](../../../real-analysis.md#comparison-test-for-series) show [absolute convergence](../../../real-analysis.md#absolute-convergence). The case $r=0$ is immediate.

If $|z|\ge1$, then $|a_nz^n|\ge1$, so the terms do not tend to zero. The [term test for divergence](../../../real-analysis.md#term-test-for-divergence) therefore rules out convergence, including every point on the boundary $|z|=1$. Thus the [radius of convergence](../../../real-analysis.md#radius-of-convergence) is

$$
\boxed{R=1.}
$$

**The series converges exactly in the open unit disc.** This is an example of [polynomial coefficient growth with unit power-series radius](../../../real-analysis.md#polynomial-coefficient-growth-with-unit-power-series-radius): the lattice-count bound is polynomial rather than exponential.

## 5A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5a/a">a</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/a/solution">Solution</h4>

↑ **Parent:** [A](#5a/a)

Use [suffix notation](../../../linear-algebra.md#einstein-notation) with indices ranging from $1$ to $3$, and sum over repeated indices. By the component definitions of the [dot product](../../../linear-algebra.md#dot-product) and [cross product](../../../vector-space.md#cross-product),

$$
\mathbf a\cdot(\mathbf b\times\mathbf c)
=a_i\epsilon_{ijk}b_jc_k.
$$

The [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) is unchanged by a cyclic permutation of its three indices: the cycle is two transpositions and hence has positive sign. Thus $\epsilon_{ijk}=\epsilon_{kij}$. Commuting the scalar components gives

$$
a_i\epsilon_{ijk}b_jc_k
=c_k\epsilon_{kij}a_ib_j
=c_k(\mathbf a\times\mathbf b)_k.
$$

Therefore the [scalar triple product](../../../linear-algebra.md#scalar-triple-product) obeys

$$
\boxed{\mathbf a\cdot(\mathbf b\times\mathbf c)
=\mathbf c\cdot(\mathbf a\times\mathbf b).}
$$

**Cyclically moving the vectors preserves the scalar triple product; interchanging just two reverses its sign.**

<h3 id="5a/b">b</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/b/solution">Solution</h4>

↑ **Parent:** [B](#5a/b)

The two displacement [vectors](../../../vector-space.md#vector) $\mathbf b-\mathbf a$ and $\mathbf c-\mathbf a$ lie in the required [plane](../../../geometry-and-topology.md#plane). Because the three points are non-collinear, their [cross product](../../../vector-space.md#cross-product)

$$
\mathbf N=(\mathbf b-\mathbf a)\times(\mathbf c-\mathbf a)
$$

is nonzero and is a [normal vector](../../../differential-geometry.md#normal-vector) to that plane. A point with position vector $\mathbf r$ lies in the plane exactly when

$$
(\mathbf r-\mathbf a)\cdot\mathbf N=0.
$$

Expanding the [cross product](../../../vector-space.md#cross-product) gives

$$
\mathbf N=\mathbf a\times\mathbf b+\mathbf b\times\mathbf c+\mathbf c\times\mathbf a.
$$

The terms $\mathbf a\cdot(\mathbf a\times\mathbf b)$ and $\mathbf a\cdot(\mathbf c\times\mathbf a)$ vanish, so the [equation of a plane through three points](../../../geometry-and-topology.md#equation-of-a-plane-through-three-points) becomes

$$
\boxed{\mathbf r\cdot
(\mathbf a\times\mathbf b+\mathbf b\times\mathbf c+\mathbf c\times\mathbf a)
=\mathbf a\cdot(\mathbf b\times\mathbf c).}
$$

Non-collinearity is important: it ensures this is a genuine plane equation with nonzero normal, rather than the vacuous equality $0=0$.

For the specified coordinates,

$$
\mathbf a\times\mathbf b=(-4,0,8),\qquad
\mathbf b\times\mathbf c=(8,0,-4),\qquad
\mathbf c\times\mathbf a=(-1,3,2).
$$

Their sum is $(3,3,6)$, with [Euclidean norm](../../../functional-analysis.md#euclidean-norm) $3\sqrt6$. Consequently either orientation of the [unit normal](../../../differential-geometry.md#unit-normal) is valid:

$$
\boxed{\mathbf n=\pm\frac{(1,1,2)}{\sqrt6}.}
$$

As a check, the [scalar triple product](../../../linear-algebra.md#scalar-triple-product) is $12$, so the plane equation simplifies to $x+y+2z=4$, which all three supplied points satisfy. **The normal direction is $(1,1,2)$.**

<h3 id="5a/c">c</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/c/solution">Solution</h4>

↑ **Parent:** [C](#5a/c)

The chosen [unit normal](../../../differential-geometry.md#unit-normal) points toward the plane from the origin, so the plane equation is

$$
\boxed{\mathbf n\cdot\mathbf r=d.}
$$

To locate the circle centre, project $\mathbf p$ onto this [plane](../../../geometry-and-topology.md#plane). Put

$$
\gamma=d-\mathbf n\cdot\mathbf p,\qquad
\mathbf h=\mathbf p+\gamma\mathbf n.
$$

Then $\mathbf n\cdot\mathbf h=d$, so $\mathbf h$ lies in the plane. For any other point $\mathbf r$ of the plane, $\mathbf r-\mathbf h$ is perpendicular to $\mathbf n$. The [Pythagorean theorem](../../../geometry-and-topology.md#pythagorean-theorem) therefore gives

$$
|\mathbf r-\mathbf p|^2
=|\mathbf r-\mathbf h|^2+\gamma^2.
$$

Restricting the sphere equation to the plane consequently gives a circle centred at $\mathbf h$. Thus $\mathbf m=\mathbf h$, proving that the displacement of its centre is purely normal:

$$
\boxed{\mathbf m-\mathbf p=\gamma\mathbf n,\qquad
\gamma=d-\mathbf n\cdot\mathbf p.}
$$

The same [Pythagorean theorem](../../../geometry-and-topology.md#pythagorean-theorem) gives $q^2=\rho^2+\gamma^2$, and hence

$$
\boxed{\gamma^2=q^2-\rho^2,\qquad
\gamma=\pm\sqrt{q^2-\rho^2}.}
$$

**The sign of $\gamma$ is fixed by which side of the plane contains $\mathbf p$; $q$ and $\rho$ alone determine only its magnitude.** Substituting the signed offset yields the [sphere-plane intersection](../../../geometry-and-topology.md#sphere-plane-intersection) radius

$$
\boxed{\rho=\sqrt{q^2-(d-\mathbf n\cdot\mathbf p)^2}.}
$$

A genuine circle requires $|d-\mathbf n\cdot\mathbf p|<q$; equality gives tangency and $\rho=0$, while a larger distance gives no intersection. The [signed distance from a point to a plane](../../../geometry-and-topology.md#signed-distance-from-a-point-to-a-plane) in the direction $\mathbf n$ is $\mathbf n\cdot\mathbf p-d=-\gamma$; the ordinary [distance from a point to a plane](../../../geometry-and-topology.md#distance-from-a-point-to-a-plane) is its absolute value.

## 6B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6b/solution">Solution</h3>

↑ **Parent:** [6B](#6b)

For the reality of the [eigenvalues](../../../linear-operator-theory.md#eigenvalue), one may initially allow a nonzero complex [eigenvector](../../../linear-operator-theory.md#eigenvector) $\mathbf v$ with $M\mathbf v=\lambda\mathbf v$. Since $M$ is real symmetric, it is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator), and

$$
\lambda=\frac{\mathbf v^\dagger M\mathbf v}{\mathbf v^\dagger\mathbf v}
$$

is real: the numerator equals its own complex conjugate and the denominator is positive. Once $\lambda$ is real, a nonzero real or imaginary part of $\mathbf v$ supplies a real eigenvector. We work with the real unit eigenvectors of the problem.

For two such [eigenvectors](../../../linear-operator-theory.md#eigenvector), symmetry gives

$$
\lambda_a\,\mathbf e_a\cdot\mathbf e_b
=(M\mathbf e_a)\cdot\mathbf e_b
=\mathbf e_a\cdot(M\mathbf e_b)
=\lambda_b\,\mathbf e_a\cdot\mathbf e_b.
$$

Distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) therefore give zero [dot product](../../../linear-algebra.md#dot-product). Together with the prescribed unit lengths,

$$
\boxed{\mathbf e_a\cdot\mathbf e_b=\delta_{ab}.}
$$

These $n$ vectors form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $\mathbb R^n$.

Expand a real [unit vector](../../../vector-space.md#unit-vector) as $\mathbf x=\sum_ac_a\mathbf e_a$. Then $\sum_ac_a^2=1$, and its [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) is

$$
\mathbf x^TM\mathbf x=\sum_a\lambda_ac_a^2\le\lambda_1.
$$

Moreover,

$$
\lambda_1-\mathbf x^TM\mathbf x
=\sum_{a=2}^n(\lambda_1-\lambda_a)c_a^2.
$$

Every coefficient on the right is strictly positive, so equality forces $c_a=0$ for $a\ge2$. **Equality occurs precisely along the top eigendirection**:

$$
\boxed{\mathbf x^TM\mathbf x\le\lambda_1,\qquad
\mathbf x^TM\mathbf x=\lambda_1\iff\mathbf x=\pm\mathbf e_1.}
$$

To obtain a unit vector in $S$ using just $\mathbf e_1,\mathbf e_2$, let $u=(\mathbf e_1)_1$ and $v=(\mathbf e_2)_1$ denote their first coordinates. If $u^2+v^2>0$, take

$$
\alpha_1=\frac v{\sqrt{u^2+v^2}},\qquad
\alpha_2=-\frac u{\sqrt{u^2+v^2}}.
$$

Then $\alpha_1u+\alpha_2v=0$ and $\alpha_1^2+\alpha_2^2=1$. Hence $\alpha_1\mathbf e_1+\alpha_2\mathbf e_2$ has first coordinate zero and unit length. If $u=v=0$, simply take $\alpha_1=1,\alpha_2=0$. In either case the [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) of the constructed vector is

$$
\lambda_1\alpha_1^2+\lambda_2\alpha_2^2\ge\lambda_2.
$$

The continuous quadratic form attains its maximum on the [compact space](../../../topology.md#compact-space) $S$, so

$$
\max_{\mathbf x\in S}\mathbf x^TM\mathbf x\ge\lambda_2.
$$

For $\mathbf x=(0,\mathbf y)^T$, deletion of the first row and column gives $\mathbf x^TM\mathbf x=\mathbf y^TA\mathbf y$, while $|\mathbf x|=|\mathbf y|$. The [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) applied to $A$ identifies its largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) with this maximum:

$$
\mu=\max_{|\mathbf y|=1}\mathbf y^TA\mathbf y
=\max_{\mathbf x\in S}\mathbf x^TM\mathbf x.
$$

Combining the upper bound for every unit vector with the constructed lower bound proves

$$
\boxed{\lambda_1\ge\mu\ge\lambda_2.}
$$

This is [largest-eigenvalue interlacing for a principal submatrix](../../../linear-operator-theory.md#largest-eigenvalue-interlacing-for-a-principal-submatrix): restricting a quadratic form to a coordinate hyperplane cannot exceed its old maximum, but leaves some direction in the span of the top two eigenvectors.

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/solution">Solution</h3>

↑ **Parent:** [7B](#7b)

A [matrix](../../../vector-space.md#matrix) is a [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) if there is an invertible matrix $P$ for which $P^{-1}MP$ is diagonal. Its columns then form a [basis](../../../vector-space.md#basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector), and the diagonal entries are their corresponding [eigenvalues](../../../linear-operator-theory.md#eigenvalue).

Here the given eigenvectors form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). Put them into the columns of $Q$:

$$
Q=(\mathbf e_1\ \cdots\ \mathbf e_n),\qquad Q^TQ=I,\qquad Q^{-1}=Q^T.
$$

Define $\Lambda=Q^TMQ$. Its entries are

$$
\Lambda_{ab}=\mathbf e_a^TM\mathbf e_b
=\lambda_b\,\mathbf e_a\cdot\mathbf e_b
=\lambda_b\delta_{ab}.
$$

This proves the claimed [diagonalization of a matrix](../../../linear-operator-theory.md#diagonalization-of-a-matrix), rather than merely guessing it:

$$
\boxed{\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_n),\qquad
M=Q\Lambda Q^T.}
$$

The [trace](../../../linear-algebra.md#matrix-trace) follows directly from this factorization:

$$
\operatorname{tr}M
=\sum_i\sum_a\lambda_aQ_{ia}^2
=\sum_a\lambda_a\sum_iQ_{ia}^2
=\sum_a\lambda_a,
$$

because each column of $Q$ has unit length. **Trace is the sum of the eigenvalues, with multiplicity.**

For the particular matrix, $(M^2)_{ij}=\sum_kM_{ik}M_{kj}$. If $i=j$, every $k\ne i$ contributes one and $k=i$ contributes zero. If $i\ne j$, precisely $k=i$ and $k=j$ contribute zero; the other $n-2$ terms contribute one. Thus

$$
(M^2)_{ij}=
\begin{cases}
n-1,&i=j,\\
n-2,&i\ne j,
\end{cases}
\qquad
M^2=(n-1)I+(n-2)M.
$$

Applying this identity to a nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector) gives

$$
\lambda^2=(n-1)+(n-2)\lambda,
\qquad
(\lambda-(n-1))(\lambda+1)=0.
$$

Every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is therefore $n-1$ or $-1$.

If $r$ is the multiplicity of $n-1$, the [trace](../../../linear-algebra.md#matrix-trace) formula for a [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) and the zero diagonal give

$$
0=r(n-1)+(n-r)(-1)=n(r-1),
$$

so $r=1$. Up to ordering, the required diagonal form is

$$
\boxed{\Lambda=\operatorname{diag}(n-1,-1,\ldots,-1).}
$$

For $n=1$ this means just $(0)$. For $n\ge2$, the eigendirections are also transparent: the all-ones vector has eigenvalue $n-1$, and the $(n-1)$-dimensional subspace whose coordinate sum is zero has eigenvalue $-1$, since $(M\mathbf x)_i=\sum_jx_j-x_i$. **The spectrum consists of one collective mode and $n-1$ zero-sum modes.**

## 8C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8c/a">a</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/a/solution">Solution</h4>

↑ **Parent:** [A](#8c/a)

Adding the three equations for $s,t$ gives the necessary [solvability condition](../../../linear-operator-theory.md#solvability-condition) $a+b+c=3$. Conversely, subtraction of the first two and use of the third force

$$
s=\frac{a-b}{2},\qquad t=\frac{1-c}{2}.
$$

If $a+b+c=3$, these values also satisfy the first two equations: for example,

$$
1+s+t=\frac{3+a-b-c}{2}=a.
$$

The analogous calculation gives $1-s+t=b$. Thus existence and uniqueness hold exactly under the stated compatibility condition:

$$
\boxed{a+b+c=3,\qquad s=\frac{a-b}{2},\quad t=\frac{1-c}{2}.}
$$

For the three-variable system the [matrix](../../../vector-space.md#matrix) and data vector are

$$
A=\begin{pmatrix}5&2&-1\\2&5&-1\\-1&-1&8\end{pmatrix},
\qquad
\mathbf x=\begin{pmatrix}x\\y\\z\end{pmatrix},
\qquad
\mathbf b=\begin{pmatrix}1+s+t\\1-s+t\\1-2t\end{pmatrix},
\qquad A\mathbf x=\mathbf b.
$$

Perform [Gaussian elimination](../../../numerical-analysis.md#gaussian-elimination) on the augmented matrix. The operations $R_2\leftarrow5R_2-2R_1$ and $R_3\leftarrow5R_3+R_1$ give

$$
\left[
\begin{array}{ccc|c}
5&2&-1&1+s+t\\
0&21&-3&3-7s+3t\\
0&-3&39&6+s-9t
\end{array}
\right].
$$

Each operation is an invertible row scaling followed by a row addition, so the solution set is preserved. Next $R_3\leftarrow7R_3+R_2$ gives

$$
\left[
\begin{array}{ccc|c}
5&2&-1&1+s+t\\
0&21&-3&3-7s+3t\\
0&0&270&45-60t
\end{array}
\right].
$$

Back substitution now yields

$$
z=\frac16-\frac{2t}{9},\qquad
y=\frac{3-7s+3t+3z}{21}
=\frac16-\frac s3+\frac t9,
$$

and then

$$
\boxed{x=\frac16+\frac s3+\frac t9,\qquad
y=\frac16-\frac s3+\frac t9,\qquad
z=\frac16-\frac{2t}{9}.}
$$

All three pivots are nonzero. Thus **the solution exists uniquely for every $s,t$**, the [matrix rank](../../../vector-space.md#matrix-rank) is $3$, and the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) represented by $A$ is $\{\mathbf0\}$. The general [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) for a matrix with $m$ columns is

$$
\boxed{\operatorname{rank}A+\dim\ker A=m;}
$$

here $m=3$.

Finally, reverse the viewpoint and regard $x,y,z$ as prescribed. The necessary and sufficient condition already proved applies with $a=5x+2y-z$, $b=2x+5y-z$, $c=-x-y+8z$. Their sum is $6(x+y+z)$. Consequently $s,t$ can be recovered exactly when

$$
\boxed{x+y+z=\frac12.}
$$

When this holds, their unique values are $s=\tfrac32(x-y)$ and $t=\tfrac12(1+x+y-8z)$. **The allowable triples form an affine plane, not all of $\mathbb R^3$.**

<h3 id="8c/b">b</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/b/solution">Solution</h4>

↑ **Parent:** [B](#8c/b)

A complex square [matrix](../../../vector-space.md#matrix) $U$ is a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) when $U^\dagger U=I$, equivalently $U^{-1}=U^\dagger$. Here $\dagger$ denotes the [adjoint matrix](../../../linear-operator-theory.md#conjugate-transpose), the conjugate transpose. Such a matrix preserves the standard complex [inner product](../../../linear-algebra.md#inner-product) and its [Euclidean norm](../../../functional-analysis.md#euclidean-norm).

A real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $A$ is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator), so $A^\dagger=A$. For arbitrary complex $\mathbf x$,

$$
\begin{aligned}
|(A+iI)\mathbf x|^2
&=\mathbf x^\dagger(A-iI)(A+iI)\mathbf x\\
&=\mathbf x^\dagger(A^2+I)\mathbf x\\
&=|A\mathbf x|^2+|\mathbf x|^2.
\end{aligned}
$$

The imaginary cross terms cancel because $A$ is Hermitian. Reversing the signs gives the same identity:

$$
\boxed{|(A-iI)\mathbf x|^2=|(A+iI)\mathbf x|^2
=|A\mathbf x|^2+|\mathbf x|^2.}
$$

In particular, $(A+iI)\mathbf x=0$ implies $|\mathbf x|^2=0$, so $A+iI$ has zero [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map). It is a square matrix, and the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) therefore makes it invertible. The same argument proves invertibility of $A-iI$.

The proposed matrix

$$
U=(A-iI)(A+iI)^{-1}
$$

is consequently well-defined. For any $\mathbf y$, put $\mathbf x=(A+iI)^{-1}\mathbf y$. The two norm identities show directly that

$$
|U\mathbf y|=|(A-iI)\mathbf x|
=|(A+iI)\mathbf x|=|\mathbf y|.
$$

To verify the [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) identity explicitly, take adjoints:

$$
U^\dagger=(A-iI)^{-1}(A+iI).
$$

The two shifts commute, because both are polynomials in $A$. Hence

$$
\begin{aligned}
U^\dagger U
&=(A-iI)^{-1}(A+iI)(A-iI)(A+iI)^{-1}\\
&=(A-iI)^{-1}(A-iI)(A+iI)(A+iI)^{-1}=I.
\end{aligned}
$$

Thus

$$
\boxed{(A-iI)(A+iI)^{-1}\ \text{is unitary}.}
$$

**The imaginary shifts are invertible, and their equal norm changes cancel in the quotient.** This is the [Cayley transform of a Hermitian matrix](../../../linear-operator-theory.md#cayley-transform-of-a-hermitian-matrix) in the $(A-iI)(A+iI)^{-1}$ convention.

## 9E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9e/solution">Solution</h3>

↑ **Parent:** [9E](#9e)

The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) states that every [bounded sequence](../../../real-analysis.md#bounded-sequence) of real numbers has a [convergent subsequence](../../../real-analysis.md#convergent-subsequence). We first use it to show that a [continuous function](../../../calculus.md#continuous-function) on $[a,b]$ is bounded above. Otherwise, choose $x_n\in[a,b]$ with $f(x_n)>n$. A convergent subsequence $x_{n_k}\to c$ exists, with $c\in[a,b]$ because the interval is closed. [Continuity](../../../calculus.md#continuous-function) would give $f(x_{n_k})\to f(c)$, contradicting $f(x_{n_k})>n_k\to\infty$.

Let $L=\sup\{f(x):x\in[a,b]\}$, which is finite. By the definition of [supremum](../../../real-analysis.md#supremum), there are $y_n\in[a,b]$ with $L-1/n<f(y_n)\le L$. Another application of the [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) gives a subsequence $y_{n_k}\to c\in[a,b]$. By [continuity](../../../calculus.md#continuous-function),

$$
f(c)=\lim_{k\to\infty}f(y_{n_k})=L.
$$

Thus **the supremum is actually attained**:

$$
\boxed{\exists c\in[a,b]\ \forall x\in[a,b]:\ f(x)\le f(c).}
$$

This proves the maximum part of the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) from sequential compactness rather than assuming it.

Now suppose $f''<0$ on $\mathbb R$. Applying the [mean value theorem](../../../calculus.md#mean-value-theorem) to $f'$ shows that $f'$ is strictly decreasing. At a [local maximum](../../../analysis.md#local-maximum) of a [differentiable function](../../../analysis.md#differentiable-function), the left difference quotients are nonnegative and the right difference quotients are nonpositive; existence of the derivative forces $f'=0$. A strictly decreasing function has at most one zero. Therefore

$$
\boxed{f''<0\ \Longrightarrow\ \text{at most one local maximum}.}
$$

If that zero exists, $f'$ is positive to its left and negative to its right, so the local maximum is also a [global maximum](../../../function.md#global-maximum).

For the uniform bound by $K<0$, define

$$
h(x)=f'(x)-Kx.
$$

Its derivative is $h'(x)=f''(x)-K<0$, so $h$ is strictly decreasing by the [mean value theorem](../../../calculus.md#mean-value-theorem). Comparing with $h(0)=f'(0)$ gives

$$
\begin{cases}
f'(x)<f'(0)+Kx,&x>0,\\
f'(x)>f'(0)+Kx,&x<0.
\end{cases}
$$

Because $K<0$, this makes $f'$ negative at sufficiently large positive $x$ and positive at sufficiently large negative $x$. The function $f'$ is continuous, since it is differentiable; the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) supplies a zero $c$ between such points. Its strict decrease makes this zero unique. Again using the [mean value theorem](../../../calculus.md#mean-value-theorem) for $f$, the derivative signs imply that $f$ increases up to $c$ and decreases after $c$:

$$
\boxed{f''(x)<K<0\ \text{for all }x
\ \Longrightarrow\ f\text{ has a unique global maximum}.}
$$

This illustrates [uniform negative curvature and global maximization](../../../real-analysis.md#uniform-negative-curvature-and-global-maximization).

Merely requiring $f''<0$ does not force existence. Take

$$
f(x)=-e^{-x}.
$$

Then $f'(x)=e^{-x}>0$ and $f''(x)=-e^{-x}<0$, but $f$ is strictly increasing, approaches $0$ as $x\to+\infty$, and never equals $0$. **The answer to the final question is no**, even for a function bounded above:

$$
\boxed{\sup_{\mathbb R}(-e^{-x})=0\quad\text{and the supremum is not attained}.}
$$

The stronger uniform curvature assumption prevents this behaviour. Here $f''(x)\to0$ at the end where the supremum is approached, so no uniform negative bound of that kind is available.

## 10E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

The [Rolle theorem](../../../calculus.md#rolle-theorem) states that if a real function is continuous on $[u,v]$, differentiable on $(u,v)$, and has equal endpoint values, then its derivative vanishes somewhere in $(u,v)$. Order the $k$ distinct real roots as $r_1<\cdots<r_k$. The theorem gives a root of $f'$ in each interval $(r_j,r_{j+1})$. These intervals are disjoint, so the obtained roots are distinct:

$$
\boxed{f'\text{ has at least }k-1\text{ distinct real roots}.}
$$

We prove the requested bound for [positive roots of a polynomial](../../../polynomial.md#positive-root-of-a-polynomial) by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on the number of nonzero terms. In fact, the proof also works with roots counted according to their [multiplicity](../../../polynomial.md#multiplicity-mathematics). Write $V(p)$ for the number of sign changes and $N_+(p)$ for the positive-root count.

A one-term polynomial $a_1x^{d_1}$ has no positive roots and no sign changes. For the induction step, factor out the smallest power of $x$:

$$
q(x)=x^{-d_1}p(x)
=a_1+\sum_{j=2}^na_jx^{e_j},
\qquad e_j=d_j-d_1>0.
$$

For $x>0$ this factor is nonzero, so $N_+(q)=N_+(p)$, including multiplicities, and $V(q)=V(p)$. Differentiation removes exactly the constant term:

$$
q'(x)=\sum_{j=2}^ne_ja_jx^{e_j-1}.
$$

The exponents remain strictly increasing, and the positive multipliers $e_j$ do not change coefficient signs. The induction hypothesis therefore gives

$$
N_+(q')\le V(q'),\qquad
V(q')=V(a_2,\ldots,a_n).
$$

First suppose $a_1a_2<0$. Removing $a_1$ removes exactly one sign change, so $V(q)=V(q')+1$. If $q$ has positive roots $r_1<\cdots<r_k$ of multiplicities $m_1,\ldots,m_k$, its derivative has multiplicity $m_j-1$ at $r_j$ and, by the [Rolle theorem](../../../calculus.md#rolle-theorem), an additional root between each pair. Thus the [Rolle root count with multiplicities](../../../calculus.md#rolle-root-count-with-multiplicities) gives

$$
N_+(q')\ge\sum_{j=1}^k(m_j-1)+(k-1)=N_+(q)-1
$$

when there is a positive root. Consequently

$$
N_+(q)\le N_+(q')+1\le V(q')+1=V(q).
$$

If there is no positive root, the desired bound is automatic.

Now suppose $a_1a_2>0$, so $V(q)=V(q')$. Again the zero-root case is immediate. Otherwise, multiplying $q$ by $-1$ if necessary lets us assume $a_1>0$ and $a_2>0$ without changing roots or sign changes. For sufficiently small $x>0$,

$$
q(x)>0,\qquad q'(x)>0,
$$

since $q(0)=a_1$ and the lowest-power term of $q'$ has positive coefficient. Choose such a point $u$ before the first positive root $r_1$. The [mean value theorem](../../../calculus.md#mean-value-theorem) on $[u,r_1]$ gives a point $v\in(u,r_1)$ with

$$
q'(v)=\frac{q(r_1)-q(u)}{r_1-u}<0.
$$

But $q'(u)>0$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) applied to the polynomial $q'$ therefore gives an extra root in $(u,v)$, before $r_1$. It is distinct from the roots at $r_j$ and those between consecutive roots. Hence

$$
N_+(q')\ge N_+(q),
\qquad
N_+(q)\le N_+(q')\le V(q')=V(q).
$$

Both sign cases complete the induction:

$$
\boxed{N_+(p)\le V(p).}
$$

**An initial sign change allows one extra positive root; without that sign change, the derivative must already turn before the first positive root.** This is the upper-bound part of the [Descartes' rule of signs](../../../polynomial.md#descartes-rule-of-signs). The multiplicity claim used above follows by differentiating $q(x)=(x-r)^mh(x)$ with $h(r)\ne0$: the derivative has a factor $(x-r)^{m-1}$ and its remaining factor is nonzero at $r$.

## 11D

↑ **Parent:** [Paper 1](paper-1.md)

The two preliminary [sequence](../../../real-analysis.md#sequence) limit laws follow directly from the [triangle inequality](../../../topological-analysis.md#triangle-inequality). For the sum, choose indices so that $|x_n-x|<\varepsilon/2$ and $|y_n-y|<\varepsilon/2$ beyond their respective cutoffs. Beyond the larger cutoff,

$$
|(x_n+y_n)-(x+y)|
\le|x_n-x|+|y_n-y|<\varepsilon.
$$

Thus

$$
\boxed{x_n+y_n\longrightarrow x+y.}
$$

For the reciprocal, convergence to nonzero $x$ gives $|x_n-x|<|x|/2$ eventually. The reverse [triangle inequality](../../../topological-analysis.md#triangle-inequality) then gives $|x_n|\ge|x|/2$, and consequently

$$
\left|\frac1{x_n}-\frac1x\right|
=\frac{|x_n-x|}{|x_n|\,|x|}
\le\frac{2|x_n-x|}{|x|^2}.
$$

Choosing the eventual error smaller than both $|x|/2$ and $\varepsilon|x|^2/2$ proves

$$
\boxed{\frac1{x_n}\longrightarrow\frac1x.}
$$

**The nonzero limit gives the denominator a positive lower bound; nonzero individual terms alone would not do so.** The assumption $x_n\ne0$ ensures the reciprocal sequence is defined even before this eventual bound applies.

<h3 id="11d/a">a</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/a/solution">Solution</h4>

↑ **Parent:** [A](#11d/a)

Use [rationalization of a square-root difference](../../../algebra.md#rationalization-of-a-square-root-difference) to avoid subtracting two large, nearly equal quantities:

$$
\sqrt{n^2+n}-n
=\frac{n}{\sqrt{n^2+n}+n}
=\frac1{\sqrt{1+1/n}+1}.
$$

Since $1/n\to0$ and the [square root](../../../algebra.md#square-root) is continuous at $1$, the denominator tends to $2$. The reciprocal limit law established above is applicable because this limit is nonzero. Hence

$$
\boxed{\lim_{n\to\infty}\bigl(\sqrt{n^2+n}-n\bigr)=\frac12.}
$$

**The limit is one half; rationalization exposes the finite difference hidden by cancellation.**

<h3 id="11d/b">b</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/b/solution">Solution</h4>

↑ **Parent:** [B](#11d/b)

Rationalize the numerator of the summand:

$$
\frac{\sqrt{n+1}-\sqrt n}{\sqrt n}
=\frac1{\sqrt n\,(\sqrt{n+1}+\sqrt n)}
=\frac1{n(\sqrt{1+1/n}+1)}.
$$

For every $n\ge1$ we have $\sqrt{1+1/n}\le\sqrt2$, and therefore

$$
\frac{\sqrt{n+1}-\sqrt n}{\sqrt n}
\ge\frac1{(\sqrt2+1)n}>0.
$$

The [harmonic series](../../../real-analysis.md#harmonic-series) diverges, so the [comparison test for series](../../../real-analysis.md#comparison-test-for-series) makes the given positive-term series diverge as well:

$$
\boxed{\sum_{n=1}^\infty
\frac{\sqrt{n+1}-\sqrt n}{\sqrt n}=+\infty.}
$$

For completeness, divergence of the [harmonic series](../../../real-analysis.md#harmonic-series) follows by grouping the terms with $2^k<n\le2^{k+1}$: each such block contributes at least $2^k/2^{k+1}=1/2$. The same rationalization also shows that $n$ times the summand tends to $1/2$. **The summands tend to zero, but their harmonic-size tail prevents convergence.**

## 12F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12f/solution">Solution</h3>

↑ **Parent:** [12F](#12f)

The stated bound is [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) with constant $1$. For every $x$ and every $\varepsilon>0$, taking $\delta=\varepsilon$ ensures $|f(x)-f(y)|<\varepsilon$ whenever $|x-y|<\delta$. The same $\delta$ works at every point, so $f$ is both continuous and [uniformly continuous](../../../topological-analysis.md#uniform-continuity).

For an integer $N\ge1$, partition $[0,1]$ into $N$ equal intervals and define a [step function](../../../measure-theory.md#step-function)

$$
g_N(x)=f(j/N)\quad\text{for }\frac jN\le x<\frac{j+1}{N},
\qquad j=0,\ldots,N-1.
$$

At the remaining endpoint set $g_N(1)=f((N-1)/N)$, so the final interval may be taken closed on the right. The [Lipschitz bound](../../../real-analysis.md#lipschitz-bound) gives

$$
|f(x)-g_N(x)|\le\frac1N
\quad\text{for all }x\in[0,1].
$$

Choosing $N\ge1/\varepsilon$ proves the requested [uniform step approximation on a compact interval](../../../uniform-approximation.md#uniform-step-approximation-on-a-compact-interval):

$$
\boxed{\sup_{x\in[0,1]}|f(x)-g_N(x)|\le\frac1N\le\varepsilon.}
$$

**A sufficiently fine partition gives a piecewise constant approximation uniformly over the whole interval.**

The [continuous function](../../../calculus.md#continuous-function) $f$ and every finite [step function](../../../measure-theory.md#step-function) $g_N$ are [Riemann integrable](../../../real-analysis.md#riemann-integrable-function). Put $c_j=f(j/N)$. Integrating each constant piece explicitly gives

$$
\int_0^1g_N(t)\cos(nt)\,dt
=\frac1n\sum_{j=0}^{N-1}c_j
\left[\sin\left(\frac{n(j+1)}N\right)
-\sin\left(\frac{nj}N\right)\right].
$$

Since the sine differences have absolute value at most $2$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) and uniform approximation give

$$
\begin{aligned}
|u_n|
&\le\left|\int_0^1(f-g_N)(t)\cos(nt)\,dt\right|
+\left|\int_0^1g_N(t)\cos(nt)\,dt\right|\\
&\le\frac1N+\frac2n\sum_{j=0}^{N-1}|c_j|.
\end{aligned}
$$

To prove convergence, fix $\varepsilon>0$ and first choose $N$ with $1/N<\varepsilon/2$. With this $N$ held fixed, the finite number $\sum_j|c_j|$ is independent of $n$, so the second term is also less than $\varepsilon/2$ for sufficiently large $n$. Therefore

$$
\boxed{u_n\longrightarrow0.}
$$

**First make the approximation error small, then let the oscillation frequency grow.** This is the [step-function proof of the Riemann-Lebesgue lemma](../../../fourier-analysis.md#step-function-proof-of-the-riemann-lebesgue-lemma); it does not require assuming that a Lipschitz function has an everywhere-defined derivative.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
