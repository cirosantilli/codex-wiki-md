# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2002/PaperIB_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2002/PaperIB_2.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3H](#3h)
  - [Solution](#3h/solution)
- [4G](#4g)
  - [Solution](#4g/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6G](#6g)
  - [Solution](#6g/solution)
- [7B](#7b)
  - [Solution](#7b/solution)
- [8F](#8f)
  - [Solution](#8f/solution)
- [9D](#9d)
  - [Solution](#9d/solution)
- [10E](#10e)
  - [a](#10e/a)
    - [Solution](#10e/a/solution)
  - [b](#10e/b)
    - [Solution](#10e/b/solution)
  - [c](#10e/c)
    - [Solution](#10e/c/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12H](#12h)
  - [Solution](#12h/solution)
- [13G](#13g)
  - [a](#13g/a)
    - [Solution](#13g/a/solution)
    - [i](#13g/a/i)
      - [Solution](#13g/a/i/solution)
    - [ii](#13g/a/ii)
      - [Solution](#13g/a/ii/solution)
  - [b](#13g/b)
    - [Solution](#13g/b/solution)
  - [c](#13g/c)
    - [Solution](#13g/c/solution)
- [14B](#14b)
  - [a](#14b/a)
    - [Solution](#14b/a/solution)
  - [b](#14b/b)
    - [Solution](#14b/b/solution)
  - [c](#14b/c)
    - [Solution](#14b/c/solution)
  - [d](#14b/d)
    - [Solution](#14b/d/solution)
- [15G](#15g)
  - [a](#15g/a)
    - [Solution](#15g/a/solution)
  - [b](#15g/b)
    - [Solution](#15g/b/solution)
  - [c](#15g/c)
    - [Solution](#15g/c/solution)
  - [d](#15g/d)
    - [Solution](#15g/d/solution)
- [16B](#16b)
  - [a](#16b/a)
    - [Solution](#16b/a/solution)
  - [b](#16b/b)
    - [Solution](#16b/b/solution)
  - [c](#16b/c)
    - [Solution](#16b/c/solution)
- [17F](#17f)
  - [Solution](#17f/solution)
  - [i](#17f/i)
    - [Solution](#17f/i/solution)
  - [ii](#17f/ii)
    - [Solution](#17f/ii/solution)
  - [iii](#17f/iii)
    - [Solution](#17f/iii/solution)
  - [iv](#17f/iv)
    - [Solution](#17f/iv/solution)
- [18D](#18d)
  - [a](#18d/a)
    - [Solution](#18d/a/solution)
  - [b](#18d/b)
    - [Solution](#18d/b/solution)
  - [c](#18d/c)
    - [Solution](#18d/c/solution)

## 1E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

A [metric space](../../../topological-analysis.md#metric-space) is a [complete metric space](../../../topological-analysis.md#complete-metric-space) when every [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) converges to a point of that space. It is a [totally bounded space](../../../topological-analysis.md#totally-bounded-space) when, for every $\varepsilon>0$, finitely many open metric balls of radius $\varepsilon$ cover the space.

With their usual distances, **$\mathbb R$ is complete but not totally bounded**, and **$(0,1)$ is totally bounded but not complete**. The [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) $1/n$ in $(0,1)$ has its limit outside the space; no finite collection of balls of a fixed radius covers $\mathbb R$.

For the requested [continuous functions](../../../calculus.md#continuous-function), take

$$
f:\mathbb R\longrightarrow(0,\infty),\qquad f(x)=e^x,
$$

and

$$
g:(0,1)\longrightarrow(1,\infty),\qquad g(x)=\frac1x.
$$

Both are continuous and onto. The domain of $f$ is a [complete metric space](../../../topological-analysis.md#complete-metric-space), but its image is not complete because $1/n$ tends to the missing point $0$. The domain of $g$ is a [totally bounded space](../../../topological-analysis.md#totally-bounded-space), but its unbounded image is not totally bounded. Uniform continuity, unlike mere continuity, would preserve total boundedness.

## 2C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

Let $R_{ij}$ be the components of an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) relating two Cartesian frames by $v'_i=R_{ij}v_j$. Repeated indices are summed from $1$ to $3$. The [tensor component transformation law](../../../general-relativity.md#tensor-component-transformation-law) for a [Cartesian second-rank tensor](../../../linear-algebra.md#cartesian-second-rank-tensor) is

$$
\boxed{A'_{ij}=R_{ik}R_{j\ell}A_{k\ell}},\qquad A'=RAR^{\mathsf T}.
$$

For a proper [rotation](../../../riemannian-geometry.md#rotation-mathematics), $\det R=1$; the transformation law itself also holds for orthogonal changes of Cartesian frame with determinant $-1$.

To find a [cubically invariant second-rank tensor](../../../linear-algebra.md#cubically-invariant-second-rank-tensor), first square each of the prescribed quarter-turns. For example the half-turn about the first axis is $S_x=\operatorname{diag}(1,-1,-1)$. Invariance under $S_xAS_x^{\mathsf T}$ forces $A_{12},A_{13},A_{21},A_{31}$ to vanish. The corresponding half-turns about the other axes eliminate the remaining off-diagonal components, even though symmetry of $A$ was never assumed.

Now write $A=\operatorname{diag}(a,b,c)$. A quarter-turn about the third axis interchanges $a,b$, so $a=b$; a quarter-turn about the first axis gives $b=c$. Conversely a scalar multiple of the [identity matrix](../../../vector-space.md#identity-matrix) is invariant under every [rotation](../../../riemannian-geometry.md#rotation-mathematics). Thus the most general answer is

$$
\boxed{A_{ij}=a\delta_{ij}}.
$$

## 3H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3h/solution">Solution</h3>

↑ **Parent:** [3H](#3h)

Represent a possibly randomized [statistical test](../../../statistical-modelling.md#statistical-test) by a function $\varphi(Y)$ taking values in $[0,1]$, its conditional probability of rejection. Its [power function](../../../statistical-modelling.md#power-function-of-a-statistical-test) is $\pi(\rho)=\mathbb E_\rho\varphi(Y)$, and its [size of a statistical test](../../../statistical-modelling.md#size-of-a-statistical-test) is the supremum of this probability over the [null hypothesis](../../../statistical-modelling.md#null-hypothesis). At a prescribed [significance level](../../../statistical-modelling.md#significance-level) $\alpha$, a [uniformly most powerful test](../../../statistical-modelling.md#uniformly-most-powerful-test) has at least as much power as every other level-$\alpha$ test at every parameter in the alternative.

Put $S=\sum_{j=1}^nY_j$. For any fixed alternative $0<\rho_1<\rho_0$, the [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) is

$$
\frac{L(\rho_1)}{L(\rho_0)}=\left(\frac{\rho_1}{\rho_0}\right)^n e^{(\rho_0-\rho_1)S},
$$

which is strictly increasing in $S$. The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) therefore selects the upper tail $S>c_\alpha$. Its cutoff is determined solely by the null distribution, not by $\rho_1$, so the same [statistical test](../../../statistical-modelling.md#statistical-test) is most powerful against every allowed alternative and hence uniformly most powerful.

Under rate $\rho$, $S$ has a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape $n$ and rate $\rho$. For completeness, convolution starts with $\rho e^{-\rho s}$ and, if the $n$-term density is $\rho^ns^{n-1}e^{-\rho s}/(n-1)!$, convolving once more gives $\rho^{n+1}s^ne^{-\rho s}/n!$. Integrating this density by parts repeatedly gives its upper-tail probability. Consequently **reject precisely when $S>c_\alpha$**, where

$$
e^{-\rho_0c_\alpha}\sum_{j=0}^{n-1}\frac{(\rho_0c_\alpha)^j}{j!}=\alpha,
$$

and the [power function](../../../statistical-modelling.md#power-function-of-a-statistical-test) is

$$
\boxed{\pi(\rho)=e^{-\rho c_\alpha}\sum_{j=0}^{n-1}\frac{(\rho c_\alpha)^j}{j!}}.
$$

For $0<\alpha<1$ the continuous strictly decreasing null tail gives a unique positive cutoff, with exact size $\alpha$ and no boundary randomization.

## 4G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4g/solution">Solution</h3>

↑ **Parent:** [4G](#4g)

Use the [one-sided product bound for an entire function](../../../complex-analysis.md#one-sided-product-bound-for-an-entire-function) by considering

$$
F(z)=\exp[-if(z)^2].
$$

This is an [entire function](../../../complex-analysis.md#entire-function), and $f^2=(u^2-v^2)+2iuv$ gives $|F|=e^{2uv}$. If $uv\leq M$, then $|F|\leq e^{2M}$ everywhere. The [Liouville theorem](../../../complex-analysis.md#liouville-theorem) therefore makes $F$ constant.

Because an exponential never vanishes, differentiating yields $0=F'=-2iff'F$, and hence $(f^2)'=2ff'=0$. Thus $f^2$ is constant. If that constant is zero, $f=0$; otherwise $f$ takes values in the two square roots of one nonzero constant. Continuity on the [connected space](../../../geometry-and-topology.md#connected-space) $\mathbb C$ prevents switching between those two values. **Therefore $f$ is constant.**

## 5B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

Let $a_1,a_2,a_3$ denote the columns. The [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process) begins with $\|a_1\|=2$, so

$$
q_1=\frac12(1,1,1,1)^{\mathsf T},\qquad r_{11}=2.
$$

The second column has $r_{12}=q_1^{\mathsf T}a_2=4$ and residual

$$
a_2-4q_1=(-1,1,-1,1)^{\mathsf T}.
$$

This residual has norm $2$, giving $q_2=\tfrac12(-1,1,-1,1)^{\mathsf T}$ and $r_{22}=2$.

For the third column the [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) are $r_{13}=6$ and $r_{23}=4$. Subtracting them gives

$$
a_3-6q_1-4q_2=(1,1,-1,-1)^{\mathsf T}.
$$

Its norm is $2$, so $q_3=\tfrac12(1,1,-1,-1)^{\mathsf T}$ and $r_{33}=2$. Thus the requested thin [QR decomposition](../../../linear-algebra.md#qr-decomposition) is

$$
\boxed{Q=\frac12\begin{pmatrix}1&-1&1\\1&1&1\\1&-1&-1\\1&1&-1\end{pmatrix},\qquad R=\begin{pmatrix}2&4&6\\0&2&4\\0&0&2\end{pmatrix}}.
$$

The three displayed columns have pairwise zero [inner products](../../../linear-algebra.md#inner-product) and unit norms; direct multiplication gives $QR=A$.

## 6G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6g/solution">Solution</h3>

↑ **Parent:** [6G](#6g)

The [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) divides the annihilating polynomial $t^2(t-1)$, since $A^3-A^2=0$. Every nonconstant monic divisor can occur in dimension four: use [Jordan blocks](../../../linear-operator-theory.md#jordan-block) of sizes at most two at [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $0$ and of size one at [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $1$, adding scalar blocks as needed. The complete list is

$$
\boxed{t,\quad t^2,\quad t-1,\quad t(t-1),\quad t^2(t-1)}.
$$

For example the first four occur for $0$, $J_2(0)\oplus0\oplus0$, $I$, and $\operatorname{diag}(0,0,1,1)$, respectively; the final one occurs for $J_2(0)\oplus0\oplus1$.

Failure to be [diagonalizable](../../../linear-operator-theory.md#diagonalizable-matrix) requires a size-two [Jordan block](../../../linear-operator-theory.md#jordan-block) at zero. The condition $A^2\ne0$ requires at least one block at one, since every allowed zero block squares to zero. A size-two zero block and one scalar block at one leave only one dimension. It can carry zero or one. Thus, up to permutation of blocks, **the only possible [Jordan normal forms](../../../linear-operator-theory.md#jordan-normal-form) are**

$$
\boxed{J_2(0)\oplus[0]\oplus[1],\qquad J_2(0)\oplus[1]\oplus[1]},\qquad J_2(0)=\begin{pmatrix}0&1\\0&0\end{pmatrix}.
$$

## 7B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7b/solution">Solution</h3>

↑ **Parent:** [7B](#7b)

Write the [holomorphic function](../../../complex-analysis.md#holomorphic-function) as $f=u+iv$, with $u^2+v^2=C$. If $C=0$ then $f=0$. If $C>0$, differentiating the constant modulus with respect to both coordinates, and using the [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) $u_y=-v_x$, $v_y=u_x$, gives

$$
u u_x+v v_x=0,\qquad v u_x-u v_x=0.
$$

The coefficient matrix has [determinant](../../../linear-algebra.md#determinant) $-(u^2+v^2)=-C\ne0$, so $u_x=v_x=0$. The [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) then also give $u_y=v_y=0$. Along a straight segment inside the disk, both real components have zero derivative and hence are constant. **Thus $f$ is constant throughout the disk.**

## 8F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8f/solution">Solution</h3>

↑ **Parent:** [8F](#8f)

Use the convention that a [sesquilinear form](../../../linear-algebra.md#sesquilinear-form) is linear in its first argument and conjugate-linear in its second: for complex scalars $a,b$,

$$
\phi(av_1+bv_2,w)=a\phi(v_1,w)+b\phi(v_2,w),\qquad \phi(v,aw_1+bw_2)=\bar a\phi(v,w_1)+\bar b\phi(v,w_2).
$$

No symmetry or positivity is assumed. Put $\chi=\phi-\psi$. Its diagonal vanishes. Expansion at $v+w$ gives

$$
\chi(v,w)+\chi(w,v)=0,
$$

while expansion at $v+iw$ gives

$$
-i\chi(v,w)+i\chi(w,v)=0.
$$

These two equations force $\chi(v,w)=\chi(w,v)=0$. This is the [polarization argument for a vanishing quadratic form](../../../linear-algebra.md#polarization-argument-for-a-vanishing-quadratic-form), and proves **$\phi=\psi$ on every pair of vectors**.

For the final deduction, the [linear map](../../../vector-space.md#linear-map) $\alpha$ makes $\psi(v,w)=\phi(\alpha v,\alpha w)$ another [sesquilinear form](../../../linear-algebra.md#sesquilinear-form). Its diagonal agrees with that of $\phi$, so the result just proved gives

$$
\boxed{\phi(\alpha v,\alpha w)=\phi(v,w)\quad\text{for all }v,w\in V}.
$$

## 9D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9d/solution">Solution</h3>

↑ **Parent:** [9D](#9d)

Use the position-space [momentum operator](../../../quantum-mechanics.md#momentum-operator) $P_j=-i\hbar\partial_j$ and set $F=(x+iy)z$. Direct differentiation gives

$$
L_zF=-i\hbar(x\partial_y-y\partial_x)F=-i\hbar(ix-y)z=\hbar F.
$$

To compute the squared [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum), write $D_x=y\partial_z-z\partial_y$, $D_y=z\partial_x-x\partial_z$, $D_z=x\partial_y-y\partial_x$, so $L_j=-i\hbar D_j$. Expanding the products, including derivatives of their variable coefficients, gives

$$
D_x^2+D_y^2+D_z^2=r^2\Delta-E^2-E,\qquad E=x\partial_x+y\partial_y+z\partial_z.
$$

For example $D_x^2=y^2\partial_z^2+z^2\partial_y^2-2yz\partial_y\partial_z-y\partial_y-z\partial_z$; summing the three cyclic expressions proves the identity.

Here $\Delta F=0$ and $EF=2F$, so $E^2F=4F$. Therefore

$$
\boxed{\mathbf L^2F=6\hbar^2F,\qquad L_zF=\hbar F}.
$$

This is the [angular momentum of a homogeneous harmonic polynomial](../../../quantum-mechanics.md#angular-momentum-of-a-homogeneous-harmonic-polynomial), with angular quantum numbers $\ell=2,m=1$. The polynomial is a nonzero angular [eigenfunction](../../../linear-operator-theory.md#eigenfunction); by itself it is not a normalizable full-space [wavefunction](../../../quantum-mechanics.md#wave-function).

## 10E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10e/a">a</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/a/solution">Solution</h4>

↑ **Parent:** [A](#10e/a)

The [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) says that a self-map $g$ of a nonempty [complete metric space](../../../topological-analysis.md#complete-metric-space) satisfying $d(gx,gy)\leq k d(x,y)$ for a constant $0\leq k<1$ has exactly one [fixed point](../../../function.md#fixed-point). Apply it to $g=f^N$ to obtain $p$ with $f^Np=p$.

No continuity of $f$ itself is needed: composition gives

$$
f^N(fp)=f(f^Np)=fp.
$$

Thus $fp$ is also a [fixed point](../../../function.md#fixed-point) of $f^N$, whose uniqueness forces $fp=p$. Conversely any [fixed point](../../../function.md#fixed-point) of $f$ is fixed by $f^N$, so it must equal $p$. **The unique fixed point of the contracting iterate is also the unique fixed point of $f$.** The usual nonempty-space hypothesis is necessary; an empty space has no fixed point.

<h3 id="10e/b">b</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/b/solution">Solution</h4>

↑ **Parent:** [B](#10e/b)

The strict distance inequality implies $d(fx,fy)\leq d(x,y)$ for all points, so $f$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity). Hence

$$
g(x)=d(fx,x)
$$

is a [continuous function](../../../calculus.md#continuous-function), since $|g(x)-g(y)|\leq d(fx,fy)+d(x,y)\leq2d(x,y)$. On the nonempty [compact metric space](../../../topological-analysis.md#compact-metric-space), $g$ attains its minimum at some $p$.

If $fp\ne p$, the strict distance inequality applied to $fp,p$ gives

$$
g(fp)=d(f^2p,fp)<d(fp,p)=g(p),
$$

a contradiction. Thus $fp=p$. If $p,q$ were different [fixed points](../../../function.md#fixed-point), then $d(p,q)=d(fp,fq)<d(p,q)$, again impossible. **There is exactly one fixed point.** This proves [strict distance decrease on a compact metric space](../../../analysis.md#strict-distance-decrease-on-a-compact-metric-space) without assuming a uniform contraction constant.

<h3 id="10e/c">c</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/c/solution">Solution</h4>

↑ **Parent:** [C](#10e/c)

Let $K=\overline{O(x)}$. It is nonempty, closed and bounded in finite-dimensional [Euclidean space](../../../functional-analysis.md#euclidean-norm), hence compact by the [Heine-Borel theorem](../../../topology.md#heine-borel-theorem). The strict distance inequality again makes $f$ [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity). If $y\in K$, choose a sequence $y_j\in O(x)$ converging to $y$. Then $fy_j\in O(x)$, and continuity gives $fy_j\to fy$, so $fy\in K$. This proves **$f(K)\subseteq K$**.

The restriction to $K$ satisfies [strict distance decrease on a compact metric space](../../../analysis.md#strict-distance-decrease-on-a-compact-metric-space), so part (b) produces a [fixed point](../../../function.md#fixed-point) there. If a second [fixed point](../../../function.md#fixed-point) existed anywhere in $\mathbb R^n$, the same strict distance inequality applied to the two points would contradict equality of their distance. **Therefore the fixed point is unique in all of $\mathbb R^n$.** This is the [bounded-orbit fixed point for a strictly distance-decreasing Euclidean map](../../../analysis.md#bounded-orbit-fixed-point-for-a-strictly-distance-decreasing-euclidean-map).

## 11C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

Under a Cartesian frame change $B'_i=R_{ik}B_k$, where $R$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix). Orthogonality gives $B'_kB'_k=B_kB_k$ and $R_{ik}R_{j\ell}\delta_{k\ell}=\delta_{ij}$. Therefore

$$
\alpha B'_iB'_j+\beta|\mathbf B'|^2\delta_{ij}=R_{ik}R_{j\ell}T_{k\ell},
$$

which is the [tensor component transformation law](../../../general-relativity.md#tensor-component-transformation-law). Also $T_{ij}=T_{ji}$ directly, proving that it is a symmetric [Cartesian second-rank tensor](../../../linear-algebra.md#cartesian-second-rank-tensor) for every choice of the two scalars.

For $\mathbf B\ne0$, the direction of $\mathbf B$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $(\alpha+\beta)|\mathbf B|^2$. Every vector perpendicular to $\mathbf B$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\beta|\mathbf B|^2$, a two-dimensional [eigenspace](../../../linear-operator-theory.md#eigenspace). If $\alpha=0$, these eigenvalues coincide and every nonzero vector is an eigenvector. If $\mathbf B=0$, the [tensor](../../../linear-algebra.md#tensor) is zero and again every nonzero vector is an eigenvector, now with eigenvalue zero.

For the position-dependent field with zero [divergence](../../../calculus.md#divergence), the [product rule](../../../calculus.md#product-rule) gives

$$
\partial_jT_{ij}=\alpha B_j\partial_jB_i+2\beta B_k\partial_iB_k.
$$

Contraction of the two [Levi-Civita symbols](../../../calculus.md#levi-civita-symbol) in the [curl](../../../calculus.md#curl) and [cross product](../../../vector-space.md#cross-product) gives

$$
[(\nabla\times\mathbf B)\times\mathbf B]_i=B_j\partial_jB_i-B_k\partial_iB_k.
$$

Consequently

$$
\boxed{\alpha=1,\qquad\beta=-\frac12},\qquad T_{ij}=B_iB_j-\frac12|\mathbf B|^2\delta_{ij}.
$$

These constants give the magnetic part of the [Maxwell stress tensor](../../../electromagnetism.md#maxwell-stress-tensor), with its physical prefactor suppressed. They are forced if the identity is to hold for every divergence-free field: $\mathbf B=(y,0,0)$ forces $2\beta=-1$; at the origin $\mathbf B=(y,1,0)$ then forces $\alpha=1$.

Apply the [divergence theorem](../../../calculus.md#divergence-theorem) separately to each component:

$$
\int_V[(\nabla\times\mathbf B)\times\mathbf B]_i\,dV=\int_S T_{ij}n_j\,dS.
$$

Since the whole vector field vanishes on $S$, all components of $T$ vanish there, and hence **the vector volume integral is zero**. The argument assumes a differentiable field and a boundary for which the [divergence theorem](../../../calculus.md#divergence-theorem) applies.

## 12H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12h/solution">Solution</h3>

↑ **Parent:** [12H](#12h)

For independent observations from a [normal distribution](../../../probability-theory.md#normal-distribution) with unknown mean and positive variance, the [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) of the mean gives

$$
\boxed{\widehat\mu=\bar X=74.56}.
$$

Indeed $\sum_i(X_i-\mu)^2=S_{XX}+n(\bar X-\mu)^2$, which is minimized at $\mu=\bar X$. The [likelihood](../../../statistical-modelling.md#likelihood-function) is

$$
L(\mu,\sigma^2)=(2\pi\sigma^2)^{-n/2}\exp\!\left[-\frac{S_{XX}+n(\bar X-\mu)^2}{2\sigma^2}\right].
$$

For fixed $\mu$, differentiation in $\sigma^2$ gives the maximizer $[S_{XX}+n(\bar X-\mu)^2]/n$. Thus the unrestricted fit has $\widehat\sigma^2=S_{XX}/n$, whereas under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) $\mu=\mu_0$ the fitted variance is $[S_{XX}+n(\bar X-\mu_0)^2]/n$. Both maximize rather than minimize the likelihood: it tends to zero at either variance endpoint when the residual sum of squares is positive.

The restricted-to-unrestricted [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) is therefore

$$
\Lambda=\left[\frac{S_{XX}}{S_{XX}+n(\bar X-\mu_0)^2}\right]^{n/2}=\left(1+\frac{T^2}{n-1}\right)^{-n/2},\qquad T=\frac{\sqrt n(\bar X-\mu_0)}{s},\quad s^2=\frac{S_{XX}}{n-1}.
$$

The [generalized likelihood-ratio test](../../../statistical-modelling.md#generalized-likelihood-ratio-test) rejects for small $\Lambda$, equivalently large $|T|$. Under the null, $Z=\sqrt n(\bar X-\mu_0)/\sigma$ is standard normal, $U=S_{XX}/\sigma^2$ has a [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $n-1$ degrees of freedom, and they are independent. To see the independence, apply an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) to the standardized normal sample, taking its first row to be $(1,\ldots,1)/\sqrt n$: the transformed coordinates remain independent standard normal variables, and $U$ is the sum of squares of the other $n-1$ coordinates. Hence $T=Z/\sqrt{U/(n-1)}$ has [Student's t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution) with $n-1$ degrees of freedom.

For this two-sided test at $5\%$, the cutoff is the $97.5\%$ percentile of $t_9$, namely $2.26$. The data give

$$
s^2=\frac{12.824}{9},\qquad T=\frac{\sqrt{10}(74.56-75)}{\sqrt{12.824/9}}\simeq-1.166.
$$

Since $|T|<2.26$, **do not reject the manufacturer's mean-hardness claim at the $5\%$ level**. This is a failure to reject, not proof that the mean equals $75$.

## 13G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13g/a">a</h3>

↑ **Parent:** [13G](#13g)

<h4 id="13g/a/solution">Solution</h4>

↑ **Parent:** [A](#13g/a)

Define $\mathcal T$ to be the family of all unions of members of $\mathcal B$, including the empty union. We will verify that this is a [topology](../../../topology.md) and that $\mathcal B$ is a [basis of a topology](../../../topology.md#basis-of-a-topology). The two conditions play different roles: the covering condition supplies the whole space, while the local intersection condition supplies closure under finite intersections.

<h4 id="13g/a/i">i</h4>

↑ **Parent:** [A](#13g/a)

<h5 id="13g/a/i/solution">Solution</h5>

↑ **Parent:** [I](#13g/a/i)

By the covering condition, $X=\bigcup_{B\in\mathcal B}B$ belongs to $\mathcal T$. The empty set belongs to $\mathcal T$ as the empty union. An arbitrary union of sets that are themselves unions of members of $\mathcal B$ is still a union of members of $\mathcal B$. Thus $\mathcal T$ contains $X,\varnothing$ and is closed under arbitrary unions, as required for a [topology](../../../topology.md).

<h4 id="13g/a/ii">ii</h4>

↑ **Parent:** [A](#13g/a)

<h5 id="13g/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#13g/a/ii)

Take $U,V\in\mathcal T$ and $x\in U\cap V$. Their representations as unions provide $B_1,B_2\in\mathcal B$ with $x\in B_1\subseteq U$ and $x\in B_2\subseteq V$. The intersection condition supplies $B\in\mathcal B$ with $x\in B\subseteq B_1\cap B_2\subseteq U\cap V$.

It follows that $U\cap V$ is the union of all members of $\mathcal B$ contained in it, and hence belongs to $\mathcal T$. Induction gives closure under every finite intersection. Together with part (i), this proves that $\mathcal T$ is a [topology](../../../topology.md). Each $B\in\mathcal B$ belongs to $\mathcal T$ as a union with one member, and every open set is a union of such members by construction. **Thus $\mathcal B$ is a basis for $\mathcal T$.** Here the printed subset sign is interpreted as inclusion, allowing equality, as in the usual basis criterion.

<h3 id="13g/b">b</h3>

↑ **Parent:** [13G](#13g)

<h4 id="13g/b/solution">Solution</h4>

↑ **Parent:** [B](#13g/b)

The [lexicographic order](../../../extremal-set-theory.md#lexicographic-order) is a [total order](../../../set.md#total-order). Each point $p=(a,b)$ lies in the order interval between $(a,b-1)$ and $(a,b+1)$, so the order intervals cover $\mathbb R^2$.

If $p$ lies in both $\langle x_1,y_1\rangle$ and $\langle x_2,y_2\rangle$, let $x=\max(x_1,x_2)$ and $y=\min(y_1,y_2)$ in that [total order](../../../set.md#total-order). Then $x<p<y$ and

$$
\langle x_1,y_1\rangle\cap\langle x_2,y_2\rangle=\langle x,y\rangle.
$$

In particular an order interval contains $p$ and is contained in the intersection. Both conditions of part (a) hold, proving that these intervals form a [basis of a topology](../../../topology.md#basis-of-a-topology). **The resulting topology is the [lexicographic order topology on the real plane](../../../set.md#lexicographic-order-topology-on-the-real-plane).**

<h3 id="13g/c">c</h3>

↑ **Parent:** [13G](#13g)

<h4 id="13g/c/solution">Solution</h4>

↑ **Parent:** [C](#13g/c)

For every $a\in\mathbb R$, the nonempty order interval

$$
U_a=\langle(a,-1),(a,1)\rangle=\{a\}\times(-1,1)
$$

is open in the [lexicographic order topology on the real plane](../../../set.md#lexicographic-order-topology-on-the-real-plane). The sets $U_a$ are pairwise disjoint.

Suppose $\{B_n:n\in\mathbb N\}$ were a countable [basis of a topology](../../../topology.md#basis-of-a-topology). For each $a$, the [basis of a topology](../../../topology.md#basis-of-a-topology) property gives a member containing $(a,0)$ and contained in $U_a$. Let $n(a)$ be the least index of such a member. The same nonempty $B_n$ cannot lie in two disjoint $U_a$, so $a\mapsto n(a)$ is an injection from the uncountable set $\mathbb R$ into $\mathbb N$, a contradiction. **This topology is not second countable.**

## 14B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14b/a">a</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/a/solution">Solution</h4>

↑ **Parent:** [A](#14b/a)

For distinct [interpolation nodes](../../../numerical-analysis.md#interpolation-node) $x_0,\ldots,x_n$, let $p_n$ be the unique [polynomial](../../../polynomial.md) of degree at most $n$ satisfying $p_n(x_i)=f(x_i)$. Existence follows from the [Lagrange polynomial](../../../numerical-analysis.md#lagrange-polynomial) expression

$$
p_n(x)=\sum_{i=0}^nf(x_i)\prod_{j\ne i}\frac{x-x_j}{x_i-x_j};
$$

uniqueness follows because the difference of two interpolants has $n+1$ distinct zeros but degree at most $n$.

Define the [divided difference](../../../numerical-analysis.md#divided-difference) $f[x_0,\ldots,x_n]$ to be the coefficient of $x^n$ in $p_n$, even when that coefficient is zero. For $n=0$ this gives $f[x_0]=f(x_0)$. Permuting the nodes does not change the interpolation conditions, so it does not change their unique interpolant or this coefficient. **The divided difference is symmetric in all the nodes.** Equivalently its symmetric expression is

$$
f[x_0,\ldots,x_n]=\sum_{i=0}^n\frac{f(x_i)}{\prod_{j\ne i}(x_i-x_j)}.
$$

<h3 id="14b/b">b</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/b/solution">Solution</h4>

↑ **Parent:** [B](#14b/b)

For $n\geq1$, let $p_L,p_R$ be the [interpolation polynomials](../../../numerical-analysis.md#interpolation-polynomial) of degree at most $n-1$ on nodes $x_0,\ldots,x_{n-1}$ and $x_1,\ldots,x_n$, respectively. The polynomial

$$
p(x)=\frac{(x-x_0)p_R(x)-(x-x_n)p_L(x)}{x_n-x_0}
$$

has degree at most $n$. At $x_0$ it equals $p_L(x_0)$; at $x_n$ it equals $p_R(x_n)$. At each common node both interpolants equal $f$, and the displayed weights sum to one, so $p$ also equals $f$ there. Thus it is the full interpolant by uniqueness.

Its coefficient of $x^n$ is the difference of the leading coefficients of $p_R,p_L$ divided by $x_n-x_0$. By the definition of a [divided difference](../../../numerical-analysis.md#divided-difference),

$$
\boxed{f[x_0,\ldots,x_n]=\frac{f[x_1,\ldots,x_n]-f[x_0,\ldots,x_{n-1}]}{x_n-x_0}}.
$$

<h3 id="14b/c">c</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/c/solution">Solution</h4>

↑ **Parent:** [C](#14b/c)

Write $D=f[x_0,\ldots,x_n]$ and let $D_i$ be the [divided difference](../../../numerical-analysis.md#divided-difference) with $x_i$ omitted. By symmetry from part (a), reorder the full list so that its first node is $x_i$ and its last is $x_j$. The recurrence from part (b) then has first omitted-node term $D_i$ and second omitted-node term $D_j$, and gives

$$
\boxed{D=\frac{D_i-D_j}{x_j-x_i}}.
$$

This proves the requested identity for every pair $i\ne j$ and fixes its sign explicitly; it is one of the [omitted-node identities for divided differences](../../../numerical-analysis.md#omitted-node-identities-for-divided-differences).

<h3 id="14b/d">d</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/d/solution">Solution</h4>

↑ **Parent:** [D](#14b/d)

Continue with $D,D_i$ from part (c). Comparing omission of $x_i$ and $x_n$ gives

$$
D_i=D_n+(x_n-x_i)D.
$$

Comparing omission of $x_0$ and $x_n$ gives $D_0=D_n+(x_n-x_0)D$. Eliminating $D$ proves

$$
\boxed{D_i=\gamma D_n+(1-\gamma)D_0,\qquad \gamma=\frac{x_i-x_0}{x_n-x_0}}.
$$

Here $D_n=f[x_0,\ldots,x_{n-1}]$ and $D_0=f[x_1,\ldots,x_n]$, so this is exactly the required [omitted-node identities for divided differences](../../../numerical-analysis.md#omitted-node-identities-for-divided-differences). The original nodes need not be ordered, and the formula remains valid even if $\gamma$ lies outside $[0,1]$.

## 15G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15g/a">a</h3>

↑ **Parent:** [15G](#15g)

<h4 id="15g/a/solution">Solution</h4>

↑ **Parent:** [A](#15g/a)

If $U$ is a [unipotent matrix](../../../lie-theory.md#unipotent-matrix), $N=U-I$ is a [nilpotent matrix](../../../linear-operator-theory.md#nilpotent-matrix). If $Uv=\lambda v$ for a nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector), then $N^mv=(\lambda-1)^mv=0$ for some $m$, forcing $\lambda=1$.

Conversely, suppose the only [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $1$. Over $\mathbb C$, the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is then $(t-1)^n$. The [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) gives $(U-I)^n=0$, so $U-I$ is nilpotent. **Thus $U$ is unipotent if and only if its only eigenvalue is one.**

<h3 id="15g/b">b</h3>

↑ **Parent:** [15G](#15g)

<h4 id="15g/b/solution">Solution</h4>

↑ **Parent:** [B](#15g/b)

Choose an invertible change-of-basis [matrix](../../../vector-space.md#matrix) $P$ so that $J=PTP^{-1}$ is the [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) of $T$. Write each block as

$$
J_{m_j}(\lambda_j)=\lambda_jI_{m_j}+N_{m_j},
$$

where $N_{m_j}$ has ones on its first superdiagonal and all other entries zero. Define

$$
D_0=\bigoplus_j\lambda_jI_{m_j},\qquad N=\bigoplus_jN_{m_j}.
$$

Every $\lambda_j\ne0$ because $T$ is invertible, so $D_0$ is an invertible [diagonal matrix](../../../linear-algebra.md#diagonal-matrix). The [matrix](../../../vector-space.md#matrix) $N$ is strictly upper triangular and hence nilpotent. On each block $D_0$ is a scalar multiple of the identity, so it commutes with $N$ on that block and therefore on the whole space. This gives

$$
\boxed{PTP^{-1}=D_0+N,\qquad D_0N=ND_0}.
$$

<h3 id="15g/c">c</h3>

↑ **Parent:** [15G](#15g)

<h4 id="15g/c/solution">Solution</h4>

↑ **Parent:** [C](#15g/c)

For $D=P^{-1}D_0P$, conjugating $U=D^{-1}T$ gives

$$
PUP^{-1}=D_0^{-1}(D_0+N)=I+D_0^{-1}N.
$$

Because $D_0^{-1}$ commutes with $N$, and $N^n=0$,

$$
(D_0^{-1}N)^n=D_0^{-n}N^n=0.
$$

Thus $U-I$ is similar to a [nilpotent matrix](../../../linear-operator-theory.md#nilpotent-matrix), and is itself nilpotent. **Therefore $U$ is a unipotent matrix.**

<h3 id="15g/d">d</h3>

↑ **Parent:** [15G](#15g)

<h4 id="15g/d/solution">Solution</h4>

↑ **Parent:** [D](#15g/d)

The definition gives $T=DU$. The [matrix](../../../vector-space.md#matrix) $D=P^{-1}D_0P$ is invertible and [diagonalizable](../../../linear-operator-theory.md#diagonalizable-matrix). In the same basis $U$ is $I+D_0^{-1}N$, which commutes with $D_0$ because $N$ does. Conjugating back gives

$$
\boxed{T=DU=UD,\qquad D\text{ diagonalizable},\quad U\text{ unipotent}}.
$$

This is the multiplicative [Jordan decomposition in an affine algebraic group](../../../lie-theory.md#jordan-decomposition-in-an-affine-algebraic-group), here applied to the general linear group. The explicit construction also handles repeated eigenvalues and nontrivial Jordan blocks.

## 16B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16b/a">a</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/a/solution">Solution</h4>

↑ **Parent:** [A](#16b/a)

The [residue](../../../analysis.md#residue) is the coefficient of $(z-a)^{-1}$ in the [Laurent series](../../../analysis.md#laurent-series):

$$
\boxed{\operatorname{res}(f,a)=c_{-1}}.
$$

Equivalently it is $\tfrac1{2\pi i}\int_{|z-a|=r}f(z)\,dz$ for a positively oriented circle small enough to enclose no other singularities.

<h3 id="16b/b">b</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/b/solution">Solution</h4>

↑ **Parent:** [B](#16b/b)

If the [pole](../../../isolated-singularity.md#pole) has order $k+1$, multiplying the [Laurent series](../../../analysis.md#laurent-series) by $(z-a)^{k+1}$ gives a function $h$ with a holomorphic extension across $a$:

$$
h(z)=c_{-(k+1)}+c_{-k}(z-a)+\cdots+c_{-1}(z-a)^k+\cdots.
$$

Its coefficient of $(z-a)^k$ is exactly $c_{-1}$. The [Taylor series](../../../calculus.md#taylor-series) coefficient formula gives $h^{(k)}(a)=k!c_{-1}$. Continuity of this derivative at $a$ therefore proves

$$
\boxed{\operatorname{res}(f,a)=\frac{h^{(k)}(a)}{k!}=\lim_{z\to a}\frac{h^{(k)}(z)}{k!}}.
$$

<h3 id="16b/c">c</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/c/solution">Solution</h4>

↑ **Parent:** [C](#16b/c)

Integrate $F(z)=(1+z^2)^{-(k+1)}$ along the interval $[-R,R]$ closed by the positively oriented upper semicircle, with $R>1$. There is just one enclosed [pole](../../../isolated-singularity.md#pole), at $i$, of order $k+1$. There,

$$
h(z)=(z-i)^{k+1}F(z)=(z+i)^{-(k+1)}.
$$

Differentiating $k$ times gives

$$
h^{(k)}(z)=(-1)^k\frac{(2k)!}{k!}(z+i)^{-(2k+1)}.
$$

By part (b),

$$
\operatorname{res}(F,i)=\frac{(-1)^k(2k)!}{(k!)^2(2i)^{2k+1}}=\frac{(2k)!}{2^{2k+1}i(k!)^2}.
$$

On the semicircle $|1+z^2|\geq R^2-1$, so its integral has absolute value at most $\pi R/(R^2-1)^{k+1}$, tending to zero. The real integral converges absolutely, so the [residue theorem](../../../analysis.md#residue-theorem) and the limit $R\to\infty$ give

$$
\boxed{\int_{-\infty}^{\infty}\frac{dx}{(1+x^2)^{k+1}}=2\pi i\operatorname{res}(F,i)=\pi\frac{(2k)!}{(k!)^2}4^{-k}}.
$$

## 17F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17f/solution">Solution</h3>

↑ **Parent:** [17F](#17f)

Use an [inner product](../../../linear-algebra.md#inner-product) linear in its first argument. The [adjoint operator](../../../hilbert-space.md#adjoint-operator) $\alpha^*$ is the unique [linear operator](../../../vector-space.md#linear-operator) such that

$$
\langle\alpha v,w\rangle=\langle v,\alpha^*w\rangle\quad\text{for all }v,w\in V.
$$

In a finite-dimensional [inner product space](../../../linear-algebra.md#inner-product-space), existence follows by choosing an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis): the [matrix](../../../vector-space.md#matrix) of the adjoint is the conjugate transpose of the matrix of $\alpha$. Uniqueness follows from nondegeneracy of the [inner product](../../../linear-algebra.md#inner-product).

If $\alpha(W)\subseteq W$, then for $w\in W$ and $v\in W^\perp$,

$$
\langle w,\alpha^*v\rangle=\langle\alpha w,v\rangle=0.
$$

Thus $\alpha^*v\in W^\perp$. Conversely, if $\alpha^*(W^\perp)\subseteq W^\perp$, the same equality gives $\langle\alpha w,v\rangle=0$ for every $v\in W^\perp$, so $\alpha w\in(W^\perp)^\perp=W$. This proves the [adjoint criterion for an invariant orthogonal complement](../../../hilbert-space.md#adjoint-criterion-for-an-invariant-orthogonal-complement).

The equality $(W^\perp)^\perp=W$ uses the finite-dimensional setting appropriate here. In a general [Hilbert space](../../../hilbert-space.md) it holds for closed subspaces, and an adjoint is assured for bounded operators. Without closedness the converse only implies invariance of the closure. For example in $\ell^2$, take $W$ to be the finite-support sequences and $\alpha v=\langle v,e_1\rangle(2^{-j})_{j\geq1}$. Then $W^\perp=\{0\}$ is automatically adjoint-invariant, but $\alpha e_1\notin W$. Thus the finite-dimensional or closed-subspace hypothesis cannot be omitted from an infinite-dimensional reading.

<h3 id="17f/i">i</h3>

↑ **Parent:** [17F](#17f)

<h4 id="17f/i/solution">Solution</h4>

↑ **Parent:** [I](#17f/i)

A [normal operator](../../../hilbert-space.md#normal-operator) satisfies $\alpha^*\alpha=\alpha\alpha^*$. Moving an operator across the [inner product](../../../linear-algebra.md#inner-product) gives

$$
\|\alpha v\|^2=\langle v,\alpha^*\alpha v\rangle=\langle v,\alpha\alpha^*v\rangle=\|\alpha^*v\|^2.
$$

One of these norms is zero exactly when the other is zero. Therefore

$$
\boxed{\ker\alpha=\ker\alpha^*}.
$$

<h3 id="17f/ii">ii</h3>

↑ **Parent:** [17F](#17f)

<h4 id="17f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#17f/ii)

For any complex $\lambda$, the shifted [linear operator](../../../vector-space.md#linear-operator) $T=\alpha-\lambda I$ is normal: expansion of $T^*T-TT^*$ leaves just $\alpha^*\alpha-\alpha\alpha^*=0$. Apply part (i) to this shifted [normal operator](../../../hilbert-space.md#normal-operator):

$$
\ker(\alpha-\lambda I)=\ker(\alpha^*-\bar\lambda I).
$$

Hence a nonzero vector is an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $\alpha$ with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$ if and only if it is an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $\alpha^*$ with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\bar\lambda$. **The eigenspaces coincide, with conjugate eigenvalues.**

<h3 id="17f/iii">iii</h3>

↑ **Parent:** [17F](#17f)

<h4 id="17f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#17f/iii)

Part (ii) shows that $\alpha^*v=\bar\lambda v$ for every $v\in E_\lambda$, so $E_\lambda$ is invariant under $\alpha^*$. Apply the [adjoint criterion for an invariant orthogonal complement](../../../hilbert-space.md#adjoint-criterion-for-an-invariant-orthogonal-complement) with $\alpha^*$ in place of $\alpha$, using $(\alpha^*)^*=\alpha$. It follows that

$$
\boxed{\alpha(E_\lambda^\perp)\subseteq E_\lambda^\perp}.
$$

The same argument interchanging $\alpha$ and $\alpha^*$ shows that $E_\lambda^\perp$ is invariant under both operators, a fact needed for the induction in part (iv).

<h3 id="17f/iv">iv</h3>

↑ **Parent:** [17F](#17f)

<h4 id="17f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#17f/iv)

Proceed by induction on $\dim V$. The zero-dimensional case has the empty [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). In positive dimension, the [fundamental theorem of algebra](../../../algebra.md#fundamental-theorem-of-algebra) gives a root of the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial), hence a unit [eigenvector](../../../linear-operator-theory.md#eigenvector) $e$ of $\alpha$, say with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$. Part (ii) makes it an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $\alpha^*$ as well. Thus the line spanned by $e$ and its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) are invariant under both operators by the introductory adjoint argument.

On $\{e\}^\perp$, the restriction of $\alpha^*$ is the adjoint of the restriction of $\alpha$, and the restrictions still commute. The restricted [linear operator](../../../vector-space.md#linear-operator) is therefore normal. By induction it has an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector). Adjoining $e$ proves **an orthonormal eigenbasis exists for $V$**, establishing the finite-dimensional [spectral theorem](../../../hilbert-space.md#spectral-theorem) by construction.

For the final deduction, use this [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $e_j$ and write $\alpha e_j=\lambda_je_j$. Define

$$
\beta e_j=|\lambda_j|e_j,\qquad \gamma e_j=\begin{cases}(\lambda_j/|\lambda_j|)e_j,&\lambda_j\ne0,\\e_j,&\lambda_j=0.\end{cases}
$$

The real nonnegative diagonal entries make $\beta$ a [Hermitian operator](../../../hilbert-space.md#hermitian-operator), and the modulus-one diagonal entries make $\gamma$ a [unitary operator](../../../vector-space.md#unitary-operator). Both are diagonal in the same [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), so they commute and $\beta\gamma e_j=\lambda_je_j$ even when $\lambda_j=0$. This proves the required factorization without assuming invertibility.

Conversely, if $\alpha=\beta\gamma$ with $\beta^*=\beta$, $\gamma^*\gamma=\gamma\gamma^*=I$, and $\beta\gamma=\gamma\beta$, then $\alpha^*=\gamma^*\beta$ and

$$
\alpha\alpha^*=\beta^2,\qquad \alpha^*\alpha=\gamma^*\beta^2\gamma=\beta^2.
$$

Thus $\alpha$ is normal. **Normality is equivalent to a commuting Hermitian–unitary factorization**, with the Hermitian factor even selectable nonnegative. This is the [polar decomposition](../../../linear-operator-theory.md#polar-decomposition) with a unitary extension on the kernel.

## 18D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18d/a">a</h3>

↑ **Parent:** [18D](#18d)

<h4 id="18d/a/solution">Solution</h4>

↑ **Parent:** [A](#18d/a)

For the proposed [Gaussian wave packet](../../../quantum-mechanics.md#gaussian-wave-packet), differentiation gives

$$
\partial_t\Psi=(\dot A-A\dot Bx^2)e^{-Bx^2},\qquad \partial_x^2\Psi=(4B^2x^2-2B)\Psi.
$$

Inserting these in the [Time-dependent Schrödinger equation](../../../physics.md#time-dependent-schrodinger-equation) with [Hamiltonian](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) $(p^2-x^2)/2$, its right-hand side becomes

$$
\left[\hbar^2B-\left(2\hbar^2B^2+\frac12\right)x^2\right]\Psi.
$$

Equating the constant and quadratic coefficients with $i\hbar\partial_t\Psi$ yields

$$
\boxed{\dot A=-i\hbar AB,\qquad \dot B=-\frac{i}{2\hbar}-2i\hbar B^2}.
$$

Conversely these two equations make the substitution an identity, so they are sufficient for the [Gaussian evolution in an inverted harmonic oscillator](../../../quantum-mechanics.md#gaussian-evolution-in-an-inverted-harmonic-oscillator).

<h3 id="18d/b">b</h3>

↑ **Parent:** [18D](#18d)

<h4 id="18d/b/solution">Solution</h4>

↑ **Parent:** [B](#18d/b)

Set $z=\phi-it$ with real constant $\phi$. Then

$$
\dot B=-\frac{i}{2\hbar}\sec^2z=-\frac{i}{2\hbar}-\frac{i}{2\hbar}\tan^2z=-\frac{i}{2\hbar}-2i\hbar B^2.
$$

Thus **$B=\tan(\phi-it)/(2\hbar)$ solves the Riccati equation wherever it is finite**. Integrating the amplitude equation also gives

$$
A(t)=A(0)\left[\frac{\cos\phi}{\cos(\phi-it)}\right]^{1/2},
$$

with the square root chosen continuously from $t=0$. For the normalizable solutions used in part (c), $\sin(2\phi)>0$; equivalently one can choose $0<\phi<\pi/2$ modulo $\pi$. The unrestricted real parameter solves the differential equation locally, but not every value defines a normalizable [wavefunction](../../../quantum-mechanics.md#wave-function).

<h3 id="18d/c">c</h3>

↑ **Parent:** [18D](#18d)

<h4 id="18d/c/solution">Solution</h4>

↑ **Parent:** [C](#18d/c)

Write $B=b+ic$ with $b>0$. Normalization of the [Gaussian wave packet](../../../quantum-mechanics.md#gaussian-wave-packet) gives $|A|^2\int e^{-2bx^2}\,dx=1$, hence $|A|^2=\sqrt{2b/\pi}$. The supplied [Gaussian integral](../../../calculus.md#gaussian-integral) ratio then gives

$$
\boxed{\langle x^2\rangle=\frac1{4b}}.
$$

The [momentum operator](../../../quantum-mechanics.md#momentum-operator) obeys $p\Psi=2i\hbar Bx\Psi$, and direct second differentiation gives $p^2\Psi=(2\hbar^2B-4\hbar^2B^2x^2)\Psi$. Taking the [expectation value](../../../quantum-mechanics.md#expectation-value) and substituting the first result gives

$$
\langle p^2\rangle=2\hbar^2B-\frac{\hbar^2B^2}{b}=\frac{\hbar^2B(2b-B)}b=\frac{\hbar^2|B|^2}b=\boxed{4\hbar^2|B|^2\langle x^2\rangle},
$$

since $2b-B=\bar B$. These are the [second moments of a complex Gaussian wave packet](../../../quantum-mechanics.md#second-moments-of-a-complex-gaussian-wave-packet).

For the solution in part (b), the trigonometric identity

$$
\tan(\phi-it)=\frac{\sin(2\phi)-i\sinh(2t)}{\cos(2\phi)+\cosh(2t)}
$$

gives, writing $D=\cosh(2t)+\cos(2\phi)$,

$$
b=\frac{\sin(2\phi)}{2\hbar D},\qquad |B|^2=\frac{\cosh(2t)-\cos(2\phi)}{4\hbar^2D}.
$$

Thus normalizability requires $\sin(2\phi)>0$, and the exact [expectation values](../../../quantum-mechanics.md#expectation-value) are

$$
\langle x^2\rangle=\frac{\hbar[\cosh(2t)+\cos(2\phi)]}{2\sin(2\phi)},\qquad \langle p^2\rangle=\frac{\hbar[\cosh(2t)-\cos(2\phi)]}{2\sin(2\phi)}.
$$

Since $\cosh(2t)\sim e^{2t}/2$,

$$
\boxed{\langle x^2\rangle\sim\langle p^2\rangle\sim\frac{\hbar}{4\sin(2\phi)}e^{2t}}.
$$

Their difference is the constant $-\hbar\cot(2\phi)$, so the mean [energy](../../../classical-mechanics.md#energy) $\langle H\rangle=-\hbar\cot(2\phi)/2$ stays constant despite exponential spreading in both observables.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
