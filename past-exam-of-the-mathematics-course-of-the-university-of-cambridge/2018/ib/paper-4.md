# Paper 4

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperib_4_2018.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperib_4_2018.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2G](#2g)
  - [a](#2g/a)
    - [Solution](#2g/a/solution)
  - [b](#2g/b)
    - [Solution](#2g/b/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4F](#4f)
  - [a](#4f/a)
    - [Solution](#4f/a/solution)
  - [b](#4f/b)
    - [Solution](#4f/b/solution)
- [5A](#5a)
  - [Solution](#5a/solution)
- [6B](#6b)
  - [Solution](#6b/solution)
- [7C](#7c)
  - [Solution](#7c/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9H](#9h)
  - [a](#9h/a)
    - [Solution](#9h/a/solution)
  - [b](#9h/b)
    - [Solution](#9h/b/solution)
  - [c](#9h/c)
    - [Solution](#9h/c/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11G](#11g)
  - [a](#11g/a)
    - [Solution](#11g/a/solution)
  - [b](#11g/b)
    - [Solution](#11g/b/solution)
  - [c](#11g/c)
    - [Solution](#11g/c/solution)
- [12F](#12f)
  - [a](#12f/a)
    - [Solution](#12f/a/solution)
  - [b](#12f/b)
    - [i](#12f/b/i)
      - [Solution](#12f/b/i/solution)
    - [ii](#12f/b/ii)
      - [Solution](#12f/b/ii/solution)
- [13E](#13e)
  - [i](#13e/i)
    - [Solution](#13e/i/solution)
  - [ii](#13e/ii)
    - [Solution](#13e/ii/solution)
- [14A](#14a)
  - [a](#14a/a)
    - [Solution](#14a/a/solution)
  - [b](#14a/b)
    - [Solution](#14a/b/solution)
- [15G](#15g)
  - [Solution](#15g/solution)
- [16B](#16b)
  - [a](#16b/a)
    - [Solution](#16b/a/solution)
  - [b](#16b/b)
    - [Solution](#16b/b/solution)
- [17C](#17c)
  - [Solution](#17c/solution)
- [18D](#18d)
  - [Solution](#18d/solution)
- [19H](#19h)
  - [Solution](#19h/solution)
- [20H](#20h)
  - [Solution](#20h/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

A [quadratic form](../../../linear-algebra.md#quadratic-form) on a finite-dimensional real [vector space](../../../vector-space.md) $V$ is a function $q(v)=B(v,v)$ for some symmetric [bilinear form](../../../linear-algebra.md#bilinear-form) $B$. A [positive-definite quadratic form](../../../linear-algebra.md#positive-definite-quadratic-form) satisfies $q(v)>0$ for every $v\ne0$.

Completing squares gives

$$
x^2+2xy+2y^2+2yz+3z^2=(x+y)^2+(y+z)^2+2z^2.
$$

Set $u=x+y$, $v=y+z$, $w=z$. The corresponding ordered basis in the original coordinates is

$$
\boxed{(1,0,0),\ (-1,1,0),\ (1,-1,1),}
$$

and the diagonal form is $u^2+v^2+2w^2$. All diagonal coefficients are positive, so **the form is positive definite**.

## 2G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2g/a">a</h3>

↑ **Parent:** [2G](#2g)

<h4 id="2g/a/solution">Solution</h4>

↑ **Parent:** [A](#2g/a)

Use the presentation $D_6=\langle r,s:r^3=s^2=1, srs=r^{-1}\rangle$. Its subgroup $\langle r\rangle$ is the unique subgroup of order $3$, hence is a [characteristic subgroup](../../../algebra.md#characteristic-subgroup). An [automorphism](../../../algebra.md#automorphism) must send $r$ to $r$ or $r^{-1}$ and $s$ to one of the three reflections $r^js$. Thus there are at most six automorphisms.

The [center of a group](../../../group-theory.md#center-of-a-group) of $D_6$ is trivial, so conjugation embeds $D_6$ as a group of six [inner automorphisms](../../../group-theory.md#inner-automorphism). These exhaust the possibilities. Hence **every automorphism of $D_6$ is inner**.

<h3 id="2g/b">b</h3>

↑ **Parent:** [2G](#2g)

<h4 id="2g/b/solution">Solution</h4>

↑ **Parent:** [B](#2g/b)

Let $D_8=\langle r,s:r^4=s^2=1, srs=r^{-1}\rangle$, the symmetry group of a square. The map

$$
r\mapsto r,\qquad s\mapsto rs
$$

preserves the relations and is an automorphism. Conjugation by a rotation sends $s$ to $r^{2j}s$, while conjugation by a reflection also inverts $r$. Therefore no conjugation fixes $r$ and sends $s$ to $rs$. This is an **outer automorphism of the nonabelian group $D_8$**.

## 3F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) in $\mathbb R$ says that every bounded real sequence has a convergent subsequence. For a bounded sequence in $\mathbb R^n$, successively extract subsequences on which the first, second, and so on through the $n$th coordinate converge. The final diagonal subsequence converges in [Euclidean space](../../../functional-analysis.md#euclidean-norm), proving the theorem in $\mathbb R^n$.

Put $K=D\setminus\bigcup_{z\in S}B_\varepsilon(z)$. Suppose the asserted $\delta$ did not exist. Then there would be $x_k\in D$ and $y_k\in K$ with $\|x_k-y_k\|<1/k$ but $|f(x_k)-f(y_k)|\geq\varepsilon$. Since $K$ is closed and bounded, Bolzano-Weierstrass gives a subsequence $y_k\to y\in K$, and then $x_k\to y$. The point $y$ is not in $S$, because otherwise $y\in B_\varepsilon(y)$, so $f$ has [continuity](../../../calculus.md#continuous-function) at $y$. Both $f(x_k)$ and $f(y_k)$ tend to $f(y)$, a contradiction. Hence the required **uniform $\delta>0$ exists**.

## 4F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4f/a">a</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/a/solution">Solution</h4>

↑ **Parent:** [A](#4f/a)

The [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) and its differentiated form are

$$
f(a)=\frac1{2\pi i}\oint_C\frac{f(z)}{z-a}\,dz,
\qquad
f'(a)=\frac1{2\pi i}\oint_C\frac{f(z)}{(z-a)^2}\,dz.
$$

If $f$ is entire and $|f|\leq M$, the [Cauchy estimate](../../../analysis.md#cauchy-estimate) gives $|f'(a)|\leq M/\rho$. Letting $\rho\to\infty$ yields $f'(a)=0$ for every $a$. Thus **$f$ is constant**, which is [Liouville theorem](../../../complex-analysis.md#liouville-theorem).

<h3 id="4f/b">b</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/b/solution">Solution</h4>

↑ **Parent:** [B](#4f/b)

The inequality implies $u(u-1)\geq v^2\geq0$, so $u\leq0$ or $u\geq1$. Since $u$ is continuous and $\mathbb C$ is [connected](../../../geometry-and-topology.md#connected-space), its image lies wholly in one of these intervals. If $u\geq1$, then $g$ has no zero and $|1/g|\leq1$; [Liouville theorem](../../../complex-analysis.md#liouville-theorem) makes $1/g$, hence $g$, constant. If $u\leq0$, then $|g-1|\geq1$, so the same argument applied to $1/(g-1)$ proves that **$g$ is constant**.

## 5A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5a/solution">Solution</h3>

↑ **Parent:** [5A](#5a)

[Separation of variables](../../../partial-differential-equation.md#separation-of-variables) with $u=X(x)Y(y)$ and the three homogeneous boundary conditions gives $X_n=\sin(n\pi x)$ and $Y_n=\sinh(n\pi y)$. The boundary value at $y=1$ contains only the third [Fourier sine series](../../../fourier-series.md#fourier-sine-series) mode. Therefore

$$
\boxed{u(x,y)=2\frac{\sinh(3\pi y)}{\sinh(3\pi)}\sin(3\pi x).}
$$

This [harmonic function](../../../partial-differential-equation.md#harmonic-function) has all four prescribed boundary values.

## 6B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6b/solution">Solution</h3>

↑ **Parent:** [6B](#6b)

The [Born rule](../../../quantum-mechanics.md#born-rule) and [probability current](../../../quantum-mechanics.md#probability-current) in one dimension give

$$
\rho=|\Psi|^2,
\qquad
j=\frac{\hbar}{2mi}\left(\Psi^*\Psi_x-\Psi\Psi_x^*\right).
$$

Multiply the [Time-dependent Schrödinger equation](../../../physics.md#time-dependent-schrodinger-equation) by $\Psi^*$, subtract its complex conjugate multiplied by $\Psi$, and rearrange to obtain the [continuity equation](../../../physics.md#continuity-equation) $\rho_t+j_x=0$.

For the stated superposition, the interference terms in $j$ are real and cancel from its imaginary part. Hence

$$
\boxed{j=\frac{\hbar k}{m}\left(|A|^2-|B|^2\right),}
$$

independent of $x$ and $t$.

## 7C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7c/solution">Solution</h3>

↑ **Parent:** [7C](#7c)

Taking the [divergence](../../../calculus.md#divergence) of the [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) and using the [Gauss's law](../../../electromagnetism.md#gauss-s-law) $\nabla\cdot E=\rho/\varepsilon_0$ gives

$$
0=\mu_0\nabla\cdot J+\mu_0\frac{\partial\rho}{\partial t},
$$

which is [charge conservation from Maxwell equations](../../../electromagnetism.md#charge-conservation-from-maxwell-equations) $\rho_t+\nabla\cdot J=0$.

By [Ohm's law](../../../electromagnetism.md#ohm-s-law), $J=\sigma E$, so $\nabla\cdot J=\sigma\rho/\varepsilon_0$. Therefore

$$
\boxed{\rho(t)=\rho(0)e^{-\sigma t/\varepsilon_0},}
$$

with charge-relaxation rate $\sigma/\varepsilon_0$ and time $\varepsilon_0/\sigma$.

## 8D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

[Gaussian elimination](../../../numerical-analysis.md#gaussian-elimination) without pivoting gives

$$
A=LU,
\quad
L=\begin{pmatrix}1&0&0&0\\2&1&0&0\\1&3&1&0\\2&2&2&1\end{pmatrix},
\quad
U=\begin{pmatrix}1&2&1&2\\0&1&3&2\\0&0&3&6\\0&0&0&\lambda-20\end{pmatrix}.
$$

Thus $\det A=3(\lambda-20)$ and the solution is unique exactly when **$\lambda\ne20$**.

For $\lambda=20$, [forward substitution in a triangular system](../../../linear-algebra.md#forward-substitution-in-a-triangular-system) in $Ly=b$ gives $y=(1,1,3,\mu-10)^T$. Consistency of $Ux=y$ requires $\boxed{\mu=10}$. [backward substitution in a triangular system](../../../linear-algebra.md#backward-substitution-in-a-triangular-system) then gives

$$
\boxed{x=(4-8t,\ 4t-2,\ 1-2t,\ t)^T,\qquad t\in\mathbb R.}
$$

## 9H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9h/a">a</h3>

↑ **Parent:** [9H](#9h)

<h4 id="9h/a/solution">Solution</h4>

↑ **Parent:** [A](#9h/a)

A distribution $\pi$ is an [invariant distribution](../../../markov-process.md#stationary-distribution) when

$$
\pi_j=\sum_{i\in S}\pi_i p_{ij}
$$

for every $j$, equivalently $\pi P=\pi$.

<h3 id="9h/b">b</h3>

↑ **Parent:** [9H](#9h)

<h4 id="9h/b/solution">Solution</h4>

↑ **Parent:** [B](#9h/b)

[Detailed balance](../../../markov-process.md#detailed-balance) means $\pi_i p_{ij}=\pi_jp_{ji}$ for all $i,j$. Summing over $i$ gives

$$
\sum_i\pi_i p_{ij}=\pi_j\sum_i p_{ji}=\pi_j,
$$

so **detailed balance implies invariance**.

<h3 id="9h/c">c</h3>

↑ **Parent:** [9H](#9h)

<h4 id="9h/c/solution">Solution</h4>

↑ **Parent:** [C](#9h/c)

Let $D_i$ be the [degree of a vertex](../../../graph-theory.md#degree-graph-theory) and put

$$
\pi_i=\frac{D_i}{\sum_kD_k}.
$$

If $i$ and $j$ are adjacent, then $\pi_ip_{ij}=1/\sum_kD_k=\pi_jp_{ji}$; if they are not adjacent, both sides vanish. Thus the walk is in detailed balance, and its invariant distribution is **proportional to vertex degree**.

## 10E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

A [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) $T$ satisfies $\langle Tx,y\rangle=\langle x,Ty\rangle$. If $Tx=\lambda x$, then $\lambda\langle x,x\rangle=\langle Tx,x\rangle=\langle x,Tx\rangle=\overline\lambda\langle x,x\rangle$, so $\lambda\in\mathbb R$. An eigenvector exists over $\mathbb C$; its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) is $T$-invariant. Induction on dimension produces an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of eigenvectors, proving the [finite-dimensional spectral theorem](../../../linear-operator-theory.md#finite-dimensional-spectral-theorem).

A self-adjoint $T$ is positive definite exactly when every eigenvalue is positive, since $\langle Tx,x\rangle=\sum_i\lambda_i|x_i|^2$ in an eigenbasis. The quadratic forms of two positive-definite operators add, so their sum is positive definite.

The same eigenbasis shows that $\operatorname{spec}T\subset[a,b]$ exactly when $T-\lambda I$ is positive definite for every $\lambda<a$ and negative definite for every $\lambda>b$. Finally, if $v$ is a unit eigenvector of $\alpha+\beta$ with eigenvalue $\gamma$, the [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) bounds give

$$
\gamma=\langle\alpha v,v\rangle+\langle\beta v,v\rangle\in[a+c,b+d].
$$

Thus **every eigenvalue of $\alpha+\beta$ lies in $[a+c,b+d]$**.

## 11G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11g/a">a</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/a/solution">Solution</h4>

↑ **Parent:** [A](#11g/a)

The [structure theorem for finitely generated modules over a principal ideal domain](../../../module-theory.md#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain) says that a finitely generated module over a Euclidean domain $R$ is

$$
R^r\oplus R/(d_1)\oplus\cdots\oplus R/(d_k),
\qquad d_1\mid d_2\mid\cdots\mid d_k,
$$

with the rank and nonunit [invariant factors of a linear operator](../../../linear-operator-theory.md#invariant-factors-of-a-linear-operator) unique up to associates.

<h3 id="11g/b">b</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/b/solution">Solution</h4>

↑ **Parent:** [B](#11g/b)

Make $F^n$ an $F[X]$-module by $Xv=Av$. It is finitely generated and torsion, so the structure theorem gives cyclic summands $F[X]/(d_i)$ with $d_1\mid\cdots\mid d_k$. In the power basis of each summand, multiplication by $X$ has the [companion matrix](../../../linear-operator-theory.md#companion-matrix) of $d_i$. Their block diagonal sum is the **rational canonical form**, unique because the invariant factors are unique.

<h3 id="11g/c">c</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/c/solution">Solution</h4>

↑ **Parent:** [C](#11g/c)

The [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is $(t-\tfrac12)^3$. For $N=A-\tfrac12I$, one finds $N\ne0$ but $N^2=0$, so the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) is $(t-\tfrac12)^2$. Hence the invariant factors are $t-\tfrac12$ and $(t-\tfrac12)^2$, and the rational canonical form is

$$
\boxed{\begin{pmatrix}
\tfrac12&0&0\\
0&0&-\tfrac14\\
0&1&1
\end{pmatrix}.}
$$

## 12F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/solution">Solution</h4>

↑ **Parent:** [A](#12f/a)

A [complete metric space](../../../topological-analysis.md#complete-metric-space) is one in which every [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) converges. On $I=(0,1]$ define

$$
d(x,y)=|x^{-1}-y^{-1}|.
$$

The map $x\mapsto1/x$ is an [isometry](../../../riemannian-geometry.md#isometry) from $(I,d)$ onto the closed subset $[1,\infty)$ of $\mathbb R$, so $d$ is a metric and is complete. That map and its inverse are continuous in the ordinary Euclidean metrics, so it is also a [homeomorphism](../../../topology.md#homeomorphism). Therefore $d$ induces exactly the usual subspace topology on $I$.

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/i">i</h4>

↑ **Parent:** [B](#12f/b)

<h5 id="12f/b/i/solution">Solution</h5>

↑ **Parent:** [I](#12f/b/i)

If $Y$ is closed and $(y_n)$ is Cauchy in $Y$, completeness of $X$ gives $y_n\to y\in X$, and closedness gives $y\in Y$. Conversely, if $Y$ is complete and $y$ lies in its closure, choose $y_n\in Y$ with $d(y_n,y)<1/n$. This sequence is Cauchy, so it converges in $Y$; uniqueness of limits makes its limit $y$. Thus **$Y$ is complete exactly when it is closed in $X$**.

<h4 id="12f/b/ii">ii</h4>

↑ **Parent:** [B](#12f/b)

<h5 id="12f/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12f/b/ii)

Choose $x\in X$ and iterate $x_{n+1}=f(x_n)$. The [contraction mapping](../../../analysis.md#contraction-mapping) estimate

$$
d(x_{n+1},x_n)\leq\lambda^nd(x_1,x_0)
$$

makes $(x_n)$ Cauchy by a [geometric series](../../../real-analysis.md#geometric-series). Its limit $x_0$ satisfies $f(x_0)=x_0$ because $f$ is Lipschitz. Two fixed points would satisfy $d(x_0,y_0)\leq\lambda d(x_0,y_0)$, so they coincide. This proves the [Banach fixed-point theorem](../../../analysis.md#contraction-mapping-theorem).

Now suppose the final assertion failed. There would be $m_k,n_k\to\infty$ with $f(a_{m_k})=a_{n_k}$. Since $a_n\to a$ and $f$ is continuous, the two sides tend respectively to $f(a)$ and $a$, so $f(a)=a$. Uniqueness would give $a=x_0$, a contradiction. Hence the required **$\ell$ and $m$ exist**.

## 13E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="13e/i">i</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/i/solution">Solution</h4>

↑ **Parent:** [I](#13e/i)

Since $U_m\cap U_n=U_{\gcd(m,n)}$ when the greatest common divisor is at least $2$, and is empty otherwise, finite intersections of the $U_n$ are again among the allowed unions. Arbitrary unions are built into the definition; the empty union is empty, and $X=\bigcup_{n\in X}U_n$. Thus these sets form a [topology](../../../topology.md).

The space is **not Hausdorff**: every neighborhood of $4$ contains its divisor $2$, and every neighborhood of $2$ contains $2$, so $2$ and $4$ cannot have disjoint neighborhoods.

<h3 id="13e/ii">ii</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#13e/ii)

The cover $X=\bigcup_{n\in X}U_n$ has no finite subcover, because every $U_n$ is finite. Hence **$X$ is not compact**.

For the stated [pasting lemma for closed subspaces](../../../topology.md#pasting-lemma-for-closed-subspaces), if $C\subset Z$ is closed, then

$$
f^{-1}(C)=(A\cap f^{-1}(C))\cup(B\cap f^{-1}(C))
$$

is a union of two closed subsets of $Y$; therefore $f$ is continuous.

For $m,n\in X$, let $q=mn$. On $[0,\tfrac12]$ define a path equal to $m$ before the endpoint and equal to $q$ at the endpoint; it is continuous because every open set containing $q$ also contains its divisor $m$. On $[\tfrac12,1]$ define it to equal $q$ at the first endpoint and $n$ thereafter. This is likewise continuous. The two closed-interval paths agree at $1/2$, so the pasting lemma joins them into a path from $m$ to $n$. Thus **$X$ is path-connected**.

## 14A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="14a/a">a</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/a/solution">Solution</h4>

↑ **Parent:** [A](#14a/a)

The [Laplace transform](../../../analysis.md#laplace-transform) is

$$
\mathcal L[y](s)=\frac1{\sqrt\pi}\int_0^\infty t^{-1/2}\exp\left(-st-\frac{a^2}{4t}\right)dt.
$$

Using the supplied Gaussian integral after $t=x^2$ gives

$$
\boxed{\mathcal L[y](s)=\frac{e^{-|a|\sqrt s}}{\sqrt s}.}
$$

<h3 id="14a/b">b</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/b/solution">Solution</h4>

↑ **Parent:** [B](#14a/b)

Taking the Laplace transform in $t$ gives

$$
U_{xx}-sU=-f(x).
$$

The bounded resolvent solution supplied in the hint can be written

$$
U(x,s)=\int_{-\infty}^{\infty}\frac{e^{-\sqrt s|x-\xi|}}{2\sqrt s}f(\xi)\,d\xi.
$$

Part (a) inverts the kernel, yielding the [heat kernel](../../../diffusion-equation.md#heat-kernel)

$$
\boxed{K(|x-\xi|,t)=\frac1{\sqrt{4\pi t}}\exp\left(-\frac{(x-\xi)^2}{4t}\right).}
$$

## 15G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="15g/solution">Solution</h3>

↑ **Parent:** [15G](#15g)

Differentiate the [parametrized surface](../../../calculus.md#parametrized-surface). The coefficients of the [first fundamental form](../../../differential-geometry.md#first-fundamental-form) simplify to

$$
E=Q^2+\frac{v^2}{4},\qquad F=0,\qquad G=1.
$$

If $c=\sigma_u\times\sigma_v$, then $|c|^2=E$. Moreover

$$
\sigma_{uv}\mathbin{\cdot}c=1,
\qquad
\sigma_{vv}\mathbin{\cdot}c=0.
$$

Thus the second-fundamental-form coefficients satisfy $M=1/\sqrt E$ and $N=0$. The [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) is consequently

$$
\boxed{K=\frac{LN-M^2}{EG-F^2}=-\frac1{E^2}=-\frac1{(v^2/4+Q^2)^2}.}
$$

## 16B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="16b/a">a</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/a/solution">Solution</h4>

↑ **Parent:** [A](#16b/a)

The [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) are $\ddot x+\omega^2x=0$ and $\ddot y+\omega^2y=0$. They imply

$$
\dot J=\ddot xy-\ddot yx=0.
$$

Writing

$$
x=A\cos\omega t+B\sin\omega t,
\qquad y=C\cos\omega t+D\sin\omega t,
$$

gives the conserved value

$$
\boxed{J=\omega(BC-AD).}
$$

<h3 id="16b/b">b</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/b/solution">Solution</h4>

↑ **Parent:** [B](#16b/b)

The equations are

$$
\ddot x+\alpha x^3+\beta xy^2=0,
\qquad
\ddot y+\alpha y^3+\beta x^2y=0.
$$

Hence

$$
\dot J=(\beta-\alpha)xy(x^2-y^2),
$$

which is not generally zero. Conservation requires **$\beta/\alpha=1$**. Then the potential is $\alpha(x^2+y^2)^2/4$, so the action has [rotational symmetry](../../../linear-algebra.md#rotational-symmetry). By [Noether's theorem](../../../calculus-of-variations.md#noether-conserved-quantity-for-a-mechanical-point-symmetry), $J$ is the conserved angular momentum, up to the sign convention used in its definition.

## 17C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="17c/solution">Solution</h3>

↑ **Parent:** [17C](#17c)

Remove a small disc about $x$ and apply [Green second identity](../../../partial-differential-equation.md#green-second-identity) to $u(x_0)$ and $G_0(x;x_0)$. Since $\nabla_{x_0}^2G_0=\delta(x_0-x)$ and $\nabla^2u=-\rho$, the shrinking inner boundary contributes $u(x)$ and gives

$$
u(x)=-\int_\Omega G_0(x;x_0)\rho(x_0)\,dx_0dy_0
+\oint_{\partial\Omega}\left(u\,\partial_nG_0-G_0\partial_nu\right)ds.
$$

For the unit disc, the [method of images](../../../mathematics.md#method-of-images) gives the [Dirichlet Green function](../../../analysis.md#dirichlet-green-function)

$$
G_D(x;x_0)=\frac1{2\pi}\log\frac{|x-x_0|}{|x_0|\,|x-x_0/|x_0|^2|},
$$

which vanishes on the boundary by the hinted identity. The boundary representation with $u(1,\theta_0)=\delta(\theta_0-\alpha)$ evaluates the normal derivative of $G_D$ at $\theta_0=\alpha$, giving the [Poisson kernel](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane)

$$
\boxed{u(r,\theta)=\frac1{2\pi}\frac{1-r^2}{1+r^2-2r\cos(\theta-\alpha)}.}
$$

## 18D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="18d/solution">Solution</h3>

↑ **Parent:** [18D](#18d)

Let $\phi$ be the [velocity potential](../../../fluid-mechanics.md#velocity-potential). The linearized deep-water equations are $\nabla^2\phi=0$ for $z<0$, $\eta_t=\phi_z$ and $\phi_t+g\eta=0$ at $z=0$, with zero normal velocity at the four side walls. The [normal modes](../../../wave-equation.md#normal-mode) are

$$
\phi=C e^{kz}\cos\frac{m\pi x}{a}\cos\frac{n\pi y}{a}e^{-i\omega t},
\quad
k=\frac\pi a\sqrt{m^2+n^2},
$$

where $m,n\geq0$ are not both zero. The free-surface conditions give the dispersion relation for a [deep-water gravity wave](../../../fluid-mechanics.md#deep-water-gravity-wave):

$$
\boxed{\omega^2=gk.}
$$

The initial displacement is the $(m,n)=(3,4)$ mode, so $k=5\pi/a$. Release from rest selects a cosine in time:

$$
\boxed{\eta=\varepsilon\cos\frac{3\pi x}{a}\cos\frac{4\pi y}{a}
\cos\left(\sqrt{\frac{5\pi g}{a}}\,t\right).}
$$

Velocity decays as $e^{kz}$, so it falls to $1/e$ of its surface value at depth **$a/(5\pi)$**.

## 19H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="19h/solution">Solution</h3>

↑ **Parent:** [19H](#19h)

With the uniform prior, the [binomial likelihood](../../../discrete-probability-distribution.md#binomial-likelihood) gives the [Beta distribution](../../../probability-theory.md#beta-distribution) posterior $\operatorname{Beta}(s+1,n-s+1)$. Under [squared-error loss](../../../statistical-inference.md#squared-error-loss), the [Bayes estimator](../../../statistical-inference.md#bayes-estimator) is the posterior mean:

$$
\boxed{\hat p_G=\frac{s+1}{n+2}.}
$$

The production manager's prior gives posterior density proportional to $p^{s+1}(1-p)^{n-s}$. Minimizing $\mathbb E[(1-p)(\hat p-p)^2\mid X=s]$ gives the weighted posterior mean

$$
\hat p_P=\frac{\mathbb E[p(1-p)\mid X=s]}{\mathbb E[1-p\mid X=s]}
=\boxed{\frac{s+2}{n+4}},
$$

using the supplied [beta function](../../../complex-analysis.md#beta-function). Cross multiplication shows $\hat p_P>\hat p_G$ exactly when $n>2s$, so it is greater unless **$s\geq n/2$**.

## 20H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="20h/solution">Solution</h3>

↑ **Parent:** [20H](#20h)

A cut is a partition $(S,T)$ of the vertices with the source in $S$ and sink in $T$; its capacity is the sum of capacities of directed edges from $S$ to $T$. The [max-flow min-cut theorem](../../../graph-theory.md#max-flow-min-cut-theorem) says that maximum flow value equals minimum cut capacity. With integral capacities, there is an [integral max-flow theorem](../../../graph-theory.md#integral-max-flow-theorem) attaining the maximum.

Construct a [bipartite graph](../../../graph-theory.md#bipartite-graph) with one vertex for each row and column and an edge $r_i\to c_j$ whenever $A_{ij}=1$. Add source-to-row and column-to-sink edges of capacity $1$, and give row-to-column edges infinite capacity. An integral flow is precisely a set of independent $1$s, so its maximum value is the largest such set.

A finite-capacity cut places some rows on the sink side and some columns on the source side; these lines cover every $1$, since an uncovered row-to-column edge would cross the cut with infinite capacity. Its capacity is the number of selected lines. Conversely every line cover defines such a cut. Max-flow min-cut therefore proves **the maximum number of independent $1$s equals the minimum number of covering lines**, the matrix form of [Kőnig's theorem for bipartite matching](../../../graph-theory.md#konig-s-theorem-graph-theory).

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
