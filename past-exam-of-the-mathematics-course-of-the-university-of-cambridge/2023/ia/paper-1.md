# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperia_1_2023.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperia_1_2023.pdf)

**Table of contents**

- [1A](#1a)
  - [a](#1a/a)
    - [Solution](#1a/a/solution)
  - [b](#1a/b)
    - [Solution](#1a/b/solution)
  - [c](#1a/c)
    - [Solution](#1a/c/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
  - [a](#2c/a)
    - [Solution](#2c/a/solution)
  - [b](#2c/b)
    - [Solution](#2c/b/solution)
  - [c](#2c/c)
    - [Solution](#2c/c/solution)
- [3E](#3e)
  - [Solution](#3e/solution)
  - [i](#3e/i)
    - [Solution](#3e/i/solution)
  - [ii](#3e/ii)
    - [Solution](#3e/ii/solution)
  - [iii](#3e/iii)
    - [Solution](#3e/iii/solution)
- [4E](#4e)
  - [Solution](#4e/solution)
- [5A](#5a)
  - [a](#5a/a)
    - [i](#5a/a/i)
      - [Solution](#5a/a/i/solution)
    - [ii](#5a/a/ii)
      - [Solution](#5a/a/ii/solution)
    - [iii](#5a/a/iii)
      - [Solution](#5a/a/iii/solution)
  - [b](#5a/b)
    - [Solution](#5a/b/solution)
  - [c](#5a/c)
    - [Solution](#5a/c/solution)
- [6C](#6c)
  - [a](#6c/a)
    - [Solution](#6c/a/solution)
  - [b](#6c/b)
    - [Solution](#6c/b/solution)
  - [c](#6c/c)
    - [Solution](#6c/c/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [Solution](#7b/a/solution)
  - [b](#7b/b)
    - [Solution](#7b/b/solution)
  - [c](#7b/c)
    - [Solution](#7b/c/solution)
- [8B](#8b)
  - [Solution](#8b/solution)
- [9E](#9e)
  - [a](#9e/a)
    - [Solution](#9e/a/solution)
  - [b](#9e/b)
    - [Solution](#9e/b/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11E](#11e)
  - [a](#11e/a)
    - [Solution](#11e/a/solution)
  - [b](#11e/b)
    - [Solution](#11e/b/solution)
  - [c](#11e/c)
    - [Solution](#11e/c/solution)
- [12E](#12e)
  - [a](#12e/a)
    - [Solution](#12e/a/solution)
  - [b](#12e/b)
    - [Solution](#12e/b/solution)
  - [c](#12e/c)
    - [Solution](#12e/c/solution)

## 1A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1a/a">a</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/a/solution">Solution</h4>

↑ **Parent:** [A](#1a/a)

For the stated angular-frequency [Fourier transform](../../../analysis.md#fourier-transform) convention, the [convolution theorem](../../../fourier-analysis.md#convolution-theorem) gives

$$
\widetilde{f*g}(k)=\widetilde f(k)\widetilde g(k),
\qquad
(f*g)(x)=\int_{-\infty}^{\infty}f(\xi)g(x-\xi)\,d\xi.
$$

The [Fourier inversion theorem](../../../fourier-analysis.md#fourier-inversion-theorem) and the assumed absolute integrability therefore imply

$$
\boxed{h(x)=\int_{-\infty}^{\infty}f(\xi)g(x-\xi)\,d\xi.}
$$

Since $|-i|=1$ and the principal argument is $-\pi/2$,

$$
\operatorname{Log}(-i)=-\frac{\pi i}{2}.
$$

All logarithms are $-\pi i/2+2\pi i n$, $n\in\mathbb Z$.

<h3 id="1a/b">b</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/b/solution">Solution</h4>

↑ **Parent:** [B](#1a/b)

The [Fourier transform of a derivative](../../../fourier-analysis.md#fourier-transform-of-a-derivative) gives

$$
\widetilde{p'}(k)=ik\widetilde p(k).
$$

Since $p'=g$,

$$
\boxed{\widetilde p(k)=\frac{\widetilde g(k)}{ik}},
\qquad k\neq0.
$$

An arbitrary additive constant in $p$ affects only the zero-frequency [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) when transforms are interpreted as distributions.

The values of $\log i$ are $i(\pi/2+2\pi n)$. Hence

$$
i^{-2i}=\exp\{-2i\log i\}
=\exp((4n+1)\pi),\qquad n\in\mathbb Z.
$$

These are infinitely many distinct positive real numbers.

<h3 id="1a/c">c</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/c/solution">Solution</h4>

↑ **Parent:** [C](#1a/c)

Since

$$
\mathcal F^{-1}[e^{ika}]=\delta(x+a),
\qquad
\mathcal F^{-1}[e^{-ika}]=\delta(x-a),
$$

the [Inverse Fourier transforms of phase factors](../../../fourier-analysis.md#inverse-fourier-transforms-of-phase-factors) give

$$
\boxed{
\mathcal F^{-1}[\cos(ka)]
=\frac12\bigl[\delta(x+a)+\delta(x-a)\bigr]
}
$$

and

$$
\boxed{
\mathcal F^{-1}[\sin(ka)]
=\frac1{2i}\bigl[\delta(x+a)-\delta(x-a)\bigr].
}
$$

From $z=\tan w=-i(e^{2iw}-1)/(e^{2iw}+1)$ one obtains

$$
e^{2iw}=\frac{1+iz}{1-iz},
\qquad
w=\frac1{2i}\log\frac{1+iz}{1-iz}.
$$

For $z=(2\sqrt3-3i)/7$ the quotient is $1+i\sqrt3=2e^{i\pi/3}$. Its principal logarithm is $\log2+i\pi/3$, so the principal value is

$$
\boxed{\tan^{-1}z=\frac\pi6-\frac i2\log2.}
$$

## 2C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

The Hermitian conjugate is $A^\dagger=\overline A^{,T}$. A [matrix](../../../vector-space.md#matrix) is unitary when $A^\dagger A=AA^\dagger=I$, and Hermitian when $A^\dagger=A$.

<h3 id="2c/a">a</h3>

↑ **Parent:** [2C](#2c)

<h4 id="2c/a/solution">Solution</h4>

↑ **Parent:** [A](#2c/a)

For $B=A^{-1}A^\dagger$,

$$
B^\dagger B=A(A^\dagger)^{-1}A^{-1}A^\dagger.
$$

Multiplying $B^\dagger B=I$ on the left by $A^{-1}$ and on the right by $(A^\dagger)^{-1}$ shows that it is equivalent to $(A^\dagger)^{-1}A^{-1}=A^{-1}(A^\dagger)^{-1}$. Taking inverses gives $A^\dagger A=AA^\dagger$. Thus $B$ is unitary exactly when $A$ is a [normal matrix](../../../linear-operator-theory.md#normal-matrix).

<h3 id="2c/b">b</h3>

↑ **Parent:** [2C](#2c)

<h4 id="2c/b/solution">Solution</h4>

↑ **Parent:** [B](#2c/b)

Normality gives

$$
|Cx|^2=x^\dagger C^\dagger Cx=x^\dagger CC^\dagger x=|C^\dagger x|^2.
$$

**Therefore one norm vanishes exactly when the other does.**

<h3 id="2c/c">c</h3>

↑ **Parent:** [2C](#2c)

<h4 id="2c/c/solution">Solution</h4>

↑ **Parent:** [C](#2c/c)

Apply part (b) to the normal [matrix](../../../vector-space.md#matrix) $C=D-\lambda I$. Since $(D-\lambda I)e=0$, one has

$$
(D^\dagger-\overline\lambda I)e=C^\dagger e=0.
$$

**Thus $e$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $D^\dagger$ with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\overline\lambda$.**

## 3E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3e/solution">Solution</h3>

↑ **Parent:** [3E](#3e)

If $f$ is [differentiable](../../../analysis.md#differentiable-function) at $a$ and $g$ at $f(a)$, then $g\circ f$ is [differentiable](../../../analysis.md#differentiable-function) at $a$ and

$$
(g\circ f)'(a)=g'(f(a))f'(a).
$$

Write $g(f(a)+u)-g(f(a))=u\{g'(f(a))+\varepsilon(u)\}$, where $\varepsilon(u)\to0$, and put $u=f(a+h)-f(a)$. Division by $h$ and passage to the [limit](../../../calculus.md#limit-of-a-function) proves the formula.

<h3 id="3e/i">i</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/i/solution">Solution</h4>

↑ **Parent:** [I](#3e/i)

**No.** Take $f(x)=x^2$, $a=0$, and $g(y)=|y|$. The [function](../../../function.md) $g$ is not [differentiable](../../../analysis.md#differentiable-function) at $f(0)=0$, but $g(f(x))=x^2$ is [differentiable](../../../analysis.md#differentiable-function). Neither [function](../../../function.md) is constant on an interval.

<h3 id="3e/ii">ii</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3e/ii)

**No.** Take $f(x)=|x|$, $a=0$, and $g(y)=y^2$. Then $f$ is not [differentiable](../../../analysis.md#differentiable-function) at zero, but $g\circ f=x^2$ is [differentiable](../../../analysis.md#differentiable-function) there.

<h3 id="3e/iii">iii</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3e/iii)

**No.** Take

$$
f(x)=\begin{cases}x,&x\geq0,\\2x,&x<0,\end{cases}
\qquad
g(y)=\begin{cases}2y,&y\geq0,\\y,&y<0.
\end{cases}
$$

Both [functions](../../../function.md) are nonconstant on every interval and nondifferentiable at zero, but $g(f(x))=2x$ is [differentiable](../../../analysis.md#differentiable-function).

## 4E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4e/solution">Solution</h3>

↑ **Parent:** [4E](#4e)

The comparison test says that if $0\leq b_n\leq c_n$ eventually and $\sum c_n$ converges, then $\sum b_n$ converges. If $\sum a_nz_0^n$ converges, its terms are bounded: $|a_nz_0^n|\leq M$. For $|z_1|<|z_0|$,

$$
|a_nz_1^n|\leq M\left|\frac{z_1}{z_0}\right|^n,
$$

so comparison with a geometric [series](../../../real-analysis.md#series-mathematics) proves absolute convergence.

The radius $R$ is the number for which the power [series](../../../real-analysis.md#series-mathematics) converges absolutely for $|z|<R$ and diverges for $|z|>R$. Given $r_i<R_i$, both $\sum|a_n|r_1^n$ and $\sum|b_n|r_2^n$ converge, so their terms are bounded, say $|a_n|r_1^n\leq M$. Then

$$
\sum|a_nb_n|(r_1r_2)^n
\leq M\sum|b_n|r_2^n<\infty.
$$

**Thus $R\geq r_1r_2$; letting $r_i\uparrow R_i$ gives $R\geq R_1R_2$.**

## 5A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5a/a">a</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/a/i">i</h4>

↑ **Parent:** [A](#5a/a)

<h5 id="5a/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5a/a/i)

This is the plane through $a$ perpendicular to the nonzero [normal vector](../../../differential-geometry.md#normal-vector) $n$.

<h4 id="5a/a/ii">ii</h4>

↑ **Parent:** [A](#5a/a)

<h5 id="5a/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5a/a/ii)

This is the affine plane through $b,d,f$, provided $d-b$ and $f-b$ are independent. The [scalars](../../../vector-space.md#scalar) $\lambda,\mu$ are affine coordinates in those two directions.

<h4 id="5a/a/iii">iii</h4>

↑ **Parent:** [A](#5a/a)

<h5 id="5a/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5a/a/iii)

This is the sphere with centre $c$ and radius $\rho>0$.

<h3 id="5a/b">b</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/b/solution">Solution</h4>

↑ **Parent:** [B](#5a/b)

The cross product of the plane normals is proportional to $(1,-1,-1)$, so

$$
m=\frac1{\sqrt3}(1,-1,-1).
$$

The point on the intersection perpendicular to $m$ is

$$
u=\frac19(11,4,7),
$$

which satisfies both plane equations and $u\cdot m=0$. Hence the line is $r\times m=u\times m$.

The equally inclined line has direction $d=(1,1,1)/\sqrt3$. The distance between the two skew lines is

$$
\boxed{\frac{|u\cdot(m\times d)|}{|m\times d|}
=\frac1{3\sqrt2}.}
$$

<h3 id="5a/c">c</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/c/solution">Solution</h4>

↑ **Parent:** [C](#5a/c)

The signed displacement of the sphere centre from the plane is $g\cdot n-p$. Orthogonal projection gives the circle centre

$$
h=g+(p-g\cdot n)n.
$$

Pythagoras gives

$$
R=\sqrt{A^2-(p-g\cdot n)^2}.
$$

A real circle exists when $|p-g\cdot n|\leq A$: equality gives tangency and radius zero, while strict inequality gives a genuine circle.

## 6C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6c/a">a</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/a/solution">Solution</h4>

↑ **Parent:** [A](#6c/a)

The characteristic [polynomial](../../../polynomial.md) is

$$
(\lambda-3)(\lambda-2)^2.
$$

For $\lambda=2$, the eigenspace is spanned only by $(1,0,0)^T$, so its geometric multiplicity is one although its algebraic multiplicity is two. Hence $M$ is not diagonalisable.

<h3 id="6c/b">b</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/b/solution">Solution</h4>

↑ **Parent:** [B](#6c/b)

If $B=S^{-1}AS$, then

$$
\det(tI-B)=\det(S^{-1}(tI-A)S)=\det(tI-A),
$$

so the characteristic [polynomials](../../../polynomial.md), [eigenvalues](../../../linear-operator-theory.md#eigenvalue), and algebraic multiplicities agree. The converse is false: $I_2$ and $\left(\begin{smallmatrix}1&1\\0&1\end{smallmatrix}\right)$ have the same characteristic [polynomial](../../../polynomial.md), but the first is diagonalisable and the second is not, so they cannot be similar.

<h3 id="6c/c">c</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/c/solution">Solution</h4>

↑ **Parent:** [C](#6c/c)

The [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) states that a square [matrix](../../../vector-space.md#matrix) satisfies its characteristic [polynomial](../../../polynomial.md). If a $2\times2$ [matrix](../../../vector-space.md#matrix) is diagonalisable, $A=S\operatorname{diag}(\lambda_1,\lambda_2)S^{-1}$; applying $p(t)=(t-\lambda_1)(t-\lambda_2)$ to the diagonal [matrix](../../../vector-space.md#matrix) gives zero and hence $p(A)=0$.

If $B^k=0$, every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$ satisfies $\lambda^k=0$, so all [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are zero and the characteristic [polynomial](../../../polynomial.md) is $t^n$. Cayley--Hamilton then gives $B^n=0$.

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/solution">Solution</h4>

↑ **Parent:** [A](#7b/a)

For $x\ne0$,

$$
x^\dagger Gx=|Ax|^2>0,
$$

so the Hermitian [matrix](../../../vector-space.md#matrix) $G$ has positive real [eigenvalues](../../../linear-operator-theory.md#eigenvalue). If $Ge_i=\lambda_i e_i$, then

$$
H(Ae_i)=AA^\dagger Ae_i=A(Ge_i)=\lambda_iAe_i.
$$

Moreover $|Ae_i|^2=\lambda_i|e_i|^2$, so $|f_i|/|e_i|=\sqrt{\lambda_i}$.

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/solution">Solution</h4>

↑ **Parent:** [B](#7b/b)

Choose an orthonormal eigenbasis $e_i$ of $G$ and set $u_i=e_i$, $v_i=Ae_i/\sqrt{\lambda_i}$. Part (a) shows that the $v_i$ form an orthonormal eigenbasis of $H$. If $U$ and $V$ have these [vectors](../../../vector-space.md#vector) as columns, then they are unitary and

$$
V^\dagger AU=\operatorname{diag}(\sqrt{\lambda_1},\ldots,\sqrt{\lambda_n}).
$$

This is the [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition).

<h3 id="7b/c">c</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/c/solution">Solution</h4>

↑ **Parent:** [C](#7b/c)

Here

$$
A^\dagger A=\frac12\begin{pmatrix}5&-3\\-3&5\end{pmatrix},
$$

with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $4,1$ and corresponding normalized [vectors](../../../vector-space.md#vector) $(1,-1)^T/\sqrt2$ and $(1,1)^T/\sqrt2$. A compatible choice is

$$
U=\frac1{\sqrt2}\begin{pmatrix}1&1\\-1&1\end{pmatrix},
\qquad
V=\begin{pmatrix}1&0\\0&-1\end{pmatrix},
\qquad
D=\begin{pmatrix}2&0\\0&1\end{pmatrix}.
$$

Direct multiplication gives $V^\dagger AU=D$.

## 8B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8b/solution">Solution</h3>

↑ **Parent:** [8B](#8b)

A real [matrix](../../../vector-space.md#matrix) is orthogonal when $Q^TQ=I$. If $Qv=\lambda v$, norm preservation gives $|\lambda|=1$. If $Qv=\lambda v$ and $Qw=\mu w$, preservation of the Hermitian [inner product](../../../linear-algebra.md#inner-product) gives $(1-\overline\lambda\mu)v^\dagger w=0$; distinct unit-modulus [eigenvalues](../../../linear-operator-theory.md#eigenvalue) therefore have orthogonal [eigenvectors](../../../linear-operator-theory.md#eigenvector).

The nonreal [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of a real $3\times3$ [matrix](../../../vector-space.md#matrix) occur in conjugate pairs. Since their product is one and $\det Q=-1$, the remaining real [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $-1$. If $x\cdot n=0$, then $(Qx)\cdot(Qn)=x\cdot n=0$, and $Qn=-n$, so $Qx\cdot n=0$: the plane $\Pi$ is invariant.

The restriction to $\Pi$ is a planar orthogonal map whose [determinant](../../../linear-algebra.md#determinant) is $(-1)/(-1)=1$, hence a rotation through some $\theta$. In an orthonormal [basis](../../../vector-space.md#basis) adapted to $n$,

$$
Q\sim\operatorname{diag}(-1,R_\theta).
$$

Therefore $\operatorname{tr}Q=-1+2\cos\theta$ and

$$
\boxed{\det(Q-I)=(-2)\det(R_\theta-I)=4(\cos\theta-1).}
$$

## 9E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9e/a">a</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/a/solution">Solution</h4>

↑ **Parent:** [A](#9e/a)

The arithmetic--geometric mean inequality gives $x_n\geq1$ from $n=2$ onward. For $x>1$,

$$
1<\frac12(x+x^{-1})<x,
$$

so the tail decreases to a [limit](../../../calculus.md#limit-of-a-function) $L\geq1$. Passing to the recurrence gives $2L=L+L^{-1}$, hence $L=1$.

For the subadditive [sequence](../../../real-analysis.md#sequence), $0\leq x_n/n\leq x_1$, so it is bounded. The [Fekete lemma](../../../real-analysis.md#fekete-s-lemma) can be proved directly here as follows. Let $\alpha=\inf_kx_k/k$. Fix $k$ and write $n=qk+r$, $0\leq r<k$. Then

$$
\frac{x_n}{n}\leq\frac{qx_k+x_r}{qk+r}\longrightarrow\frac{x_k}{k}.
$$

**Thus $\limsup x_n/n\leq\alpha$, while the definition gives $\liminf x_n/n\geq\alpha$. Hence $x_n/n\to\alpha$.**

<h3 id="9e/b">b</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/b/solution">Solution</h4>

↑ **Parent:** [B](#9e/b)

Let $S_n=\sum_{i\leq n}a_i$ and $T_n=\sum_{i\leq n}|a_i|$. Conditional convergence gives $S_n\to S$ and $T_n\to\infty$. Since $P_n=T_n+S_n$ and $N_n=T_n-S_n$,

$$
\frac{P_n}{N_n}=\frac{1+S_n/T_n}{1-S_n/T_n}\longrightarrow1.
$$

The alternating-series test says that $b_n\downarrow0$ implies convergence of $\sum(-1)^nb_n$. The hypothesis implies $b_n/b_{n+1}>1$ eventually, so $b_n$ is eventually decreasing. For some $c>0$, eventually $b_n/b_{n+1}\geq1+c/n$; the divergent product of these factors forces $b_n\to0$. The test now applies.

## 10E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) says that a continuous $f:[a,b]\to\mathbb R$ takes every value between $f(a)$ and $f(b)$. For $f(a)<y<f(b)$, the closed sets where $f\leq y$ and $f\geq y$ cannot separate the connected interval; equivalently, taking the supremum of $\{x:f(x)\leq y\}$ and using continuity gives a point with value $y$.

Set $\phi(a)=0$ and $\phi(x)=\sin(1/(x-a))$ for $x>a$. Every interval $[a,b]$ contains a zero $c<b$; continuity on $[c,b]$ makes $\phi$ take every value between $0=\phi(a)$ and $\phi(b)$, yet $\phi$ is discontinuous at $a$.

A monotone [function](../../../function.md) can be discontinuous only by a jump. If it had a jump at $c$, any number strictly between the left and right [limits](../../../calculus.md#limit-of-a-function) would lie between $f(a)$ and $f(b)$ but would not be attained, contrary to the hypothesis. Thus it is continuous.

For the last assertion, pass to subsequences with $x_n,y_n$ both within $1/n$ of $a$ and $g(x_n)$ near $l$, $g(y_n)$ near $L$. For $\lambda\in(l,L)$, the intermediate value theorem on the interval joining $x_n$ and $y_n$ gives $z_n$ with $g(z_n)=\lambda$; then $z_n\to a$. The endpoint cases use the original [sequences](../../../real-analysis.md#sequence).

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/a">a</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/a/solution">Solution</h4>

↑ **Parent:** [A](#11e/a)

The mean value theorem says that for continuous $f$ on $[a,b]$, [differentiable](../../../analysis.md#differentiable-function) inside, $f(b)-f(a)=f'(c)(b-a)$ for some $c$. Applied to $\log$ on $[b,a]$,

$$
\log(a/b)=\frac{a-b}{c},\qquad b<c<a,
$$

which gives $(a-b)/a<\log(a/b)<(a-b)/b$.

<h3 id="11e/b">b</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/b/solution">Solution</h4>

↑ **Parent:** [B](#11e/b)

The ordinary mean value theorem gives $\Delta_hf(a)=hf'(b_1)$ for some $b_1\in(a,a+h)$. More generally, applying it to the difference of two translated [functions](../../../function.md) shows inductively that

$$
\Delta_h^kf(a)=h^kf^{(k)}(b_k)
$$

for some $b_k\in(a,a+kh)$. Taking $k=n$ proves the result.

<h3 id="11e/c">c</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/c/solution">Solution</h4>

↑ **Parent:** [C](#11e/c)

**No.** The [Darboux theorem](../../../calculus.md#darboux-s-theorem-analysis) says that every [derivative](../../../calculus.md#derivative) has the intermediate-value property. Choose $\epsilon<1/3$. In a deleted neighborhood of $a$, the assumed [limit](../../../calculus.md#limit-of-a-function) puts $\phi(x)$ within $\epsilon$ of $\phi(a)+1$. Darboux's theorem applied between $a$ and any such $x$ would require values near $\phi(a)+1/2$, which that neighborhood excludes. This contradiction shows that $\phi$ cannot be a [derivative](../../../calculus.md#derivative).

## 12E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12e/a">a</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/a/solution">Solution</h4>

↑ **Parent:** [A](#12e/a)

For a [bounded function](../../../function.md#bounded-function), the lower and upper [integrals](../../../calculus.md#integral) are the supremum of lower Darboux sums and infimum of upper Darboux sums. It is Riemann integrable when these agree.

Here $u(x)=1/x-\lfloor1/x\rfloor$ for $x>0$, so $0\leq u<1$. On $[\delta,1]$ it has only finitely many discontinuities and is piecewise continuous, hence integrable. On $[0,\delta]$ its upper-minus-lower contribution is at most $\delta$. Taking $\delta\downarrow0$ proves integrability on $[0,1]$.

<h3 id="12e/b">b</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/b/solution">Solution</h4>

↑ **Parent:** [B](#12e/b)

Changing variables gives

$$
\frac1h\int_a^x(f(t+h)-f(t))dt
=\frac1h\left(\int_x^{x+h}f(s)ds-\int_a^{a+h}f(s)ds\right).
$$

The average of a [continuous function](../../../calculus.md#continuous-function) over $[y,y+h]$ tends to $f(y)$ as $h\to0$. The two terms therefore tend to $f(x)$ and $f(a)$, proving the stated [limit](../../../calculus.md#limit-of-a-function).

<h3 id="12e/c">c</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/c/solution">Solution</h4>

↑ **Parent:** [C](#12e/c)

The [continuous approximation of a Riemann-integrable function](../../../real-analysis.md#continuous-approximation-of-a-riemann-integrable-function) follows here by choosing partitions $P_n$ with upper-minus-lower sum below $1/n$. On each subinterval choose the midpoint of the infimum and supremum to form a step [function](../../../function.md) $s_n$. Then

$$
\int_a^b|g-s_n|<\frac1n.
$$

Replace each of the finitely many jumps of $s_n$ by a linear transition on intervals of sufficiently small total length, obtaining a continuous $\phi_n$ with $\int|s_n-\phi_n|<1/n$. Hence $\int|g-\phi_n|<2/n$, and uniformly for every subinterval $[\alpha,\beta]$,

$$
\boxed{\left|\int_\alpha^\beta(g-\phi_n)\right|\leq\int_a^b|g-\phi_n|\to0.}
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
