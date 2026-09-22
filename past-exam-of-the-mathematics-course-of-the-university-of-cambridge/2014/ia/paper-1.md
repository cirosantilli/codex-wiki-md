# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2014/PaperIA_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2014/PaperIA_1.pdf)

**Table of contents**

- [1B](#1b)
  - [a](#1b/a)
    - [i](#1b/a/i)
      - [Solution](#1b/a/i/solution)
    - [ii](#1b/a/ii)
      - [Solution](#1b/a/ii/solution)
  - [b](#1b/b)
    - [Solution](#1b/b/solution)
  - [c](#1b/c)
    - [Solution](#1b/c/solution)
- [2A](#2a)
  - [a](#2a/a)
    - [Solution](#2a/a/solution)
  - [b](#2a/b)
    - [Solution](#2a/b/solution)
- [3D](#3d)
  - [Solution](#3d/solution)
- [4F](#4f)
  - [i](#4f/i)
    - [Solution](#4f/i/solution)
  - [ii](#4f/ii)
    - [Solution](#4f/ii/solution)
- [5B](#5b)
  - [i](#5b/i)
    - [Solution](#5b/i/solution)
  - [ii](#5b/ii)
    - [Solution](#5b/ii/solution)
  - [iii](#5b/iii)
    - [Solution](#5b/iii/solution)
- [6A](#6a)
  - [i](#6a/i)
    - [Solution](#6a/i/solution)
  - [ii](#6a/ii)
    - [Solution](#6a/ii/solution)
- [7C](#7c)
  - [Solution](#7c/solution)
- [8C](#8c)
  - [i](#8c/i)
    - [Solution](#8c/i/solution)
  - [ii](#8c/ii)
    - [Solution](#8c/ii/solution)
  - [iii](#8c/iii)
    - [Solution](#8c/iii/solution)
  - [iv](#8c/iv)
    - [Solution](#8c/iv/solution)
- [9D](#9d)
  - [a](#9d/a)
    - [Solution](#9d/a/solution)
  - [b](#9d/b)
    - [Solution](#9d/b/solution)
- [10E](#10e)
  - [i](#10e/i)
    - [Solution](#10e/i/solution)
  - [ii](#10e/ii)
    - [Solution](#10e/ii/solution)
  - [iii](#10e/iii)
    - [Solution](#10e/iii/solution)
- [11E](#11e)
  - [i](#11e/i)
    - [Solution](#11e/i/solution)
  - [ii](#11e/ii)
    - [Solution](#11e/ii/solution)
- [12F](#12f)
  - [a](#12f/a)
    - [Solution](#12f/a/solution)
  - [b](#12f/b)
    - [Solution](#12f/b/solution)

## 1B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1b/a">a</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/a/i">i</h4>

↑ **Parent:** [A](#1b/a)

<h5 id="1b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1b/a/i)

Squaring first avoids unnecessary expansion: $(2+2i)^2=8i$, and squaring again gives **the fourth power** $\boxed{z^4=-64}$. In the [polar form of a complex number](../../../complex-analysis.md#polar-form-of-a-complex-number), $z=2\sqrt2\,e^{i\pi/4}$; multiplying its [complex argument](../../../complex-analysis.md#argument-complex-analysis) by four gives the same negative-real result.

<h4 id="1b/a/ii">ii</h4>

↑ **Parent:** [A](#1b/a)

<h5 id="1b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1b/a/ii)

Write a nonzero [complex number](../../../complex-analysis.md#complex-number) as $w=re^{i\theta}$. Matching [modulus](../../../complex-analysis.md#modulus) and [complex argument](../../../complex-analysis.md#argument-complex-analysis) gives $r^4=2\sqrt2$ and $4\theta=\pi/4+2\pi k$. Thus **the four distinct fourth roots are**

$$
\boxed{w_k=2^{3/8}\exp\!\left(i\left(\frac\pi{16}+\frac{k\pi}2\right)\right),\qquad k=0,1,2,3.}
$$

These angles differ by $\pi/2$, so the values are distinct. Every further integer $k$ repeats one of them; this is multiplication by the fourth [roots of unity](../../../algebra.md#root-of-unity).

<h3 id="1b/b">b</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/b/solution">Solution</h4>

↑ **Parent:** [B](#1b/b)

The exponent in the PDF is $2z^2$. A [complex exponential](../../../calculus.md#complex-exponential-function) equals one precisely when its exponent is an integer multiple of $2\pi i$: its real part must be zero, and its imaginary part must be a full rotation. Therefore $z^2=\pi i k$ for $k\in\mathbb Z$. Taking both square roots yields **all solutions**

$$
\boxed{\{0\}\ \cup\ \left\{\pm\sqrt{\frac{\pi k}2}(1+i):k=1,2,\ldots\right\}
\ \cup\ \left\{\pm\sqrt{\frac{\pi k}2}(1-i):k=1,2,\ldots\right\}.}
$$

The first nonzero family corresponds to positive exponent index, and the second to negative index. Both signs are required.

<h3 id="1b/c">c</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/c/solution">Solution</h4>

↑ **Parent:** [C](#1b/c)

For a real line $ux+vy+w=0$, with $(u,v)\ne(0,0)$, choose $B=(u-iv)/2$ and $C=w$. Direct multiplication gives $Bz+\overline B\,\overline z=ux+vy$, so **every line has the required form** with $B\ne0$.

For a [circle](../../../topology.md#circle) of centre $c$ and radius $\rho>0$, expand its [modulus](../../../complex-analysis.md#modulus) equation:

$$
|z-c|^2=\rho^2
\iff z\overline z-\overline c z-c\overline z+|c|^2-\rho^2=0.
$$

Thus **the required [circle](../../../topology.md#circle) parameters are** $\boxed{B=-c,\ C=|c|^2-\rho^2}$. Conversely, completing the square in the [circle](../../../topology.md#circle) form gives $|z+B|^2=|B|^2-C$, which describes a genuine [circle](../../../topology.md#circle) when $|B|^2-C>0$. The [complex conjugate](../../../complex-analysis.md#complex-conjugate) terms make both equations real-valued.

## 2A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2a/a">a</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/a/solution">Solution</h4>

↑ **Parent:** [A](#2a/a)

An [eigenvector](../../../linear-operator-theory.md#eigenvector) of a [matrix](../../../vector-space.md#matrix) $A$ is a nonzero vector $v$ for which $Av=\lambda v$. The scalar $\lambda$ is its [eigenvalue](../../../linear-operator-theory.md#eigenvalue). For a fixed [eigenvalue](../../../linear-operator-theory.md#eigenvalue), the zero vector together with all corresponding [eigenvectors](../../../linear-operator-theory.md#eigenvector) forms the [eigenspace](../../../linear-operator-theory.md#eigenspace) $\ker(A-\lambda I)$. The requirement $v\ne0$ prevents every scalar from being an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) merely because $A0=\lambda0$.

<h3 id="2a/b">b</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/b/solution">Solution</h4>

↑ **Parent:** [B](#2a/b)

Expanding the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) gives

$$
\det(\lambda I-A)=\lambda^3-2\lambda^2-\lambda+2
=(\lambda+1)(\lambda-1)(\lambda-2).
$$

Solving the three nullspace systems gives **the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and [eigenspaces](../../../linear-operator-theory.md#eigenspace)**

$$
\boxed{E_{-1}=\operatorname{span}\{(1,1,1)^T\},\quad
E_1=\operatorname{span}\{(1,1,0)^T\},\quad
E_2=\operatorname{span}\{(0,1,-1)^T\}.}
$$

For example, at $\lambda=1$ the first two equations force $z=0$ and $x=y$; at $\lambda=2$ they force $x=0$ and $y=-z$; at $\lambda=-1$ they force $x=y=z$.

Putting these [eigenvectors](../../../linear-operator-theory.md#eigenvector) in columns proves their [linear independence](../../../vector-space.md#linear-independence):

$$
P=\begin{pmatrix}1&1&0\\1&1&1\\1&0&-1\end{pmatrix},\qquad\det P=1,\qquad
P^{-1}AP=\operatorname{diag}(-1,1,2).
$$

Hence **$A$ is a [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) over the reals**.

## 3D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3d/solution">Solution</h3>

↑ **Parent:** [3D](#3d)

Call an index $n$ a peak if $a_n\geq a_m$ for every $m>n$. If there are infinitely many peaks, list their indices increasingly. Each selected value is at least every later selected value, so this gives a nonincreasing [subsequence](../../../real-analysis.md#subsequence).

If there are only finitely many peaks, choose an index beyond the last one. Every index from then onward has a later index with strictly larger value. Select these recursively: $n_{j+1}>n_j$ with $a_{n_{j+1}}>a_{n_j}$. This gives an increasing [subsequence](../../../real-analysis.md#subsequence). Neither [complex argument](../../../complex-analysis.md#argument-complex-analysis) requires the original [sequence](../../../real-analysis.md#sequence) to be bounded. **Every real [sequence](../../../real-analysis.md#sequence) therefore has a monotone [subsequence](../../../real-analysis.md#subsequence)**, as asserted by the [monotone subsequence theorem](../../../real-analysis.md#monotone-subsequence-theorem).

## 4F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4f/i">i</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/i/solution">Solution</h4>

↑ **Parent:** [I](#4f/i)

Let $a_n=n!/n^n$. Its consecutive coefficient ratio is

$$
\frac{a_{n+1}}{a_n}=\left(\frac n{n+1}\right)^n\longrightarrow e^{-1}.
$$

The [ratio test](../../../real-analysis.md#ratio-test) for the full terms therefore has limit $|z|/e$: the series has [absolute convergence](../../../real-analysis.md#absolute-convergence) when $|z|<e$ and its terms eventually grow in magnitude when $|z|>e$. Thus **the [radius of convergence](../../../real-analysis.md#radius-of-convergence) is** $\boxed{R=e}$. No boundary decision is needed to determine the [radius of convergence](../../../real-analysis.md#radius-of-convergence).

<h3 id="4f/ii">ii</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4f/ii)

This is a [lacunary power series](../../../real-analysis.md#lacunary-power-series): the coefficient of $z^{n!}$ is $n^n$, while the other coefficients are zero. Along its nonzero coefficients,

$$
(n^n)^{1/n!}=\exp\!\left(\frac{n\log n}{n!}\right)\longrightarrow1.
$$

The factorial dominates $n\log n$; for example $n!\geq n(n-1)(n-2)(n-3)$ for large $n$ already suffices for this limit. Hence the coefficient limsup in the [Cauchy-Hadamard theorem](../../../real-analysis.md#cauchy-hadamard-theorem) is one. **The [radius of convergence](../../../real-analysis.md#radius-of-convergence) is** $\boxed{R=1}$.

Directly, for $|z|<1$ the consecutive term ratio is $(n+1)^{n+1}n^{-n}|z|^{n n!}$, which tends to zero; for $|z|\geq1$ the term magnitudes are at least $n^n$ and fail to tend to zero. The factorial is the exponent of $z$, not part of its coefficient.

## 5B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5b/i">i</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/i/solution">Solution</h4>

↑ **Parent:** [I](#5b/i)

The first coordinate of the [vector triple product](../../../calculus.md#vector-triple-product) is

$$
[a\times(b\times c)]_1=a_2(b_1c_2-b_2c_1)-a_3(b_3c_1-b_1c_3)
=b_1(a\cdot c)-c_1(a\cdot b).
$$

The other two coordinates follow by cyclically permuting the indices, proving the identity.

A point on the line has the form $r=b+s m$. Substituting in the [plane](../../../geometry-and-topology.md#plane) equation gives $s(m\cdot n)=(a-b)\cdot n$. When $m\cdot n\ne0$ the parameter, and therefore the intersection point, is unique. The [vector triple product](../../../calculus.md#vector-triple-product) gives $n\times(b\times m)=(n\cdot m)b-(n\cdot b)m$, so **the unique intersection is**

$$
\boxed{r=b+\frac{(a-b)\cdot n}{m\cdot n}m
=\frac{(a\cdot n)m+n\times(b\times m)}{m\cdot n}.}
$$

For the parallel case $m\cdot n=0$, the line is entirely in the [plane](../../../geometry-and-topology.md#plane) if $(b-a)\cdot n=0$, and otherwise has no intersection. As usual, a genuine line and [plane](../../../geometry-and-topology.md#plane) require nonzero direction and normal vectors. This is the [line-plane intersection criterion](../../../geometry-and-topology.md#line-plane-intersection-criterion).

<h3 id="5b/ii">ii</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5b/ii)

The [plane](../../../geometry-and-topology.md#plane) through $a_i$ has the constant normal coordinate $r\cdot\widehat n=a_i\cdot\widehat n$. Since $\widehat n$ is a [unit vector](../../../vector-space.md#unit-vector), the separation of these normal coordinates is a length. Every displacement joining the [planes](../../../geometry-and-topology.md#plane) has this fixed normal component, so its length is at least its absolute value; a displacement parallel to $\widehat n$ attains that bound. Hence **the distance between parallel [planes](../../../geometry-and-topology.md#plane) is**

$$
\boxed{d=|(a_1-a_2)\cdot\widehat n|.}
$$

The absolute value, present in the PDF, is necessary because distance is nonnegative.

<h3 id="5b/iii">iii</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5b/iii)

Take points $p=(3,0,4)$ and $q=(-2,3,3)$ with directions $u=(1,3,-1)$ and $v=(0,1,-1)$. A common normal is $u\times v=(-2,1,1)$, of length $\sqrt6$. The [planes](../../../geometry-and-topology.md#plane) through the two lines with this common normal have separation

$$
\frac{|(q-p)\cdot(u\times v)|}{|u\times v|}
=\frac{12}{\sqrt6}=2\sqrt6.
$$

This is a lower bound for the [distance between skew lines](../../../geometry-and-topology.md#distance-between-skew-lines). It is attained at $s=-1$ and $t=-4$: the two points are $(2,-3,5)$ and $(-2,-1,7)$, whose difference $(4,-2,-2)$ is perpendicular to both directions and has length $2\sqrt6$. Thus **the shortest distance is** $\boxed{2\sqrt6}$.

## 6A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6a/i">i</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/i/solution">Solution</h4>

↑ **Parent:** [I](#6a/i)

View a possible complex [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$ using the [Hermitian inner product](../../../linear-algebra.md#hermitian-form). For a real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), $A^\dagger=A$, so $v^\dagger Av$ is real. Since $v^\dagger Av=\lambda v^\dagger v$ and $v^\dagger v>0$, **every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is real**.

For [eigenvectors](../../../linear-operator-theory.md#eigenvector) $v,w$ with distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda,\mu$, symmetry gives

$$
\lambda v^\dagger w=(Av)^\dagger w=v^\dagger Aw=\mu v^\dagger w,
$$

so **$v^\dagger w=0$**. In particular, real [eigenvectors](../../../linear-operator-theory.md#eigenvector) are [orthogonal](../../../linear-algebra.md#orthogonal-vectors) in the real [dot product](../../../linear-algebra.md#dot-product).

Use the permitted diagonalizability assumption to take bases of the real [eigenspaces](../../../linear-operator-theory.md#eigenspace) whose union spans $\mathbb R^n$. Apply the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process) within each [eigenspace](../../../linear-operator-theory.md#eigenspace). Its linear combinations remain [eigenvectors](../../../linear-operator-theory.md#eigenvector) of that same [eigenvalue](../../../linear-operator-theory.md#eigenvalue); vectors in different [eigenspaces](../../../linear-operator-theory.md#eigenspace) are already [orthogonal](../../../linear-algebra.md#orthogonal-vectors). The resulting union is **an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector)**, giving an [orthogonal diagonalization of a real symmetric matrix](../../../linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix).

<h3 id="6a/ii">ii</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6a/ii)

If $Ax=b$ and $h\in\ker A$, symmetry gives $b\cdot h=(Ax)\cdot h=x\cdot Ah=0$, proving necessity. Conversely, expand $b$ in the [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) from part (i), with $Ay_i=\lambda_i y_i$. The zero-[eigenvalue](../../../linear-operator-theory.md#eigenvalue) vectors span the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map). If $b$ is [orthogonal](../../../linear-algebra.md#orthogonal-vectors) to that kernel, then $b\cdot y_i=0$ whenever $\lambda_i=0$, so the remaining coordinates can be solved independently.

For a nonzero [eigenvalue](../../../linear-operator-theory.md#eigenvalue) and any associated nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$, symmetry gives $b\cdot v=\lambda x\cdot v$. Thus **the component vector along $v$ is**

$$
\boxed{\operatorname{proj}_v x=\frac{b\cdot v}{\lambda\|v\|^2}v.}
$$

For the unit vectors $y_i$, this coefficient is $(b\cdot y_i)/\lambda_i$. Consequently **the general solution is**

$$
\boxed{x=\sum_{\lambda_i\ne0}\frac{b\cdot y_i}{\lambda_i}y_i
+\sum_{\lambda_i=0}c_i y_i,\qquad c_i\in\mathbb R.}
$$

This proves sufficiency as well as the claimed kernel criterion. If the compatibility condition fails, there is no solution; if it holds, the freedom is exactly an arbitrary kernel vector.

## 7C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7c/solution">Solution</h3>

↑ **Parent:** [7C](#7c)

Reading the coefficients of the [linear map](../../../vector-space.md#linear-map) gives

$$
\boxed{A=\begin{pmatrix}e^{i\theta}&1\\1&e^{-i\phi}\end{pmatrix},\qquad
\det A=e^{i(\theta-\phi)}-1
=2i\sin\!\left(\frac{\theta-\phi}2\right)e^{i(\theta-\phi)/2}.}
$$

Under the inverse identification, the four standard real basis vectors map respectively to $(1,0)$, $(i,0)$, $(0,1)$ and $(0,i)$ in $\mathbb C^2$. Applying $A$ and taking real and imaginary parts therefore gives the columns

$$
\begin{aligned}
\mathcal B e_1&=(\cos\theta,\sin\theta,1,0)^T,\\
\mathcal B e_2&=(-\sin\theta,\cos\theta,0,1)^T,\\
\mathcal B e_3&=(1,0,\cos\phi,-\sin\phi)^T,\\
\mathcal B e_4&=(0,1,\sin\phi,\cos\phi)^T.
\end{aligned}
$$

Thus **the real [matrix](../../../vector-space.md#matrix) is**

$$
\boxed{B=\begin{pmatrix}
\cos\theta&-\sin\theta&1&0\\
\sin\theta&\cos\theta&0&1\\
1&0&\cos\phi&\sin\phi\\
0&1&-\sin\phi&\cos\phi
\end{pmatrix}.}
$$

For verification, write its blocks as $\begin{pmatrix}R_\theta&I\\I&R_{-\phi}\end{pmatrix}$, where $R_\psi$ is the planar rotation [matrix](../../../vector-space.md#matrix). Block elimination gives $\det B=\det(R_{\theta-\phi}-I)=2-2\cos(\theta-\phi)$. Therefore **the determinant identity is**

$$
\boxed{\det B=4\sin^2\!\left(\frac{\theta-\phi}2\right)=|\det A|^2.}
$$

This is an instance of the [realification determinant identity](../../../vector-space.md#realification-determinant-identity). The identification is real-linear; it is not an identification of complex vector-space dimensions.

## 8C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8c/i">i</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/i/solution">Solution</h4>

↑ **Parent:** [I](#8c/i)

Expanding the [commutator](../../../lie-algebra.md#commutator) immediately gives $[A,A]=0$, $[A,B]=-[B,A]$, and $[A,\lambda B]=\lambda[A,B]$. For its [matrix trace](../../../linear-algebra.md#matrix-trace), write

$$
\operatorname{tr}(AB)=\sum_{i,j}A_{ij}B_{ji}
=\sum_{j,i}B_{ji}A_{ij}=\operatorname{tr}(BA).
$$

Consequently **every [matrix](../../../vector-space.md#matrix) [commutator](../../../lie-algebra.md#commutator) is traceless**: $\boxed{\operatorname{tr}[A,B]=0}$. This is the [trace of a matrix commutator](../../../lie-algebra.md#trace-of-a-matrix-commutator) identity, valid for arbitrary square [matrices](../../../vector-space.md#matrix) over the [complex numbers](../../../complex-analysis.md#complex-number).

<h3 id="8c/ii">ii</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8c/ii)

The [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose) reverses multiplication. If $A^\dagger=-A$ and $B^\dagger=-B$, then

$$
[A,B]^\dagger=B^\dagger A^\dagger-A^\dagger B^\dagger
=BA-AB=-[A,B].
$$

Thus **the [commutator](../../../lie-algebra.md#commutator) is again a [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix)**. The order reversal is what produces the required minus sign.

<h3 id="8c/iii">iii</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8c/iii)

For $a=(a_1,a_2,a_3)$ the map has the explicit form

$$
\mathcal M(a)=\frac12\begin{pmatrix}ia_1&a_2+ia_3\\-a_2+ia_3&-ia_1\end{pmatrix}.
$$

Its diagonal entries sum to zero and its [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose) is its negative, because the three coordinates are real. Hence it is traceless and a [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix).

Direct multiplication of the given basis [matrices](../../../vector-space.md#matrix) yields

$$
[M_1,M_2]=M_3,\qquad[M_2,M_3]=M_1,\qquad[M_3,M_1]=M_2.
$$

The reverse products give the negative [commutators](../../../lie-algebra.md#commutator), and equal-index [commutators](../../../lie-algebra.md#commutator) vanish. Bilinearity then gives

$$
[\mathcal M(a),\mathcal M(b)]
=(a_2b_3-a_3b_2)M_1+(a_3b_1-a_1b_3)M_2+(a_1b_2-a_2b_1)M_3.
$$

Thus **the [cross product](../../../vector-space.md#cross-product) is represented by the [commutator](../../../lie-algebra.md#commutator)**:

$$
\boxed{\mathcal M(a\times b)=[\mathcal M(a),\mathcal M(b)].}
$$

This realizes the [cross-product model of su(2)](../../../linear-operator-theory.md#cross-product-model-of-su-2) with exactly the normalization and cyclic orientation used here.

<h3 id="8c/iv">iv</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#8c/iv)

Every traceless [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix) of size two has the form

$$
C=\begin{pmatrix}ip&w\\-\overline w&-ip\end{pmatrix},\qquad p\in\mathbb R,
$$

so it equals $\mathcal M(c)$ for $c=(2p,2\operatorname{Re}w,2\operatorname{Im}w)$. If $c=0$, take $A=B=0$. Otherwise choose a [unit vector](../../../vector-space.md#unit-vector) $u$ perpendicular to $c$ and set $a=u$, $b=c\times u$. The [vector triple product](../../../calculus.md#vector-triple-product) gives $a\times b=c$.

By part (iii), choosing $A=\mathcal M(a)$ and $B=\mathcal M(b)$ gives **the required representation**

$$
\boxed{C=[A,B].}
$$

In fact both factors can themselves be chosen as traceless [skew-Hermitian matrices](../../../linear-operator-theory.md#skew-hermitian-matrix). The [cross-product model of su(2)](../../../linear-operator-theory.md#cross-product-model-of-su-2) explains this geometric [commutator](../../../lie-algebra.md#commutator) construction.

## 9D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9d/a">a</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/a/solution">Solution</h4>

↑ **Parent:** [A](#9d/a)

Use $\sin0=0$, the [derivative](../../../calculus.md#derivative) identity $\sin'=\cos$, [continuity](../../../calculus.md#continuous-function) of cosine at zero, and $\cos0=1$. For $u\ne0$, the [mean value theorem](../../../calculus.md#mean-value-theorem) gives $\sin u/u=\cos c_u$ for a point between zero and $u$. Hence $\sin u/u\to1$ as $u\to0$. For $x\ne0$, apply this with $u=x/3^k$ to obtain **the limit** $\boxed{3^k\sin(x/3^k)\to x}$. For $x=0$ every term is zero.

The additional bound $|\cos t|\leq1$ and the same [mean value theorem](../../../calculus.md#mean-value-theorem) give $|\sin u|\leq|u|$. Therefore

$$
2^n\left|\sin\left(\frac x{3^n}\right)\right|\leq|x|\left(\frac23\right)^n.
$$

The right side is summable. By the [comparison test for series](../../../real-analysis.md#comparison-test-for-series) **the stated series has [absolute convergence](../../../real-analysis.md#absolute-convergence) for every real $x$**.

<h3 id="9d/b">b</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/b/solution">Solution</h4>

↑ **Parent:** [B](#9d/b)

Let $r=e^{i\theta}\ne1$. The [geometric series](../../../real-analysis.md#geometric-series) from any starting index is bounded:

$$
B_j=\sum_{n=m}^j r^n=\frac{r^m(1-r^{j-m+1})}{1-r},\qquad
|B_j|\leq K=\frac2{|1-r|}.
$$

Using [summation by parts](../../../analytic-number-theory.md#abel-s-summation-formula),

$$
\sum_{n=m}^N a_nr^n=a_NB_N+\sum_{n=m}^{N-1}(a_n-a_{n+1})B_n.
$$

Since the coefficients are nonincreasing and positive, the [modulus](../../../complex-analysis.md#modulus) is at most $K(a_N+a_m-a_N)=Ka_m\to0$. The Cauchy criterion proves **convergence for every $\theta\notin2\pi\mathbb Z$**. This is a direct proof of the [Dirichlet test](../../../real-analysis.md#dirichlet-test) in this setting.

For $a_n=1/n$, the imaginary parts of the convergent partial sums give convergence of the sine series at those angles. If $\theta\in2\pi\mathbb Z$, every sine term is zero. Hence **the sine series converges for all real angles**.

## 10E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10e/i">i</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/i/solution">Solution</h4>

↑ **Parent:** [I](#10e/i)

The [mean value theorem](../../../calculus.md#mean-value-theorem) states that a function [continuous](../../../calculus.md#continuous-function) on $[p,q]$ and differentiable on $(p,q)$ has some $c\in(p,q)$ with $f(q)-f(p)=f'(c)(q-p)$.

Take any $p<q$ inside the given open interval. Differentiability implies the [continuity](../../../calculus.md#continuous-function) needed on $[p,q]$, and the [derivative](../../../calculus.md#derivative) is zero throughout it. The [mean value theorem](../../../calculus.md#mean-value-theorem) therefore gives $f(q)=f(p)$. Since the two points were arbitrary, **the function is constant on the interval**.

<h3 id="10e/ii">ii</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10e/ii)

For [continuity](../../../calculus.md#continuous-function) at any $x$, choose $\delta=\eta^{1/\alpha}$ for a desired error $\eta>0$. If $|y-x|<\delta$, the stated bound gives $|f(y)-f(x)|<\eta$. Thus **$f$ is [continuous](../../../calculus.md#continuous-function)**, in fact [uniformly continuous](../../../topological-analysis.md#uniform-continuity).

When $\alpha>1$, the difference quotient satisfies

$$
\left|\frac{f(x+h)-f(x)}h\right|\leq|h|^{\alpha-1}\longrightarrow0.
$$

Therefore the [derivative](../../../calculus.md#derivative) exists at every point and is zero. Part (i) proves **$f$ is constant**. This is the lemma that [Hölder exponent greater than one forces constancy](../../../sobolev-space.md#holder-exponent-greater-than-one-forces-constancy); no differentiability was assumed in advance.

<h3 id="10e/iii">iii</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10e/iii)

Let $D=f'_+(a)$ and write $g(t)=(f(t)-f(a))/(t-a)$ for $t>a$. By the assumed right [derivative](../../../calculus.md#derivative), choose $\delta>0$ with $|g(t)-D|<\epsilon/2$ whenever $a<t<a+\delta$. Choose $b_0\in(a,\min(b,a+\delta))$.

Apply the [mean value theorem](../../../calculus.md#mean-value-theorem) to $f$ on $[a,b_0]$. It gives $x\in(a,b_0)$ with $f'(x)=g(b_0)$. Both $g(x)$ and $g(b_0)$ are within $\epsilon/2$ of $D$, so

$$
\boxed{\left|\frac{f(x)-f(a)}{x-a}-f'(x)\right|
\leq|g(x)-D|+|g(b_0)-D|<\epsilon.}
$$

This proves the [endpoint secant-tangent approximation](../../../calculus.md#endpoint-secant-tangent-approximation) without any [continuity](../../../calculus.md#continuous-function) assumption on $f'$. The [continuity](../../../calculus.md#continuous-function) required by the theorem is only that of $f$ itself.

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/i">i</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/i/solution">Solution</h4>

↑ **Parent:** [I](#11e/i)

For $x\ne0$, put $P(t)=\sum_{k=0}^{n-1}f^{(k)}(0)t^k/k!$ and $K=(f(x)-P(x))/x^n$. The auxiliary function $F(t)=f(t)-P(t)-Kt^n$ satisfies

$$
F(x)=F(0)=0,\qquad F^{(j)}(0)=0\quad(1\leq j\leq n-1).
$$

[Rolle's theorem](../../../calculus.md#rolle-theorem) first gives a zero of $F'$ strictly between zero and $x$. Apply [Rolle's theorem](../../../calculus.md#rolle-theorem) to $F'$ between that zero and zero, where $F'(0)=0$, to obtain a zero of $F''$. Continue in this way. The [derivatives](../../../calculus.md#derivative) through order $n-1$ are [continuous](../../../calculus.md#continuous-function), since they are differentiable; hence every application is valid even if $f^{(n)}$ is not [continuous](../../../calculus.md#continuous-function). After $n$ applications there is $c$ strictly between zero and $x$ with $F^{(n)}(c)=0$.

But $F^{(n)}(c)=f^{(n)}(c)-n!K$, so $K=f^{(n)}(c)/n!$. Writing $c=\theta x$ yields **the Taylor formula with Lagrange remainder**

$$
\boxed{f(x)=\sum_{k=0}^{n-1}\frac{f^{(k)}(0)}{k!}x^k
+\frac{f^{(n)}(\theta x)}{n!}x^n,\qquad0<\theta<1.}
$$

The same construction using repeated applications of [Rolle's theorem](../../../calculus.md#rolle-theorem) applies when $x<0$, with intervals ordered from $x$ to zero. For $x=0$ the identity is immediate and any $\theta\in(0,1)$ works. This proves the [Taylor theorem with Lagrange remainder](../../../calculus.md#taylor-theorem-with-lagrange-remainder) using only the allowed theorem and elementary differentiation.

<h3 id="11e/ii">ii</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11e/ii)

From $f''=f$, differentiating successively gives $f^{(2r)}=f$ and $f^{(2r+1)}=f'$ whenever those [derivatives](../../../calculus.md#derivative) have been constructed. Starting with twice differentiability, this relation supplies the next two [derivatives](../../../calculus.md#derivative) at each stage. Thus **$f$ is infinitely differentiable**, and its origin series is

$$
\boxed{A\sum_{r=0}^\infty\frac{x^{2r}}{(2r)!}
+B\sum_{r=0}^\infty\frac{x^{2r+1}}{(2r+1)!}.}
$$

For a fixed $x$, both $f$ and $f'$ are bounded on the compact interval between zero and $x$, say by $M_x$. Every higher [derivative](../../../calculus.md#derivative) is one of these two functions. [Taylor's theorem](../../../calculus.md#taylor-theorem), with the remainder just proved, therefore bounds the order-$n$ remainder by $M_x|x|^n/n!$, which tends to zero: its consecutive positive-term ratio is $|x|/(n+1)$. Hence **the series converges to $f(x)$ for every real $x$**. It also gives $f(x)=A\cosh x+B\sinh x$ by the usual hyperbolic-function series.

At any other centre $a$, apply the proved origin result to $g(t)=f(a+t)$, which also satisfies $g''=g$. Its even [derivatives](../../../calculus.md#derivative) at zero are $f(a)$, and its odd ones are $f'(a)$. Consequently

$$
\boxed{f(a+h)=\sum_{k=0}^\infty\frac{f^{(k)}(a)}{k!}h^k
=f(a)\sum_{r=0}^\infty\frac{h^{2r}}{(2r)!}
+f'(a)\sum_{r=0}^\infty\frac{h^{2r+1}}{(2r+1)!}.}
$$

This proves convergence at every centre without assuming that smoothness alone implies equality to a [Taylor series](../../../calculus.md#taylor-series).

## 12F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/solution">Solution</h4>

↑ **Parent:** [A](#12f/a)

For a bounded real function on $[0,1]$, take a partition $P$ with nodes $0=x_0<\cdots<x_N=1$. Its [lower Darboux sum](../../../real-analysis.md#lower-darboux-sum) and [upper Darboux sum](../../../real-analysis.md#upper-darboux-sum) are

$$
L(f,P)=\sum_j\inf_{[x_{j-1},x_j]}f\,(x_j-x_{j-1}),\qquad
U(f,P)=\sum_j\sup_{[x_{j-1},x_j]}f\,(x_j-x_{j-1}).
$$

The function is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function) when $\sup_P L(f,P)=\inf_P U(f,P)$; their common value is its [Riemann integral](../../../real-analysis.md#riemann-integral). Equivalently, for every $\eta>0$ some partition has $U-L<\eta$. Indeed a common refinement of nearly extremizing upper and lower partitions proves necessity, while arbitrarily small gaps force equality of the two integrals. This is the [Riemann integrability criterion](../../../real-analysis.md#riemann-integrability-criterion).

A [continuous](../../../calculus.md#continuous-function) function on a compact interval is bounded and [uniformly continuous](../../../topological-analysis.md#uniform-continuity). Choose a mesh small enough that its oscillation on each subinterval is less than $\eta$. Then $U-L\leq\eta\sum_j(x_j-x_{j-1})=\eta$; using $\eta/2$ first makes the desired inequality strict. Thus **every [continuous](../../../calculus.md#continuous-function) function on $[0,1]$ is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function)**.

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/solution">Solution</h4>

↑ **Parent:** [B](#12f/b)

For a nondecreasing function, the endpoint bounds show it is bounded. On the uniform partition into $N$ intervals, its [Darboux sums](../../../real-analysis.md#darboux-sum) satisfy

$$
U-L=\frac1N\sum_{j=1}^N\left[f\left(\frac jN\right)-f\left(\frac{j-1}N\right)\right]
=\frac{f(1)-f(0)}N\longrightarrow0.
$$

For a nonincreasing function apply the same calculation to $-f$, or use $|f(1)-f(0)|/N$. Thus **every [monotone function](../../../calculus.md#monotonic-function) on $[0,1]$ is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function)**.

For the unheaded rational-weight example, each summand is nonnegative, and increasing $x$ only adds indices. Hence its sum is nondecreasing and lies between zero and one, including the separately specified value at zero. It is a [left-continuous cumulative function of an atomic measure](../../../calculus.md#left-continuous-cumulative-function-of-an-atomic-measure).

If $q_j\in[0,1)$ and $q_j<x\leq1$, the index $j$ appears in the sum at $x$ but not at $q_j$. All other changes are nonnegative, so $f(x)-f(q_j)\geq2^{-j}$. This remains true for arbitrarily small positive $x-q_j$, proving discontinuity at $q_j$, including a right discontinuity at zero when that rational is encountered. Every interval of positive length contains such a rational in its interior. **The discontinuities are therefore dense**, although **the function is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function)** by the monotone-function result just proved.

More concretely, truncate after the first $N$ weights. The resulting finite sum of step functions is integrable, and the uniform tail is at most $2^{-N}$. This also proves integrability and gives, if its value is desired,

$$
\boxed{\int_0^1 f(x)\,dx=\sum_{k=1}^\infty2^{-k}(1-q_k).}
$$

The integral formula follows by integrating the finite sums and using the uniform tail bound. Here “every interval” has the usual nondegenerate-interval meaning; a singleton is not being asserted to contain a discontinuity.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
