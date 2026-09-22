# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperia_1_2018.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperia_1_2018.pdf)

**Table of contents**

- [1C](#1c)
  - [i](#1c/i)
    - [Solution](#1c/i/solution)
  - [ii](#1c/ii)
    - [Solution](#1c/ii/solution)
  - [iii](#1c/iii)
    - [Solution](#1c/iii/solution)
  - [iv](#1c/iv)
    - [Solution](#1c/iv/solution)
- [2A](#2a)
  - [i](#2a/i)
    - [Solution](#2a/i/solution)
  - [ii](#2a/ii)
    - [Solution](#2a/ii/solution)
  - [iii](#2a/iii)
    - [Solution](#2a/iii/solution)
- [3E](#3e)
  - [Solution](#3e/solution)
- [4D](#4d)
  - [Solution](#4d/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6B](#6b)
  - [a](#6b/a)
    - [Solution](#6b/a/solution)
  - [b](#6b/b)
    - [Solution](#6b/b/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [i](#7b/a/i)
      - [Solution](#7b/a/i/solution)
    - [ii](#7b/a/ii)
      - [Solution](#7b/a/ii/solution)
    - [iii](#7b/a/iii)
      - [Solution](#7b/a/iii/solution)
  - [b](#7b/b)
    - [i](#7b/b/i)
      - [Solution](#7b/b/i/solution)
    - [ii](#7b/b/ii)
      - [Solution](#7b/b/ii/solution)
    - [iii](#7b/b/iii)
      - [Solution](#7b/b/iii/solution)
  - [c](#7b/c)
    - [Solution](#7b/c/solution)
- [8A](#8a)
  - [Solution](#8a/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [Solution](#9f/b/solution)
  - [c](#9f/c)
    - [Solution](#9f/c/solution)
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
  - [c](#10f/c)
    - [Solution](#10f/c/solution)
  - [d](#10f/d)
    - [Solution](#10f/d/solution)
- [11E](#11e)
  - [Solution](#11e/solution)
- [12D](#12d)
  - [a](#12d/a)
    - [Solution](#12d/a/solution)
  - [b](#12d/b)
    - [Solution](#12d/b/solution)

## 1C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1c/i">i</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/i/solution">Solution</h4>

↑ **Parent:** [I](#1c/i)

For $z\ne0$, the principal value of [complex exponentiation](../../../analysis.md#complex-exponentiation) is $z^w=\exp(w\operatorname{Log}z)$, where the [principal complex logarithm](../../../analysis.md#principal-complex-logarithm) is $\operatorname{Log}z=\log|z|+i\operatorname{Arg}z$ with $-\pi<\operatorname{Arg}z\leq\pi$. [De Moivre's theorem](../../../analysis.md#de-moivre-s-theorem) states that $(\cos\theta+i\sin\theta)^n=\cos(n\theta)+i\sin(n\theta)$ for every [integer](../../../number-theory.md#integer) $n$.

Since $\sqrt3+i=2e^{i\pi/6}$, the six roots are

$$
\boxed{z=2^{1/6}\exp\left(i\left(\frac{\pi}{36}+\frac{k\pi}{3}\right)\right),\qquad k=0,1,\ldots,5.}
$$

<h3 id="1c/ii">ii</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1c/ii)

Write $z=re^{i\theta}$ with $-\pi<\theta\leq\pi$. Its principal sixth root is $r^{1/6}e^{i\theta/6}$, whose [complex argument](../../../complex-analysis.md#argument-complex-analysis) lies in $(-\pi/6,\pi/6]$. Equality with $2e^{i\pi/6}$ forces $r=64$ and $\theta=\pi$, so **$z=-64$**.

<h3 id="1c/iii">iii</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1c/iii)

For $z=x+iy$,

$$
i^z=e^{z\operatorname{Log}i}=e^{i\pi z/2}=e^{-\pi y/2}e^{i\pi x/2}.
$$

Matching its [modulus](../../../complex-analysis.md#modulus) and [complex argument](../../../complex-analysis.md#argument-complex-analysis) with $2e^{i\pi/6}$ gives

$$
\boxed{z=\frac13+4k-\frac{2i\log2}{\pi},\qquad k\in\mathbb Z.}
$$

<h3 id="1c/iv">iv</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1c/iv)

The base $e^{5i\pi/2}$ is the [complex number](../../../complex-analysis.md#complex-number) $i$. Principal exponentiation uses the principal logarithm of that base, so this is the same equation as in part iii:

$$
\boxed{z=\frac13+4k-\frac{2i\log2}{\pi},\qquad k\in\mathbb Z.}
$$

## 2A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2a/i">i</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/i/solution">Solution</h4>

↑ **Parent:** [I](#2a/i)

The [vector triple product identity](../../../calculus.md#vector-triple-product) gives $\mathbf n\times(\mathbf n\times\mathbf x)=\mathbf n(\mathbf n\cdot\mathbf x)-\mathbf x$, and hence

$$
\Phi(\mathbf x)=\mathbf x+(\alpha-1)(\mathbf n\cdot\mathbf x)\mathbf n.
$$

Thus $\Phi$ is the identity on the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) $\mathbf n^\perp$ and multiplies the component parallel to $\mathbf n$ by $\alpha$. It is [invertible](../../../calculus.md#invertible-linear-map) exactly when $\alpha\ne0$, and then

$$
\boxed{\Phi^{-1}(\mathbf y)=\mathbf y+(\alpha^{-1}-1)(\mathbf n\cdot\mathbf y)\mathbf n.}
$$

<h3 id="2a/ii">ii</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2a/ii)

The only noninvertible case is $\alpha=0$. Then $\Phi$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto $\mathbf n^\perp$, so

$$
\boxed{\operatorname{im}\Phi=\mathbf n^\perp,\quad \ker\Phi=\operatorname{span}\{\mathbf n\},\quad \operatorname{rank}\Phi=2,\quad \operatorname{nullity}\Phi=1.}
$$

These dimensions agree with the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem).

<h3 id="2a/iii">iii</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2a/iii)

In [Einstein notation](../../../linear-algebra.md#einstein-notation), $(\mathbf n\cdot\mathbf x)n_i=n_in_jx_j$, so the matrix and, for $\alpha\ne0$, its [matrix inverse](../../../linear-algebra.md#matrix-inverse) are

$$
\boxed{A_{ij}=\delta_{ij}+(\alpha-1)n_in_j,\qquad B_{ij}=\delta_{ij}+(\alpha^{-1}-1)n_in_j.}
$$

## 3E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3e/solution">Solution</h3>

↑ **Parent:** [3E](#3e)

Let $(u_n)$ be increasing and bounded above, and let $L=\sup\{u_n:n\in\mathbb N\}$. For every $\varepsilon>0$, the definition of the [supremum](../../../real-analysis.md#supremum) supplies $N$ with $L-\varepsilon<u_N\leq L$. Monotonicity gives $L-\varepsilon<u_n\leq L$ for every $n\geq N$, proving $u_n\to L$. This is the [monotone bounded sequence](../../../real-analysis.md#monotone-bounded-sequence) theorem.

For the recurrence, $f(x_n)>0$ makes $(x_n)$ increasing. If it were bounded above, it would converge to some $L$. Since $x_n\leq L$ and $f$ is decreasing, $f(x_n)\geq f(L)>0$, whence

$$
x_n=1+\sum_{j=1}^{n-1}f(x_j)\geq1+(n-1)f(L)\longrightarrow\infty,
$$

a contradiction. Therefore **$x_n\to\infty$**.

## 4D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4d/solution">Solution</h3>

↑ **Parent:** [4D](#4d)

The [radius of convergence](../../../real-analysis.md#radius-of-convergence) of the [power series](../../../real-analysis.md#power-series) $\sum_{n\geq0}a_nz^n$ is

$$
R=\sup\{r\geq0:\text{the series converges for every }|z|<r\}.
$$

If $|z|<R$, choose $w$ with $|z|<|w|<R$. Since $a_nw^n\to0$, those terms are [bounded](../../../real-analysis.md#bounded-sequence), say $|a_nw^n|\leq M$. Therefore

$$
|a_nz^n|\leq M\left|\frac zw\right|^n,
$$

and comparison with a [geometric series](../../../real-analysis.md#geometric-series) proves [absolute convergence](../../../real-analysis.md#absolute-convergence). If $|z|>R$, convergence would imply absolute convergence at every smaller modulus by the same argument, contradicting the definition of $R$.

If $|a_n|\leq|b_n|$, convergence of $\sum b_nw^n$ implies absolute convergence of $\sum a_nz^n$ whenever $|z|<|w|$. Letting $|w|$ approach the radius of the $b$-series shows that **$R_a\geq R_b$**.

## 5C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

The [dot product](../../../linear-algebra.md#dot-product) and [Euclidean norm](../../../functional-analysis.md#euclidean-norm) are $\mathbf x\cdot\mathbf y=\sum_i x_iy_i$ and $|\mathbf x|=\sqrt{\mathbf x\cdot\mathbf x}$. For every real $t$,

$$
0\leq|\mathbf x-t\mathbf y|^2=|\mathbf x|^2-2t\,\mathbf x\cdot\mathbf y+t^2|\mathbf y|^2.
$$

Its [quadratic discriminant](../../../polynomial.md#quadratic-discriminant) is nonpositive, proving the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) $|\mathbf x\cdot\mathbf y|\leq|\mathbf x||\mathbf y|$. In the inequality asked for, equality holds exactly when $\mathbf x$ is a positive scalar multiple of $\mathbf y$, and

$$
\boxed{\theta=\arccos\frac{\mathbf x\cdot\mathbf y}{|\mathbf x||\mathbf y|}.}
$$

Using the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) and its contraction identity,

$$
(\mathbf a\times\mathbf b)\cdot(\mathbf b\times\mathbf c)
=\varepsilon_{ijk}a_jb_k\varepsilon_{i\ell m}b_\ell c_m
=(\mathbf a\cdot\mathbf b)(\mathbf b\cdot\mathbf c)-|\mathbf b|^2(\mathbf a\cdot\mathbf c).
$$

Put $T=\mathbf a\cdot(\mathbf b\times\mathbf c)$, the [scalar triple product](../../../linear-algebra.md#scalar-triple-product). Cyclic symmetry gives $\mathbf m\cdot\mathbf a=\mathbf m\cdot\mathbf b=\mathbf m\cdot\mathbf c=T$, so each requested angle $\phi$ satisfies $\cos\phi=T/|\mathbf m|$. If every pairwise angle is $\theta$ and $t=\cos\theta$, the preceding identity gives

$$
|\mathbf m|^2=3(1-t^2)+6(t^2-t)=3(1-t)^2,
$$

and therefore **$|\mathbf m|=\sqrt3(1-\cos\theta)$**. This is $0$ when $\theta=0$; for a right-handed [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) and $\theta=\pi/2$, $\mathbf m=\mathbf a+\mathbf b+\mathbf c$ has norm $\sqrt3$.

The three [planes](../../../geometry-and-topology.md#plane) have equations $\mathbf a\cdot\mathbf x=\mathbf a\cdot\mathbf p$, $\mathbf b\cdot\mathbf x=\mathbf b\cdot\mathbf q$, and $\mathbf c\cdot\mathbf x=\mathbf c\cdot\mathbf r$. They meet at one point exactly when $\Delta=\mathbf a\cdot(\mathbf b\times\mathbf c)\ne0$, meaning their normals are [linearly independent vectors](../../../vector-space.md#linear-independence). The point is

$$
\boxed{\mathbf x=
\frac{(\mathbf a\cdot\mathbf p)(\mathbf b\times\mathbf c)+(\mathbf b\cdot\mathbf q)(\mathbf c\times\mathbf a)+(\mathbf c\cdot\mathbf r)(\mathbf a\times\mathbf b)}
{\mathbf a\cdot(\mathbf b\times\mathbf c)}.}
$$

## 6B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6b/a">a</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/a/solution">Solution</h4>

↑ **Parent:** [A](#6b/a)

The characteristic polynomial of the displayed [rotation matrix](../../../linear-algebra.md#rotation-matrix) is $(1-\lambda)(\lambda^2-2\lambda\cos\theta+1)$, so its eigenvalues are $1,e^{i\theta},e^{-i\theta}$, all of [modulus](../../../complex-analysis.md#modulus) one. The real eigenvector $(0,0,1)^T$ spans the rotation axis, while the arguments $\pm\theta$ of the conjugate eigenvalues record the rotation angle on its perpendicular plane.

Applying first the $z$-rotation and then the $x$-rotation gives

$$
R_x(\pi/2)R_z(\pi/2)=
\begin{pmatrix}0&-1&0\\0&0&-1\\1&0&0\end{pmatrix}.
$$

Its $1$-eigenspace is spanned by $(1,-1,1)^T$, so $\mathbf n=(1,-1,1)^T/\sqrt3$. The [matrix trace](../../../linear-algebra.md#matrix-trace) identity $\operatorname{tr}R=1+2\cos\phi$ gives $0=1+2\cos\phi$. Thus **$\phi=2\pi/3$**.

<h3 id="6b/b">b</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/b/solution">Solution</h4>

↑ **Parent:** [B](#6b/b)

The quadratic form has symmetric matrix

$$
A=\begin{pmatrix}7&2&1\\2&3&0\\1&0&3\end{pmatrix},
$$

whose characteristic polynomial is $(\lambda-2)(\lambda-3)(\lambda-8)$. All its eigenvalues are positive, so $A$ is [positive definite](../../../linear-algebra.md#positive-definite-matrix) and $\mathbf x^TA\mathbf x=1$ is an [ellipsoid](../../../geometry-and-topology.md#ellipsoid). The [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) gives semi-axis lengths

$$
\boxed{\frac1{\sqrt2},\quad\frac1{\sqrt3},\quad\frac1{\sqrt8}.}
$$

The nearest points lie in the eigendirection of the largest eigenvalue. Since $(5,2,1)^T$ is an $8$-eigenvector, they are

$$
\boxed{\mathbf x=\pm\frac{(5,2,1)^T}{4\sqrt{15}}.}
$$

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/i">i</h4>

↑ **Parent:** [A](#7b/a)

<h5 id="7b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7b/a/i)

Suppose $A\mathbf v=\lambda\mathbf v$ for a nonzero complex vector. Because a real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) is [Hermitian](../../../hilbert-space.md#hermitian-operator), $\mathbf v^*A\mathbf v$ is real. But $\mathbf v^*A\mathbf v=\lambda\mathbf v^*\mathbf v$, so $\lambda$ is real. The real matrix $A-\lambda I$ is singular; the real or imaginary part of a nonzero complex null vector supplies a nonzero real eigenvector. Thus **every eigenvalue is real and has a real eigenvector**.

<h4 id="7b/a/ii">ii</h4>

↑ **Parent:** [A](#7b/a)

<h5 id="7b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7b/a/ii)

If $A\mathbf u=\lambda\mathbf u$ and $A\mathbf v=\mu\mathbf v$, symmetry gives

$$
\lambda\mathbf u^T\mathbf v=(A\mathbf u)^T\mathbf v=\mathbf u^TA\mathbf v=\mu\mathbf u^T\mathbf v.
$$

For $\lambda\ne\mu$, **$\mathbf u^T\mathbf v=0$**, so the eigenvectors are [orthogonal](../../../linear-algebra.md#orthogonal-vectors).

<h4 id="7b/a/iii">iii</h4>

↑ **Parent:** [A](#7b/a)

<h5 id="7b/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7b/a/iii)

Eigenvectors belonging to distinct eigenvalues are [linearly independent](../../../vector-space.md#linear-independence). With $n$ distinct eigenvalues there are $n$ eigenvectors forming a [basis](../../../vector-space.md#basis), and the matrix is [diagonalizable](../../../linear-operator-theory.md#diagonalizable-matrix). In this eigenbasis, the [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) is a weighted average of the eigenvalues, so it is maximized by choosing $\mathbf v$ in the eigenspace of the largest eigenvalue.

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/i">i</h4>

↑ **Parent:** [B](#7b/b)

<h5 id="7b/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7b/b/i)

From $A\mathbf v=\lambda B\mathbf v$ we have $(A-\lambda B)\mathbf v=0$ with $\mathbf v\ne0$. Thus $A-\lambda B$ is singular and **$\det(A-\lambda B)=0$**.

<h4 id="7b/b/ii">ii</h4>

↑ **Parent:** [B](#7b/b)

<h5 id="7b/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7b/b/ii)

Multiplication by $\mathbf v^*$ gives

$$
\lambda=\frac{\mathbf v^*A\mathbf v}{\mathbf v^*B\mathbf v}.
$$

The numerator is real because $A$ is symmetric, while the denominator is strictly positive because $B$ is [positive definite](../../../linear-algebra.md#positive-definite-matrix). Hence $\lambda$ is real. As $A-\lambda B$ is real and singular, its kernel contains a nonzero real generalized eigenvector.

<h4 id="7b/b/iii">iii</h4>

↑ **Parent:** [B](#7b/b)

<h5 id="7b/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7b/b/iii)

For $A\mathbf u=\lambda B\mathbf u$ and $A\mathbf v=\mu B\mathbf v$, symmetry gives

$$
\lambda\mathbf u^TB\mathbf v=(A\mathbf u)^T\mathbf v=\mathbf u^TA\mathbf v=\mu\mathbf u^TB\mathbf v.
$$

If $\lambda\ne\mu$, **$\mathbf u^TB\mathbf v=0$**: the eigenvectors are orthogonal in the [inner product](../../../linear-algebra.md#inner-product) induced by $B$.

<h3 id="7b/c">c</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/c/solution">Solution</h4>

↑ **Parent:** [C](#7b/c)

The [generalized characteristic polynomial](../../../linear-operator-theory.md#generalized-characteristic-polynomial) is

$$
\det(A-\lambda B)=-(\lambda-2)(\lambda-4)(3\lambda-10).
$$

The [generalized Rayleigh quotient](../../../linear-operator-theory.md#generalized-rayleigh-quotient) is maximized by the largest generalized eigenvalue, $4$. Solving $(A-4B)\mathbf v=0$ gives

$$
\boxed{\max_{\mathbf v\ne0}F(\mathbf v)=4,\qquad \mathbf v\propto(-1,2,0)^T.}
$$

## 8A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8a/solution">Solution</h3>

↑ **Parent:** [8A](#8a)

A real square matrix $M$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) when $M^TM=I$. The planar rotation

$$
R=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}
$$

obeys $R^TR=I$ by the [Pythagorean trigonometric identity](../../../geometry-and-topology.md#pythagorean-trigonometric-identity).

For $A=\begin{pmatrix}a&b\\b&c\end{pmatrix}$, the off-diagonal entry of $RAR^T$ is $\frac12(a-c)\sin2\theta+b\cos2\theta$. Thus

$$
\boxed{(a-c)\sin2\theta+2b\cos2\theta=0.}
$$

If $(a-c,b)\ne(0,0)$, equivalently $\theta=\frac12\operatorname{atan2}(-2b,a-c)+k\pi/2$; if $A$ is scalar, every angle works.

Because $RAR^T$ is an [orthogonal similarity](../../../linear-algebra.md#orthogonal-similarity), its diagonal entries are the eigenvalues

$$
\lambda_\pm=\frac{\operatorname{tr}A\pm\sqrt{(\operatorname{tr}A)^2-4\det A}}2.
$$

The matrix $C=\begin{pmatrix}1&2\\2&1\end{pmatrix}$ has eigenvalues $3,-1$ along $(1,1)^T,(1,-1)^T$. Raising its orthogonal diagonalization to the even power gives

$$
\boxed{C^{2N}=\frac12\begin{pmatrix}3^{2N}+1&3^{2N}-1\\3^{2N}-1&3^{2N}+1\end{pmatrix}.}
$$

## 9F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

The function is [continuous](../../../calculus.md#continuous-function) at $x$ when, for every $\varepsilon>0$, there is $\delta>0$ such that $|y-x|<\delta$ implies $|f(y)-f(x)|<\varepsilon$.

If this holds and $x_n\to x$, eventually $|x_n-x|<\delta$, so $f(x_n)\to f(x)$. Conversely, if continuity fails, some $\varepsilon_0>0$ allows, for every $n$, a point $x_n$ with $|x_n-x|<1/n$ but $|f(x_n)-f(x)|\geq\varepsilon_0$. Then $x_n\to x$ while $f(x_n)\not\to f(x)$, a contradiction. This is the [sequential characterization of continuity in metric spaces](../../../topological-analysis.md#sequential-characterization-of-continuity-in-metric-spaces).

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

Let the nonconstant [polynomial](../../../polynomial.md) have degree $d$ and leading coefficient $c$. If $d$ is odd, its limits at $+\infty$ and $-\infty$ have opposite signs, so the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) shows that its image is $\mathbb R$. If $d$ is even and $c>0$, it tends to $+\infty$ at both ends. Outside a sufficiently large compact interval it exceeds $f(0)$, while on that interval the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) gives a global minimum $a$. Continuity and the intermediate value theorem then give image $[a,\infty)$. For $c<0$, applying this argument to $-f$ gives $(-\infty,a]$. These are **exactly the three possible images**.

<h3 id="9f/c">c</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/c/solution">Solution</h4>

↑ **Parent:** [C](#9f/c)

Applying the functional equation at $x^{\alpha^{-1}}$ repeatedly gives

$$
f(x)=f(x^{\alpha^{-1}})=\cdots=f(x^{\alpha^{-n}}).
$$

Since $x^{\alpha^{-n}}\to1$, continuity at $1$ gives $f(x)=f(1)$. Thus **$f$ is constant**.

Without continuity the claim is false. The function $f(1)=1$ and $f(x)=0$ for $x\ne1$ satisfies $f(x)=f(x^\alpha)$ because $x^\alpha=1$ for positive $x$ exactly when $x=1$, but it is not constant.

## 10F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

Differentiability at $x_0$ means

$$
\frac{f(x)-f(x_0)}{x-x_0}\longrightarrow f'(x_0).
$$

Hence $f(x)-f(x_0)=(x-x_0)(f'(x_0)+o(1))\to0$ as $x\to x_0$. Therefore **every [differentiable function](../../../analysis.md#differentiable-function) is continuous at each point where it is differentiable**.

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

The [mean value theorem](../../../calculus.md#mean-value-theorem) says that if $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$, then $f(b)-f(a)=f'(c)(b-a)$ for some $c\in(a,b)$.

For $F(t)=\cos(e^{-t})$ and $t\geq0$,

$$
|F'(t)|=e^{-t}|\sin(e^{-t})|\leq1.
$$

The mean value theorem gives **$|\cos(e^{-x})-\cos(e^{-y})|\leq|x-y|$**.

For the second inequality put $t=\sqrt{1+x}\geq1$. It becomes $2\log t\leq t-t^{-1}$. The difference $G(t)=t-t^{-1}-2\log t$ satisfies $G(1)=0$ and

$$
G'(t)=1+t^{-2}-2t^{-1}=\frac{(t-1)^2}{t^2}\geq0.
$$

Thus **$\log(1+x)\leq x/\sqrt{1+x}$**.

<h3 id="10f/c">c</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/c/solution">Solution</h4>

↑ **Parent:** [C](#10f/c)

For $x\ne0$, $f(x)=|x|^x=e^{x\log|x|}$, so $f'(x)=|x|^x(\log|x|+1)$. Although $x\log|x|\to0$ makes $f$ continuous at zero, $(f(x)-1)/x\sim\log|x|\to-\infty$, so it is not differentiable there.

Since the [cosine function](../../../geometry-and-topology.md#cosine) is even, $g(x)=\cos|x|=\cos x$, so it is differentiable everywhere with $g'(x)=-\sin x$. Finally, $h(x)=x|x|$ is differentiable everywhere, including at zero, and $h'(x)=2|x|$. Therefore

$$
\boxed{f'(x)=|x|^x(\log|x|+1)\ (x\ne0),\qquad g'(x)=-\sin x,\qquad h'(x)=2|x|.}
$$

<h3 id="10f/d">d</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/d/solution">Solution</h4>

↑ **Parent:** [D](#10f/d)

At a nonzero rational $p/q$ in lowest terms, irrational points approach $p/q$ with function value zero, whereas $f(p/q)=1/q>0$, so $f$ is discontinuous. At zero, $|p/q|\geq1/q$ for nonzero $p$, hence $0\leq f(x)\leq|x|$ and continuity follows.

At an irrational $x$, given $\varepsilon>0$, only finitely many rationals in a bounded neighbourhood have reduced denominator $q\leq1/\varepsilon$. Choose a neighbourhood avoiding those points; throughout it, $f<\varepsilon$. Consequently the continuity set is **$(\mathbb R\setminus\mathbb Q)\cup\{0\}$**. This is a variant of the [Thomae function](../../../mathematics.md#thomae-function).

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/solution">Solution</h3>

↑ **Parent:** [11E](#11e)

The [comparison test for series](../../../real-analysis.md#comparison-test-for-series) states that if $0\leq a_n\leq b_n$ eventually and $\sum b_n$ converges, then $\sum a_n$ converges. The partial sums of $\sum a_n$ are increasing and bounded above by a constant plus the bounded partial sums of $\sum b_n$, so the [monotone bounded sequence](../../../real-analysis.md#monotone-bounded-sequence) theorem applies.

If $\sum x_n$ converges, then $x_n^2\leq x_n$ proves convergence of $\sum x_n^2$. Also $x_n\to0$, so eventually $x_n\leq1/2$ and $x_n/(1-x_n)\leq2x_n$, proving convergence of $\sum x_n/(1-x_n)$. The converse for the square series is false: $x_n=1/(n+1)$ has convergent square series but divergent original series. The converse for the fraction series is true because $x_n\leq x_n/(1-x_n)$.

If $(x_n)$ is positive and decreasing and $\sum x_n$ converges, put $m=\lfloor n/2\rfloor$. Then

$$
(n-m)x_n\leq\sum_{k=m+1}^{n}x_k\longrightarrow0,
$$

so **$nx_n\to0$**. The converse fails for $x_n=1/(n\log n)$ for $n\geq2$: it is decreasing and $nx_n\to0$, but the [integral test for convergence](../../../real-analysis.md#integral-test-for-convergence) shows that its series diverges.

Even convergence of $\sum x_n$ need not imply $(n\log n)x_n\to0$. Choose integers $N_j=\lceil e^{2^j}\rceil$ and set $x_n=(N_j\log N_j)^{-1}$ for $N_{j-1}<n\leq N_j$. This is decreasing, and the $j$th block contributes at most $1/\log N_j\leq2^{-j}$, so the series converges. At $n=N_j$, however, $(n\log n)x_n=1$.

## 12D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12d/a">a</h3>

↑ **Parent:** [12D](#12d)

<h4 id="12d/a/solution">Solution</h4>

↑ **Parent:** [A](#12d/a)

Assume $a_n\to0$. The function is bounded, and every interval has lower [Darboux sum](../../../real-analysis.md#darboux-sum) zero because it contains an irrational. Given $\varepsilon>0$, choose $N$ so that $a_n<\varepsilon/2$ for $n>N$. Put small intervals around the finitely many points $q_1,\ldots,q_N$ whose total length makes their contribution to the upper sum less than $\varepsilon/2$, and refine their endpoints to a partition. On every remaining subinterval the function is at most $\varepsilon/2$, so the upper sum is less than $\varepsilon$. The [Riemann integrability criterion](../../../real-analysis.md#riemann-integrability-criterion) proves that **$f$ is Riemann integrable with integral zero**.

The condition $a_n\to0$ is sufficient but not necessary. Assign $a_n=1$ when $q_n=1/k$ for some positive integer $k$, and $a_n=1/n$ otherwise. Then $(a_n)$ does not tend to zero. Outside a short interval near zero only finitely many unit spikes occur and can be enclosed in intervals of arbitrarily small total length; all remaining values can be made uniformly small except for finitely many further points. The same Darboux-sum argument proves that this $f$ is Riemann integrable with integral zero.

<h3 id="12d/b">b</h3>

↑ **Parent:** [12D](#12d)

<h4 id="12d/b/solution">Solution</h4>

↑ **Parent:** [B](#12d/b)

The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) says first that if $h$ is continuous on $[a,b]$ and $H(x)=\int_a^xh(t)\,dt$, then $H'(x)=h(x)$. Indeed,

$$
\frac{H(x+s)-H(x)}s-h(x)=\frac1s\int_x^{x+s}(h(t)-h(x))\,dt,
$$

whose absolute value tends to zero by continuity. Consequently, if $F$ is differentiable with continuous derivative, applying the first part to $h=F'$ shows that $F(x)-\int_a^xF'(t)\,dt$ has zero derivative and is constant. Hence

$$
\boxed{\int_a^bF'(t)\,dt=F(b)-F(a).}
$$

A derivative need not be [Riemann integrable](../../../real-analysis.md#riemann-integrable-function). Define $f(0)=0$ and $f(x)=x^2\sin(x^{-2})$ for $x\ne0$. Then $f$ is differentiable at zero with $f'(0)=0$, while for $x\ne0$,

$$
f'(x)=2x\sin(x^{-2})-\frac2x\cos(x^{-2}),
$$

which is unbounded near zero. Since every Riemann-integrable function on a compact interval is bounded, **$g=f'|_{[0,1]}$ need not be Riemann integrable**.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
