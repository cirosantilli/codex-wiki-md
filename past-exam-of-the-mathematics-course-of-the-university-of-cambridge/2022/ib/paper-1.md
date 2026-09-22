# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperib_1_2022.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperib_1_2022.pdf)

**Table of contents**

- [1F](#1f)
  - [a](#1f/a)
    - [Solution](#1f/a/solution)
  - [b](#1f/b)
    - [Solution](#1f/b/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3G](#3g)
  - [Solution](#3g/solution)
- [4D](#4d)
  - [Solution](#4d/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6H](#6h)
  - [Solution](#6h/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8F](#8f)
  - [a](#8f/a)
    - [i](#8f/a/i)
      - [Solution](#8f/a/i/solution)
    - [ii](#8f/a/ii)
      - [Solution](#8f/a/ii/solution)
  - [b](#8f/b)
    - [i](#8f/b/i)
      - [Solution](#8f/b/i/solution)
    - [ii](#8f/b/ii)
      - [Solution](#8f/b/ii/solution)
- [9E](#9e)
  - [Solution](#9e/solution)
- [10G](#10g)
  - [a](#10g/a)
    - [Solution](#10g/a/solution)
  - [b](#10g/b)
    - [Solution](#10g/b/solution)
  - [c](#10g/c)
    - [Solution](#10g/c/solution)
  - [d](#10g/d)
    - [Solution](#10g/d/solution)
  - [e](#10g/e)
    - [Solution](#10g/e/solution)
- [11E](#11e)
  - [a](#11e/a)
    - [Solution](#11e/a/solution)
  - [b](#11e/b)
    - [Solution](#11e/b/solution)
  - [c](#11e/c)
    - [Solution](#11e/c/solution)
  - [d](#11e/d)
    - [Solution](#11e/d/solution)
- [12G](#12g)
  - [a](#12g/a)
    - [Solution](#12g/a/solution)
  - [b](#12g/b)
    - [Solution](#12g/b/solution)
  - [c](#12g/c)
    - [Solution](#12g/c/solution)
- [13B](#13b)
  - [a](#13b/a)
    - [Solution](#13b/a/solution)
  - [b](#13b/b)
    - [Solution](#13b/b/solution)
  - [c](#13b/c)
    - [Solution](#13b/c/solution)
- [14B](#14b)
  - [a](#14b/a)
    - [Solution](#14b/a/solution)
  - [b](#14b/b)
    - [Solution](#14b/b/solution)
  - [c](#14b/c)
    - [Solution](#14b/c/solution)
  - [d](#14b/d)
    - [Solution](#14b/d/solution)
  - [e](#14b/e)
    - [Solution](#14b/e/solution)
  - [f](#14b/f)
    - [Solution](#14b/f/solution)
- [15D](#15d)
  - [a](#15d/a)
    - [Solution](#15d/a/solution)
  - [b](#15d/b)
    - [Solution](#15d/b/solution)
- [16C](#16c)
  - [a](#16c/a)
    - [Solution](#16c/a/solution)
  - [b](#16c/b)
    - [Solution](#16c/b/solution)
  - [c](#16c/c)
    - [Solution](#16c/c/solution)
- [17C](#17c)
  - [a](#17c/a)
    - [Solution](#17c/a/solution)
  - [b](#17c/b)
    - [Solution](#17c/b/solution)
  - [c](#17c/c)
    - [Solution](#17c/c/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [Solution](#19h/b/solution)
  - [c](#19h/c)
    - [Solution](#19h/c/solution)

## 1F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1f/a">a</h3>

↑ **Parent:** [1F](#1f)

<h4 id="1f/a/solution">Solution</h4>

↑ **Parent:** [A](#1f/a)

For $A=(a_{ij})\in M_n(\mathbb C)$, the [determinant](../../../linear-algebra.md#determinant) is

$$
\det A
=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)
\prod_{i=1}^na_{i,\sigma(i)}.
$$

For

$$
A=\begin{pmatrix}M&X\\0&N\end{pmatrix},
$$

any nonzero term in the [Leibniz formula for determinants](../../../linear-algebra.md#leibniz-formula-for-determinants) must match every row in the lower block to a column in the $N$ block. The remaining upper rows must then match the $M$ columns. The sum consequently factors into the determinant sums for the two diagonal blocks:

$$
\boxed{\det A=(\det M)(\det N)}.
$$

<h3 id="1f/b">b</h3>

↑ **Parent:** [1F](#1f)

<h4 id="1f/b/solution">Solution</h4>

↑ **Parent:** [B](#1f/b)

Move the first $n-k$ columns of

$$
A=\begin{pmatrix}0&M\\N&0\end{pmatrix}
$$

past its last $k$ columns. This requires $k(n-k)$ column interchanges and produces the [block diagonal matrix](../../../vector-space.md#block-diagonal-matrix)

$$
\begin{pmatrix}M&0\\0&N\end{pmatrix}.
$$

Each interchange reverses the determinant's sign, so part (a) gives

$$
\boxed{\det A=(-1)^{k(n-k)}(\det M)(\det N)}.
$$

## 2E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

A unit-speed curve on a smooth embedded surface is a [geodesic](../../../riemannian-geometry.md#geodesic) exactly when its acceleration is normal to the surface, equivalently when its tangential acceleration vanishes.

Every unit-speed geodesic on the cylinder through $(1,0,0)$ has the form

$$
\boxed{\gamma(s)=(\cos(as),\sin(as),bs)},
\qquad a^2+b^2=1.
$$

Indeed, unrolling the cylinder to its [universal cover](../../../algebraic-topology.md#universal-cover) $\mathbb R^2$ turns these curves into straight lines. Directly,

$$
\gamma''(s)=-a^2(\cos(as),\sin(as),0),
$$

which is parallel to the cylinder's radial [normal vector](../../../differential-geometry.md#normal-vector), verifying the geodesic characterization. Such a geodesic is closed exactly when $b=0$; its image is then the horizontal circle $z=0$.

**Yes.** In polar coordinates $(r,\theta)$ on $\mathbb R^2\setminus\{0\}$, use the [Riemannian metric](../../../differential-geometry.md#riemannian-metric)

$$
g=\frac{dr^2}{r^2}+d\theta^2.
$$

The coordinate $u=\log r$ identifies this surface isometrically with the flat cylinder $\mathbb R\times S^1$. Through each point, the circle $u=\text{constant}$ is a closed geodesic, and every other geodesic has nonzero linear motion in $u$ and is not closed. Thus every point lies on a unique closed geodesic.

## 3G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3g/solution">Solution</h3>

↑ **Parent:** [3G](#3g)

The [Taylor series](../../../calculus.md#taylor-series) of the complex sine is

$$
\sin z=z-\frac{z^3}{3!}+\frac{z^5}{5!}-\cdots.
$$

Therefore, for $z\ne0$,

$$
\frac{\sin z}{z}
=1-\frac{z^2}{3!}+\frac{z^4}{5!}-\cdots,
$$

and the right side defines a [holomorphic function](../../../complex-analysis.md#holomorphic-function) at $z=0$ with value $1$. Thus the apparent singularity is a [removable singularity](../../../isolated-singularity.md#removable-singularity).

The resulting power series is

$$
\sum_{n=0}^{\infty}\frac{(-1)^nz^{2n}}{(2n+1)!}.
$$

The [ratio test](../../../real-analysis.md#ratio-test) shows convergence for every $z\in\mathbb C$, so its [radius of convergence](../../../real-analysis.md#radius-of-convergence) is

$$
\boxed{\infty}.
$$

## 4D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4d/solution">Solution</h3>

↑ **Parent:** [4D](#4d)

For

$$
L(x,y,y')=y'^2-y^2-2y\sin x,
$$

the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is

$$
\frac d{dx}\frac{\partial L}{\partial y'}
-\frac{\partial L}{\partial y}=0.
$$

Here this becomes

$$
2y''+2y+2\sin x=0,
\qquad\text{or}\qquad
y''+y=-\sin x.
$$

Because the forcing is resonant with the complementary solution, a particular integral is $(x/2)\cos x$. Hence

$$
y=A\cos x+B\sin x+\frac x2\cos x,
$$

and

$$
y'=-A\sin x+B\cos x+\frac12\cos x-\frac x2\sin x.
$$

The [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) give

$$
y'(0)=B+\frac12=0,
\qquad
y'(\pi/2)=-A-\frac\pi4=0.
$$

Thus

$$
\boxed{
y(x)=-\frac\pi4\cos x-\frac12\sin x+\frac x2\cos x}.
$$

## 5C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

Let the columns of $A$ be $a_1,a_2,a_3$. The [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process) gives

$$
q_1=\frac{a_1}{|a_1|}
=\frac12(1,1,1,-1)^T,
\qquad r_{11}=4.
$$

Next,

$$
r_{12}=q_1^Ta_2=2,
\qquad
a_2-r_{12}q_1=(1,-1,1,1)^T,
$$

so

$$
q_2=\frac12(1,-1,1,1)^T,
\qquad r_{22}=2.
$$

For the final column,

$$
r_{13}=q_1^Ta_3=-2,
\qquad
r_{23}=q_2^Ta_3=4,
$$

and

$$
a_3-r_{13}q_1-r_{23}q_2=(-1,-1,1,-1)^T.
$$

Thus $q_3=\frac12(-1,-1,1,-1)^T$ and $r_{33}=2$. The reduced [QR decomposition](../../../linear-algebra.md#qr-decomposition) is

$$
\boxed{
Q=\frac12
\begin{pmatrix}
1&1&-1\\
1&-1&-1\\
1&1&1\\
-1&1&-1
\end{pmatrix},
\qquad
R=
\begin{pmatrix}
4&2&-2\\
0&2&4\\
0&0&2
\end{pmatrix}}.
$$

The columns of $Q$ are orthonormal, and direct multiplication gives $QR=A$.

## 6H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6h/solution">Solution</h3>

↑ **Parent:** [6H](#6h)

The [Rao-Blackwell theorem](../../../probability-and-statistics.md#rao-blackwell-theorem) says that if $U$ is an estimator with finite second moment and $T$ is a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic), then

$$
U^*=\mathbb E[U\mid T]
$$

has the same expectation as $U$ and satisfies

$$
\operatorname{Var}(U^*)\leq\operatorname{Var}(U),
$$

with equality only when $U$ is already a function of $T$ almost surely.

Here $\widehat\theta=\mathbf1_{\{X_1=1\}}$ is unbiased because

$$
\mathbb E\widehat\theta
=\mathbb P(X_1=1)=p(1-p)=\theta.
$$

Conditional on $T=t$, every weak composition $(x_1,\ldots,x_n)$ of $t$ has the same probability $p^n(1-p)^t$. There are

$$
\binom{t+n-1}{n-1}
$$

such compositions. For $t\geq1$, those with $x_1=1$ correspond to weak compositions of $t-1$ into $n-1$ parts, of which there are

$$
\binom{t+n-3}{n-2}.
$$

The Rao-Blackwell estimator is therefore

$$
\boxed{
\widehat\theta^*(T)=
\begin{cases}
\displaystyle
\frac{(n-1)T}{(T+n-1)(T+n-2)},&T\geq1,\\[6pt]
0,&T=0.
\end{cases}}
$$

For $n\geq2$ and $0<p<1$, $\widehat\theta$ is not determined by $T$; for example, conditional on $T=1$, the sole failure can occur in any coordinate. The variance inequality is consequently strict:

$$
\boxed{\operatorname{Var}(\widehat\theta^*)<
\operatorname{Var}(\widehat\theta)}.
$$

## 7H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

Starting from $x_0\in\mathbb R^n$, [gradient descent](../../../numerical-analysis.md#gradient-descent) repeatedly computes the gradient and updates

$$
x_{k+1}=x_k-\eta\nabla f(x_k),
$$

stopping when the gradient norm, step, or objective decrease is sufficiently small.

The Hessian bounds say that $f$ is $\alpha$-[strongly convex](../../../real-analysis.md#strongly-convex-function) and has $\beta$-[smooth gradient](../../../numerical-analysis.md#lipschitz-gradient). With $\eta=1/\beta$,

$$
f(x_k)-f(x_*)
\leq
\left(1-\frac{\alpha}{\beta}\right)^k
\bigl(f(x_0)-f(x_*)\bigr).
$$

Thus the iteration count is

$$
O\left(\frac{\beta}{\alpha}\log\frac1\varepsilon\right);
$$

convergence becomes slower linearly with the [condition number](../../../linear-algebra.md#condition-number) $\kappa=\beta/\alpha$.

For

$$
f(x,y,z)=x^2+100y^2+10000z^2,
$$

the [Hessian matrix](../../../calculus.md#hessian-matrix) is $\operatorname{diag}(2,200,20000)$, so

$$
\boxed{\kappa=10000}.
$$

Take

$$
\boxed{A=\operatorname{diag}(1,1/10,1/100)}.
$$

Then

$$
(f\circ A)(u,v,w)=u^2+v^2+w^2,
$$

whose Hessian is $2I$ and whose condition number is $1$.

## 8F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8f/a">a</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/a/i">i</h4>

↑ **Parent:** [A](#8f/a)

<h5 id="8f/a/i/solution">Solution</h5>

↑ **Parent:** [I](#8f/a/i)

The [adjoint operator](../../../hilbert-space.md#adjoint-operator) $\alpha^*$ is defined by

$$
\langle\alpha v,w\rangle=\langle v,\alpha^*w\rangle
\qquad(v,w\in V).
$$

Since $V$ is a nonzero finite-dimensional complex vector space, $\alpha$ has an [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$ with eigenvalue $\lambda$. Normality gives

$$
\|(\alpha-\lambda I)x\|^2
=\|(\alpha^*-\overline\lambda I)x\|^2
$$

for every $x$, by expanding both sides and using $\alpha\alpha^*=\alpha^*\alpha$. Taking $x=v$ yields

$$
\boxed{\alpha v=\lambda v,\qquad
\alpha^*v=\overline\lambda v}.
$$

<h4 id="8f/a/ii">ii</h4>

↑ **Parent:** [A](#8f/a)

<h5 id="8f/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8f/a/ii)

For the common eigenvector $v$, its orthogonal complement $v^\perp$ is invariant under both $\alpha$ and $\alpha^*$. Indeed, if $w\perp v$, then

$$
\langle\alpha w,v\rangle
=\langle w,\alpha^*v\rangle=0,
$$

and the analogous calculation applies to $\alpha^*w$. The restriction of $\alpha$ to $v^\perp$ is therefore again normal. Induction on $\dim V$, beginning with the normalized vector $v/\|v\|$, produces an orthonormal eigenbasis. This proves the finite-dimensional [spectral theorem for normal operators](../../../hilbert-space.md#spectral-theorem-for-normal-operators).

<h3 id="8f/b">b</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/b/i">i</h4>

↑ **Parent:** [B](#8f/b)

<h5 id="8f/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8f/b/i)

If $Av=\lambda v$ for a nonzero real vector $v$, then skew-symmetry gives

$$
\lambda\|v\|^2
=v^TAv
=-(Av)^Tv
=-\lambda\|v\|^2.
$$

Thus

$$
\boxed{\lambda=0},
$$

so a real skew-symmetric matrix has no nonzero real eigenvalue.

<h4 id="8f/b/ii">ii</h4>

↑ **Parent:** [B](#8f/b)

<h5 id="8f/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8f/b/ii)

Over $\mathbb C$, the real [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix) $A$ is normal because $A^*=-A$. Part (a) gives an orthonormal complex eigenbasis, and the nonzero eigenvalues are purely imaginary pairs $\pm i\lambda$.

For each $\lambda>0$, choose a unit real vector $x$ in the kernel of $A^2+\lambda^2I$ and put

$$
y=-\frac1\lambda Ax.
$$

Then $x\perp y$, $\|y\|=1$, and

$$
Ax=-\lambda y,\qquad Ay=\lambda x.
$$

Thus $A$ has matrix

$$
\begin{pmatrix}0&\lambda\\-\lambda&0\end{pmatrix}
$$

on the orthonormal basis $(x,y)$. Distinct such invariant planes are orthogonal; complete them by an orthonormal basis of $\ker A$. Taking these basis vectors as the columns of an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) $R$ gives

$$
\boxed{R^TAR
=\operatorname{diag}\left(
\begin{pmatrix}0&\lambda_1\\-\lambda_1&0\end{pmatrix},
\ldots,
\begin{pmatrix}0&\lambda_r\\-\lambda_r&0\end{pmatrix},
0\right)}.
$$

## 9E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9e/solution">Solution</h3>

↑ **Parent:** [9E](#9e)

A [Euclidean domain](../../../commutative-algebra.md#euclidean-domain) is an integral domain $R$ equipped with a function $\delta:R\setminus\{0\}\to\mathbb N$ such that for $a,b\in R$, $b\ne0$, there are $q,r\in R$ with

$$
a=bq+r,\qquad r=0\ \text{or}\ \delta(r)<\delta(b).
$$

For the [Gaussian integers](../../../commutative-algebra.md#gaussian-integer) $\mathbb Z[i]$, take $\delta(z)=N(z)=|z|^2$. Choosing a Gaussian integer nearest to $a/b$ makes the remainder norm smaller than $N(b)$.

The units are precisely the elements of norm one:

$$
\boxed{\{\pm1,\pm i\}}.
$$

Unique factorization in this Euclidean domain gives

$$
\boxed{
2=-i(1+i)^2,\qquad
5=(2+i)(2-i),\qquad
1+3i=(1+i)(2+i)}.
$$

The displayed factors have prime norms $2$ or $5$, so they are irreducible; factors appearing together are nonassociate.

Now suppose $x^2+4=y^3$. Necessarily $y>0$. First let $y$ be odd. Then $x$ is odd, and $x+2i$ and $x-2i$ are coprime in $\mathbb Z[i]$: a common Gaussian prime would divide $4i$, while their product has odd norm. Hence

$$
x+2i=(a+bi)^3
$$

up to a unit, which can be absorbed into the cube. Comparing imaginary parts gives

$$
b(3a^2-b^2)=2.
$$

Checking $b\mid2$ yields only $b=-2$, $a=\pm1$, and therefore

$$
(x,y)=(\pm11,5).
$$

If $y$ is even, congruence modulo $8$ gives $x=2X$ with $X$ odd and $y=2Y$, where

$$
X^2+1=2Y^3.
$$

Each of $X\pm i$ contains exactly one factor $1+i$, so the coprime quotients are cubes up to units. Thus

$$
X+i=u(1+i)(a+bi)^3.
$$

Comparing the imaginary part after the four possible units reduces to

$$
|(a-b)(a^2+4ab+b^2)|=1
\quad\text{or}\quad
|(a+b)(a^2-4ab+b^2)|=1.
$$

Each integer factor must have absolute value one. Substitution then gives $a^2+b^2=1$, so $Y=1$ and $X=\pm1$. Hence

$$
(x,y)=(\pm2,2).
$$

All four pairs satisfy the equation, so the complete answer is

$$
\boxed{(x,y)=(\pm2,2),\ (\pm11,5)}.
$$

## 10G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10g/a">a</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/a/solution">Solution</h4>

↑ **Parent:** [A](#10g/a)

This is always true. Given $\varepsilon>0$, choose $N_A,N_B$ such that

$$
|f_n(x)-f(x)|<\varepsilon
$$

on $A$ for $n\geq N_A$ and on $B$ for $n\geq N_B$. For $n\geq\max(N_A,N_B)$ the same inequality holds at every point of $X=A\cup B$. Hence $f_n\to f$ [uniformly](../../../real-analysis.md#uniform-convergence) on $X$.

<h3 id="10g/b">b</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/b/solution">Solution</h4>

↑ **Parent:** [B](#10g/b)

This may be false when the limiting functions are unbounded. On $X=\mathbb R$, let

$$
f_n(x)=f(x)=x,
\qquad
g_n(x)=x+\frac1n,
\qquad
g(x)=x.
$$

Both sequences converge uniformly to their stated limits, but

$$
f_ng_n-fg=\frac xn
$$

is unbounded for every $n$. Thus the products do not converge uniformly.

<h3 id="10g/c">c</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/c/solution">Solution</h4>

↑ **Parent:** [C](#10g/c)

For every $(x,y)\in[1,2]^2$,

$$
f_n(x,y)\longrightarrow\frac xy.
$$

Moreover,

$$
\left|\frac{1+nx}{1+ny}-\frac xy\right|
=\frac{|y-x|}{y(1+ny)}
\leq\frac1{n+1}.
$$

The bound is independent of $(x,y)$ and tends to zero, so

$$
\boxed{f_n\to[(x,y)\mapsto x/y]\text{ uniformly}}.
$$

<h3 id="10g/d">d</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/d/solution">Solution</h4>

↑ **Parent:** [D](#10g/d)

This is always true. Uniform convergence makes $(f_n)$ a [uniformly Cauchy sequence](../../../real-analysis.md#uniformly-cauchy-sequence): for every $\varepsilon>0$, there is $N$ such that

$$
d_Y(f_n(x),f_m(x))<\varepsilon
$$

for every $x\in A$ and $m,n\geq N$. Letting $x\to x_0$ through points of $A\setminus\{x_0\}$ and using the assumed limits gives

$$
d_Y(y_n,y_m)\leq\varepsilon.
$$

**Thus $(y_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence). Since $Y$ is a [complete metric space](../../../topological-analysis.md#complete-metric-space), $(y_n)$ converges in $Y$.**

<h3 id="10g/e">e</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/e/solution">Solution</h4>

↑ **Parent:** [E](#10g/e)

This is always true. Since $f$ is bounded and $f_n\to f$ uniformly, there are $M$ and $N$ such that

$$
|f(x)|\leq M,\qquad |f_n(x)|\leq M+1
$$

for every $x\in X$ and $n\geq N$. The continuous function $g$ is [uniformly continuous](../../../topological-analysis.md#uniform-continuity) on the compact interval $[-M-1,M+1]$. Therefore, given $\varepsilon>0$, a sufficiently small uniform bound on $|f_n-f|$ implies

$$
\sup_{x\in X}|g(f_n(x))-g(f(x))|<\varepsilon.
$$

**Hence $g\circ f_n\to g\circ f$ uniformly.**

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/a">a</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/a/solution">Solution</h4>

↑ **Parent:** [A](#11e/a)

Every orientation-preserving isometry of the [Poincaré half-plane model](../../../geometry-and-topology.md#poincare-half-plane-model) has the form

$$
\boxed{z\longmapsto\frac{az+b}{cz+d}},
\qquad a,b,c,d\in\mathbb R,\quad ad-bc=1,
$$

with matrices identified up to multiplication by $-I$. Thus $G\cong PSL(2,\mathbb R)$.

For $z=x+iy\in\mathbb H$, the affine map $(z-x)/y$ sends $z$ to $i$, proving transitivity on points. Real translations and positive dilations act transitively on finite boundary points, while inversion $z\mapsto-1/z$ exchanges $0$ and $\infty$; hence the action on $\mathbb R\cup\{\infty\}$ is transitive. A hyperbolic line is determined by its unordered pair of boundary endpoints, and a real Möbius transformation can send any such pair to $\{0,\infty\}$. Therefore $G$ is also transitive on hyperbolic lines.

<h3 id="11e/b">b</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/b/solution">Solution</h4>

↑ **Parent:** [B](#11e/b)

By point transitivity, it suffices to take $P=i$. The condition

$$
\frac{ai+b}{ci+d}=i
$$

is equivalent to $d=a$, $c=-b$, and the determinant condition becomes $a^2+b^2=1$. Thus the stabilizer consists of

$$
\begin{pmatrix}a&b\\-b&a\end{pmatrix},
\qquad a^2+b^2=1,
$$

modulo $\pm I$. Writing $a=\cos\varphi$, $b=\sin\varphi$ identifies it with rotations of the tangent plane, and the doubled matrix angle removes the $\pm I$ quotient. Hence

$$
\boxed{\operatorname{Stab}_G(P)\cong SO(2)}.
$$

<h3 id="11e/c">c</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/c/solution">Solution</h4>

↑ **Parent:** [C](#11e/c)

An isometry sends the geodesic through $P,Q$ to the imaginary axis and sends the two points to $ir$ and $i/r$ for some $r>0$. The transformation

$$
z\longmapsto-\frac1z
$$

belongs to $PSL(2,\mathbb R)$ and exchanges $ir$ with $i/r$. Conjugating it back gives an orientation-preserving isometry exchanging $P$ and $Q$.

For uniqueness, the quotient of two such isometries fixes both $P$ and $Q$. An orientation-preserving hyperbolic isometry fixing two distinct interior points fixes their connecting geodesic and both tangent directions there, hence is the identity. Therefore the exchanging isometry is unique; geometrically it is the [hyperbolic half-turn](../../../geometry-and-topology.md#hyperbolic-half-turn) about the midpoint of the segment $PQ$.

<h3 id="11e/d">d</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/d/solution">Solution</h4>

↑ **Parent:** [D](#11e/d)

Use an orientation-preserving isometry to send $P$ to $i$ and $\ell$ to the imaginary axis, whose boundary points are $0,\infty$. A geodesic $m$ through $i$ meeting it at angle $\theta$ has boundary points

$$
u=-\tan\frac\theta2,
\qquad
v=\cot\frac\theta2.
$$

Indeed $uv=-1$, so the semicircle with endpoints $u,v$ passes through $i$, and its tangent there makes angle $\theta$ with the vertical.

The [cross-ratio](../../../group-theory.md#cross-ratio) is invariant under the normalizing Möbius transformation. With the suitable ordering $(u,v,\infty,0)$ and the convention used here,

$$
[u,v,\infty,0]
=\frac{v}{v-u}
=\frac{\cot(\theta/2)}
{\cot(\theta/2)+\tan(\theta/2)}
=\boxed{\cos^2\frac\theta2}.
$$

## 12G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12g/a">a</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/a/solution">Solution</h4>

↑ **Parent:** [A](#12g/a)

The hypothesis makes $\Omega$ [star-shaped](../../../algebra.md#star-shaped-set) with centre $z_0$. For small $h$ with the triangle having vertices $z_0,w,w+h$ contained in $\Omega$, the vanishing triangular integral gives

$$
g(w+h)-g(w)=\int_{[w,w+h]}f(z)\,dz.
$$

Parametrizing the final segment,

$$
\frac{g(w+h)-g(w)}h
=\int_0^1f(w+th)\,dt
\longrightarrow f(w)
$$

by continuity. Thus $g$ is [holomorphic](../../../complex-analysis.md#holomorphic-function) and

$$
\boxed{g'(w)=f(w)}.
$$

This is the triangle-integral construction behind [Morera's theorem](../../../complex-analysis.md#morera-s-theorem).

<h3 id="12g/b">b</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/b/solution">Solution</h4>

↑ **Parent:** [B](#12g/b)

The set $D$ is star-shaped with centre $z_0$: if $z\in D$, every point of $[z_0,z]$ has its segment to $z_0$ contained in the same segment and therefore avoids the origin. Applying part (a) and the stated triangular-integral fact to $1/z$ gives a holomorphic function

$$
G(z)=\int_{[z_0,z]}\frac{d\zeta}{\zeta},
\qquad
G'(z)=\frac1z,\quad G(z_0)=0.
$$

Choose either square root $c$ of $z_0$ and define

$$
h(z)=c\,e^{G(z)/2}.
$$

Then $h$ is holomorphic. Moreover,

$$
\frac d{dz}\left(\frac{h(z)^2}{z}\right)=0,
$$

and its value at $z_0$ is one. Hence

$$
\boxed{h(z)^2=z\quad(z\in D)}.
$$

<h3 id="12g/c">c</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/c/solution">Solution</h4>

↑ **Parent:** [C](#12g/c)

Because $\cos0=1$, continuity gives a disc $U$ about zero on which $\cos z\ne0$. The function $-\tan z=(\log\cos z)'$ has a holomorphic primitive $G$ on a sufficiently small disc, normalized by $G(0)=0$. Then

$$
\boxed{f(z)=e^{G(z)/2}}
$$

is holomorphic and satisfies $f(0)=1$ and $f(z)^2=\cos z$ on $U$.

**No such square root exists throughout $|z|<2$.** The point $z=\pi/2$ lies in that disc and is a [simple zero](../../../complex-analysis.md#simple-zero) of $\cos z$, since $-\sin(\pi/2)=-1$. Every zero of the square of a holomorphic function has even [order of a zero of a holomorphic function](../../../complex-analysis.md#order-of-a-zero-of-a-holomorphic-function), contradicting this simple zero.

## 13B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13b/a">a</h3>

↑ **Parent:** [13B](#13b)

<h4 id="13b/a/solution">Solution</h4>

↑ **Parent:** [A](#13b/a)

Take positive $y$ vertically downward. For a short string element, the transverse tension resultant is $T y_{xx}\,dx$, while gravity and linear drag contribute $\mu g\,dx$ and $-2k\mu y_t\,dx$. [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) gives

$$
\mu y_{tt}\,dx
=Ty_{xx}\,dx-2k\mu y_t\,dx+\mu g\,dx.
$$

Since $T=\mu c^2$, the [damped wave equation](../../../wave-equation.md#linearly-damped-string) is

$$
\boxed{y_{tt}+2ky_t-c^2y_{xx}=g},
\qquad
y(0,t)=y(l,t)=0.
$$

Choosing upward displacement reverses the sign of the gravity term.

<h3 id="13b/b">b</h3>

↑ **Parent:** [13B](#13b)

<h4 id="13b/b/solution">Solution</h4>

↑ **Parent:** [B](#13b/b)

With gravity omitted, the initial data contain only the first fixed-end [normal mode](../../../wave-equation.md#normal-mode), so write

$$
y(x,t)=q(t)\sin\frac{\pi x}{l}.
$$

Then

$$
q''+2kq'+\left(\frac{\pi c}{l}\right)^2q=0,
\qquad q(0)=0,\quad q'(0)=A.
$$

Because $k=\pi c/l$, this oscillator is [critically damped](../../../wave-equation.md#critical-damping), and

$$
q(t)=Ate^{-kt}.
$$

Therefore

$$
\boxed{y(x,t)=Ate^{-kt}\sin\frac{\pi x}{l}}.
$$

<h3 id="13b/c">c</h3>

↑ **Parent:** [13B](#13b)

<h4 id="13b/c/solution">Solution</h4>

↑ **Parent:** [C](#13b/c)

The first mode remains the solution from part (b). The applied force excites only the third mode, so

$$
y(x,t)=Ate^{-kt}\sin\frac{\pi x}{l}
+q_3(t)\sin\frac{3\pi x}{l},
$$

where, using $\pi c/l=k$,

$$
q_3''+2kq_3'+9k^2q_3=\alpha\cos kt,
\qquad q_3(0)=q_3'(0)=0.
$$

A particular solution is

$$
q_{3,p}(t)=\frac{\alpha}{34k^2}(4\cos kt+\sin kt).
$$

Adding the decaying complementary solution and imposing the initial conditions gives

$$
\boxed{
q_3(t)=\frac{\alpha}{34k^2}
\left[
4\cos kt+\sin kt
-e^{-kt}\left(
4\cos(2\sqrt2kt)
+\frac5{\sqrt2}\sin(2\sqrt2kt)
\right)
\right]}.
$$

As $t\to\infty$, all transients decay but the driven third-mode oscillation remains. The string approaches a periodic [steady-state response](../../../analysis.md#steady-state-response), rather than coming to rest.

With gravity omitted, its mechanical energy is

$$
E=\frac{\mu}{2}\int_0^l
\left(y_t^2+c^2y_x^2\right)dx.
$$

Writing $s=\alpha/(34k^2)$ and letting $t\to\infty$ gives

$$
\boxed{
E_\infty(t)
=\frac{\mu l\alpha^2}{4624k^2}
\left[
25\sin^2kt+145\cos^2kt
+64\sin kt\cos kt
\right]}.
$$

The limiting energy is periodic because the external force continually supplies the energy dissipated by drag.

## 14B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14b/a">a</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/a/solution">Solution</h4>

↑ **Parent:** [A](#14b/a)

For the one-dimensional [quantum harmonic oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator),

$$
\boxed{
i\hbar\frac{\partial\psi}{\partial t}
=\left(
-\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}
+\frac12m\omega^2x^2
\right)\psi}.
$$

This is the [Time-dependent Schrödinger equation](../../../physics.md#time-dependent-schrodinger-equation) with harmonic potential.

<h3 id="14b/b">b</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/b/solution">Solution</h4>

↑ **Parent:** [B](#14b/b)

For

$$
\psi=N(t)e^{-F(t)x^2+G(t)x},
$$

direct differentiation gives

$$
\psi_x=(-2Fx+G)\psi,
\qquad
\psi_{xx}=(4F^2x^2-4FGx+G^2-2F)\psi
$$

and

$$
\psi_t=\left(\frac{\dot N}{N}-\dot F x^2+\dot Gx\right)\psi.
$$

Substitution into the Schrodinger equation and equality of the coefficients of $x^2,x,1$ give the necessary and sufficient [Riccati equation](../../../analysis.md#riccati-equation) system

$$
\boxed{
\begin{aligned}
i\hbar\dot F&=\frac{2\hbar^2}{m}F^2-\frac12m\omega^2,\\
i\hbar\dot G&=\frac{2\hbar^2}{m}FG,\\
i\hbar\frac{\dot N}{N}
&=\frac{\hbar^2}{m}F-\frac{\hbar^2}{2m}G^2.
\end{aligned}}
$$

<h3 id="14b/c">c</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/c/solution">Solution</h4>

↑ **Parent:** [C](#14b/c)

Put $u=a+i\omega t$. Then

$$
\dot F=i\omega A\,\operatorname{sech}^2u,
\qquad
\dot G=-i\omega
\sqrt{\frac{m\omega}{\hbar}}\,
\operatorname{sech}u\tanh u.
$$

The $G$ equation from part (b) is satisfied when

$$
\frac{2\hbar^2A}{m}=\hbar\omega,
$$

so

$$
\boxed{A=\frac{m\omega}{2\hbar}}.
$$

With this value, the $F$ equation follows from $\tanh^2u=1-\operatorname{sech}^2u$: both its constant and $\operatorname{sech}^2u$ coefficients agree. Thus the stated $F,G$ satisfy both shape equations; the remaining scalar equation determines the normalization factor $N(t)$.

<h3 id="14b/d">d</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/d/solution">Solution</h4>

↑ **Parent:** [D](#14b/d)

The [probability density](../../../quantum-mechanics.md#probability-density) is

$$
|\psi|^2
=|N|^2
\exp\left[-2\operatorname{Re}F\,x^2
+2\operatorname{Re}G\,x\right].
$$

Completing the square shows that, when $\operatorname{Re}F>0$,

$$
|\psi|^2
=C(t)\exp\left[
-2\operatorname{Re}F\,(x-h)^2
\right],
$$

where

$$
\boxed{h(t)=
\frac{\operatorname{Re}G(t)}
{2\operatorname{Re}F(t)}}.
$$

<h3 id="14b/e">e</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/e/solution">Solution</h4>

↑ **Parent:** [E](#14b/e)

Writing $\theta=\omega t$ and

$$
D=\cosh(2a)+\cos(2\theta),
$$

the supplied identities give

$$
\operatorname{Re}\tanh(a+i\theta)
=\frac{\sinh(2a)}D,
\qquad
\operatorname{Re}\operatorname{sech}(a+i\theta)
=\frac{2\cosh a\cos\theta}{D}.
$$

Using $A=m\omega/(2\hbar)$ in part (d),

$$
\boxed{
h(t)=
\sqrt{\frac{\hbar}{m\omega}}\,
\frac{\cos(\omega t)}{\sinh a}}.
$$

The peak executes [simple harmonic motion](../../../classical-mechanics.md#simple-harmonic-motion) about the origin with angular frequency $\omega$ and amplitude $\sqrt{\hbar/(m\omega)}/\sinh a$.

<h3 id="14b/f">f</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/f/solution">Solution</h4>

↑ **Parent:** [F](#14b/f)

At each fixed time, $|\psi(x,t)|^2$ is a bell-shaped [Gaussian](../../../probability-theory.md#normal-distribution) centred at $x=h(t)$, with width determined by $\operatorname{Re}F(t)>0$. Completing the square as in part (d) makes the density symmetric about $h(t)$. Therefore its position [expectation value](../../../quantum-mechanics.md#expectation-value) is

$$
\boxed{\langle\widehat x\rangle_\psi=h(t)}.
$$

The sketch is a Gaussian peak whose centre oscillates between the two turning positions found in part (e), while its width varies periodically through $\operatorname{Re}F(t)$.

## 15D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15d/a">a</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/a/solution">Solution</h4>

↑ **Parent:** [A](#15d/a)

For a coaxial Gaussian cylinder of radius $r$ and length $L$, symmetry makes the [electric field](../../../electromagnetism.md#electric-field) radial and constant on the curved surface. [Gauss's law](../../../electromagnetism.md#gauss-s-law) gives

$$
E(2\pi rL)=\frac{\lambda L}{\varepsilon_0},
$$

so

$$
\boxed{\mathbf E(r)=\frac{\lambda}{2\pi\varepsilon_0r}\,\mathbf e_r}.
$$

Since $\mathbf E=-\nabla\phi$, a potential relative to an arbitrary reference radius $r_0$ is

$$
\boxed{
\phi(r)=-\frac{\lambda}{2\pi\varepsilon_0}
\log\frac r{r_0}}.
$$

An infinite line charge has no finite convention $\phi(\infty)=0$.

<h3 id="15d/b">b</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/b/solution">Solution</h4>

↑ **Parent:** [B](#15d/b)

Take the wire at $(a,0)$ to carry $+\lambda$ and that at $(-a,0)$ to carry $-\lambda$. If

$$
r_+=\sqrt{(x-a)^2+y^2},
\qquad
r_-=\sqrt{(x+a)^2+y^2},
$$

then, up to one additive constant,

$$
\phi=\frac{\lambda}{2\pi\varepsilon_0}
\log\frac{r_-}{r_+}.
$$

Thus an [equipotential](../../../electromagnetism.md#equipotential) with $k=2\pi\varepsilon_0\phi/\lambda$ satisfies $r_-/r_+=e^k$. For $k\ne0$, completing the square gives the [Apollonius circle](../../../geometry-and-topology.md#circles-of-apollonius)

$$
\boxed{
\left(x-a\coth k\right)^2+y^2
=a^2\operatorname{csch}^2k}.
$$

Its centre is $(a\coth k,0)$ and its radius is $a/|\sinh k|$. Positive and negative values give nested circles around the positive and negative wires. The electric field is orthogonal to these circles and points from the positive wire toward the negative wire. For $\phi=0$, the limiting equipotential is the straight line $x=0$.

Direct superposition gives

$$
\mathbf E
=\frac{\lambda}{2\pi\varepsilon_0}
\left[
\frac{(x-a,y)}{(x-a)^2+y^2}
-\frac{(x+a,y)}{(x+a)^2+y^2}
\right].
$$

In the limit $a\to0$ with $\lambda a=p$, the potential and field become those of a two-dimensional [electric dipole](../../../electromagnetism.md#electric-dipole):

$$
\boxed{\phi\longrightarrow
\frac{p}{\pi\varepsilon_0}\frac{x}{x^2+y^2}},
$$

and

$$
\boxed{
\mathbf E\longrightarrow
\frac{p}{\pi\varepsilon_0(x^2+y^2)^2}
\bigl(x^2-y^2,\,2xy\bigr)}.
$$

## 16C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16c/a">a</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/a/solution">Solution</h4>

↑ **Parent:** [A](#16c/a)

For the steady, fully developed ansatz $\mathbf u=w(r)\mathbf e_z$, both $\partial_t\mathbf u$ and $(\mathbf u\cdot\nabla)\mathbf u$ vanish. The axial [Navier-Stokes equation](../../../viscous-fluid-flow.md#navier-stokes-equation) reduces to

$$
0=-\frac{\partial p}{\partial z}
+\mu\frac1r\frac d{dr}\left(r\frac{dw}{dr}\right).
$$

Two integrations give

$$
w(r)=\frac1{4\mu}\frac{\partial p}{\partial z}r^2
+C_1\log r+C_2.
$$

Regularity at the axis forces $C_1=0$, and the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) $w(R)=0$ gives the [Hagen-Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation)

$$
\boxed{
w(r)=-\frac1{4\mu}\frac{\partial p}{\partial z}
(R^2-r^2)}.
$$

For flow in the positive $z$ direction, $\partial p/\partial z<0$.

<h3 id="16c/b">b</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/b/solution">Solution</h4>

↑ **Parent:** [B](#16c/b)

The net axial pressure force on a length-$L$ fluid cylinder is

$$
F_p
=\pi R^2[p(z_0)-p(z_0+L)]
=-\pi R^2L\frac{\partial p}{\partial z}.
$$

From part (a),

$$
\mu w'(R)=\frac R2\frac{\partial p}{\partial z}.
$$

Multiplying this wall shear stress by the lateral area $2\pi RL$ gives

$$
F_{\rm wall}
=2\pi RL\,\mu w'(R)
=\pi R^2L\frac{\partial p}{\partial z}.
$$

Consequently

$$
\boxed{F_p+F_{\rm wall}=0},
$$

which is the required steady force balance.

<h3 id="16c/c">c</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/c/solution">Solution</h4>

↑ **Parent:** [C](#16c/c)

The [mass flux](../../../physics.md#mass-flux) is density times the volume flux:

$$
\begin{aligned}
\dot M
&=\rho\int_0^{2\pi}\int_0^R w(r)\,r\,dr\,d\theta\\
&=-\frac{\rho\pi R^4}{8\mu}\frac{\partial p}{\partial z}.
\end{aligned}
$$

Thus

$$
\boxed{\dot M
=-\frac{\rho\pi R^4}{8\mu}\frac{\partial p}{\partial z}}.
$$

## 17C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17c/a">a</h3>

↑ **Parent:** [17C](#17c)

<h4 id="17c/a/solution">Solution</h4>

↑ **Parent:** [A](#17c/a)

If the bound is to hold for all $f\in C^3[-1,1]$, the error functional must annihilate every polynomial of degree at most two, because such a polynomial has $f'''=0$. Applying it to $1,x,x^2$ gives

$$
\begin{aligned}
a_{-1}+a_0+a_1&=0,\\
-a_{-1}+a_1&=0,\\
a_{-1}+a_1&=2.
\end{aligned}
$$

Therefore

$$
\boxed{a_{-1}=1,\qquad a_0=-2,\qquad a_1=1},
$$

so $\eta(f)=f(-1)-2f(0)+f(1)$ is the [central finite difference](../../../finite-difference.md#central-finite-difference) approximation.

<h3 id="17c/b">b</h3>

↑ **Parent:** [17C](#17c)

<h4 id="17c/b/solution">Solution</h4>

↑ **Parent:** [B](#17c/b)

The [Peano kernel theorem](../../../numerical-analysis.md#peano-kernel-theorem) says that if a continuous linear functional $L$ annihilates polynomials of degree below $m$, then

$$
L(f)=\int_a^bK(t)f^{(m)}(t)\,dt,
\qquad
K(t)=L\left(\frac{(x-t)_+^{m-1}}{(m-1)!}\right).
$$

Here $m=3$ and

$$
L(f)=f''(0)-f(-1)+2f(0)-f(1).
$$

Applying $L$ to $(x-t)_+^2/2$ gives

$$
K(t)=
\begin{cases}
\frac12(1+t)^2,&-1\leq t<0,\\
-\frac12(1-t)^2,&0\leq t\leq1.
\end{cases}
$$

Hence

$$
|L(f)|
\leq\|f'''\|_\infty\int_{-1}^1|K(t)|\,dt
=\frac13\|f'''\|_\infty.
$$

The smallest candidate is therefore

$$
\boxed{c=\frac13}.
$$

<h3 id="17c/c">c</h3>

↑ **Parent:** [17C](#17c)

<h4 id="17c/c/solution">Solution</h4>

↑ **Parent:** [C](#17c/c)

The constant is sharp because continuous functions bounded by one can approximate $\operatorname{sgn}K$ arbitrarily closely outside an arbitrarily small interval around zero. Choose $f'''$ to be such an approximation and integrate three times to obtain $f\in C^3[-1,1]$. Then

$$
\frac{|L(f)|}{\|f'''\|_\infty}
=\frac{\left|\int K(t)f'''(t)\,dt\right|}
{\|f'''\|_\infty}
\longrightarrow\int_{-1}^1|K(t)|\,dt=\frac13.
$$

**No smaller constant can therefore satisfy the inequality for every $f$.**

## 18H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

Let

$$
d_t=\#\{i:X_i=t\},
\qquad
r_t=\#\{i:X_i\geq t\}
=n-\sum_{s<t}d_s.
$$

Thus $d_t$ patients recover during month $t$, while $r_t-d_t$ survive that month without recovery. The [likelihood function](../../../statistical-modelling.md#likelihood-function) is

$$
\boxed{
L(q_1,\ldots,q_T)
=\prod_{t=1}^T
q_t^{d_t}(1-q_t)^{r_t-d_t}}.
$$

The independent $\operatorname{Beta}(T,1)$ prior densities are proportional to $q_t^{T-1}$. [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy) therefore leaves the coordinates posteriorly independent, with

$$
\boxed{
q_t\mid X
\sim\operatorname{Beta}
\bigl(T+d_t,\ 1+r_t-d_t\bigr)}.
$$

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

The probability of no recovery through month $M$ is the product of the conditional survival probabilities, so

$$
\boxed{\gamma=1-\prod_{t=1}^M(1-q_t)}.
$$

Under [quadratic loss](../../../statistical-inference.md#bayes-estimator-under-squared-error-loss), the [Bayes estimator](../../../statistical-inference.md#bayes-estimator) is the posterior mean. Posterior independence and the mean of a [Beta distribution](../../../probability-theory.md#beta-distribution) give

$$
\mathbb E[1-q_t\mid X]
=\frac{1+r_t-d_t}{T+1+r_t}.
$$

Consequently

$$
\boxed{
\widehat\gamma_B
=1-\prod_{t=1}^M
\frac{1+r_t-d_t}{T+1+r_t}}.
$$

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

The posterior expected loss at decision $\delta$ is

$$
R(\delta)
=2\int_{\gamma\leq\delta}(\delta-\gamma)\,dF(\gamma)
+\int_{\gamma>\delta}(\gamma-\delta)\,dF(\gamma).
$$

At continuity points its derivative is

$$
R'(\delta)=2F(\delta)-[1-F(\delta)]
=3F(\delta)-1.
$$

Thus the risk is minimized at a posterior one-third [quantile](../../../probability-theory.md#quantile-function):

$$
\boxed{
\widehat\gamma_B=F^{-1}\left(\frac13\right)}.
$$

More generally, any $\delta$ satisfying

$$
F(\delta-)\leq\frac13\leq F(\delta)
$$

is optimal. The quantile lies below the posterior median, reflecting the smaller penalty assigned to underestimation.

## 19H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

Let $D,E,F$ be the midpoints of $AB,AC,BC$. Write

$$
a=\mathbb E_A T_{BC},\qquad
d=\mathbb E_D T_{BC}=\mathbb E_E T_{BC},\qquad
f=\mathbb E_F T_{BC}.
$$

[First-step analysis](../../../analysis.md#first-step-analysis) for the [simple random walk](../../../markov-process.md#simple-random-walk) gives

$$
a=1+d,
$$

because $A$ has neighbours $D,E$;

$$
d=1+\frac{a+d+f}{4},
$$

because $D$ has neighbours $A,B,E,F$; and

$$
f=1+\frac d2,
$$

because $F$ has neighbours $B,C,D,E$. Solving,

$$
d=4,\qquad f=3,\qquad
\boxed{\mathbb E_A T_{BC}=a=5}.
$$

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/solution">Solution</h4>

↑ **Parent:** [B](#19h/b)

View each of the three level-one triangles in $G_2$ as a copy of $G_1$. Observe the walk only when it moves from one corner of such a copy to a different corner. By symmetry, the next of the two other corners is equally likely, so this embedded chain is the simple random walk on the coarse graph $G_1$. Part (a) says it makes an expected five coarse transitions before reaching $B$ or $C$.

Within each level-one copy, the mean time for one coarse transition is again five by part (a). The [Strong Markov property](../../../markov-process.md#strong-markov-property) at successive coarse-corner hitting times therefore gives

$$
\boxed{\mathbb E_A T_{BC}=5\cdot5=5^2=25}.
$$

<h3 id="19h/c">c</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/c/solution">Solution</h4>

↑ **Parent:** [C](#19h/c)

Let

$$
H_n=\mathbb E_A T_{BC}
$$

for the walk on $G_n$. Decompose $G_n$ into its three outer copies of $G_{n-1}$ and trace the walk only when it passes between distinct corner vertices of these copies. The [self-similarity](../../../geometry-and-topology.md#self-similarity) and reflection symmetry of the Sierpinski graph make this trace the simple random walk on $G_1$. It requires an expected five transitions to hit the two target outer corners.

Each coarse transition is an excursion across a copy of $G_{n-1}$ and has mean duration $H_{n-1}$. Applying the strong Markov property at the coarse stopping times gives

$$
H_n=5H_{n-1}.
$$

Since $H_1=5$, induction yields

$$
\boxed{\mathbb E_A T_{BC}=H_n=5^n}.
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
