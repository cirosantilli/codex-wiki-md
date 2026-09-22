# Paper 3

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperib_3_2019.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperib_3_2019.pdf)

**Table of contents**

- [1G](#1g)
  - [Solution](#1g/solution)
- [2E](#2e)
  - [a](#2e/a)
    - [Solution](#2e/a/solution)
  - [b](#2e/b)
    - [i](#2e/b/i)
      - [Solution](#2e/b/i/solution)
    - [ii](#2e/b/ii)
      - [Solution](#2e/b/ii/solution)
    - [iii](#2e/b/iii)
      - [Solution](#2e/b/iii/solution)
- [3G](#3g)
  - [a](#3g/a)
    - [Solution](#3g/a/solution)
  - [b](#3g/b)
    - [Solution](#3g/b/solution)
- [4D](#4d)
  - [Solution](#4d/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
- [6A](#6a)
  - [Solution](#6a/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8B](#8b)
  - [Solution](#8b/solution)
- [9H](#9h)
  - [a](#9h/a)
    - [Solution](#9h/a/solution)
  - [b](#9h/b)
    - [Solution](#9h/b/solution)
  - [c](#9h/c)
    - [Solution](#9h/c/solution)
- [10F](#10f)
  - [Solution](#10f/solution)
- [11G](#11g)
  - [a](#11g/a)
    - [Solution](#11g/a/solution)
  - [b](#11g/b)
    - [Solution](#11g/b/solution)
  - [c](#11g/c)
    - [Solution](#11g/c/solution)
- [12E](#12e)
  - [a](#12e/a)
    - [Solution](#12e/a/solution)
  - [b](#12e/b)
    - [i](#12e/b/i)
      - [Solution](#12e/b/i/solution)
    - [ii](#12e/b/ii)
      - [Solution](#12e/b/ii/solution)
- [13F](#13f)
  - [Solution](#13f/solution)
- [14E](#14e)
  - [a](#14e/a)
    - [Solution](#14e/a/solution)
  - [b](#14e/b)
    - [i](#14e/b/i)
      - [Solution](#14e/b/i/solution)
    - [ii](#14e/b/ii)
      - [Solution](#14e/b/ii/solution)
  - [c](#14e/c)
    - [Solution](#14e/c/solution)
- [15D](#15d)
  - [Solution](#15d/solution)
- [16B](#16b)
  - [Solution](#16b/solution)
- [17A](#17a)
  - [Solution](#17a/solution)
- [18C](#18c)
  - [Solution](#18c/solution)
- [19C](#19c)
  - [a](#19c/a)
    - [Solution](#19c/a/solution)
  - [b](#19c/b)
    - [Solution](#19c/b/solution)
  - [c](#19c/c)
    - [Solution](#19c/c/solution)
  - [d](#19c/d)
    - [Solution](#19c/d/solution)
- [20H](#20h)
  - [a](#20h/a)
    - [Solution](#20h/a/solution)
  - [b](#20h/b)
    - [Solution](#20h/b/solution)
  - [c](#20h/c)
    - [i](#20h/c/i)
      - [Solution](#20h/c/i/solution)
    - [ii](#20h/c/ii)
      - [Solution](#20h/c/ii/solution)
    - [iii](#20h/c/iii)
      - [Solution](#20h/c/iii/solution)
  - [d](#20h/d)
    - [Solution](#20h/d/solution)
- [21H](#21h)
  - [a](#21h/a)
    - [Solution](#21h/a/solution)
  - [b](#21h/b)
    - [Solution](#21h/b/solution)

## 1G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1g/solution">Solution</h3>

↑ **Parent:** [1G](#1g)

Write $R=\mathbb Z[\sqrt{-13}]$ and $I=(2,1+\sqrt{-13})$. The map

$$
R\longrightarrow\mathbb F_2,
\qquad a+b\sqrt{-13}\longmapsto a+b\pmod2
$$

is a surjective [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism): in $\mathbb F_2$, the image of $\sqrt{-13}$ is $1$ and $1^2=-13=1$. Its kernel is exactly $I$. Indeed, both generators lie in the kernel; conversely, if $a+b$ is even, then

$$
a+b\sqrt{-13}=b(1+\sqrt{-13})+(a-b),
$$

and $a-b$ is even. Hence $R/I\cong\mathbb F_2$ and the [index of a subgroup](../../../group.md#index-of-a-subgroup) is $[R:I]=2$.

If $I=(\alpha)$ were a [principal ideal](../../../commutative-algebra.md#principal-ideal), multiplication by $\alpha=a+b\sqrt{-13}$ would identify its additive lattice with a sublattice of index

$$
|N(\alpha)|=|\alpha\overline\alpha|=a^2+13b^2.
$$

Thus principality would require $a^2+13b^2=2$. This [Diophantine equation](../../../number-theory.md#diophantine-equation) has no integer solution: $b=0$ would give $a^2=2$, while $b\ne0$ makes the left side at least $13$. Therefore

$$
\boxed{(2,1+\sqrt{-13})\text{ is not principal}}.
$$

## 2E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2e/a">a</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/a/solution">Solution</h4>

↑ **Parent:** [A](#2e/a)

A function $f:A\to\mathbb R$ is [uniformly continuous](../../../topological-analysis.md#uniform-continuity) if, for every $\varepsilon>0$, there is a $\delta>0$ such that

$$
x,y\in A,\quad |x-y|<\delta
\quad\Longrightarrow\quad
|f(x)-f(y)|<\varepsilon.
$$

The same $\delta$ must work at every pair of points in the domain.

<h3 id="2e/b">b</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/b/i">i</h4>

↑ **Parent:** [B](#2e/b)

<h5 id="2e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2e/b/i)

The function $x\mapsto x^2$ is not uniformly continuous on $\mathbb R$. Take $x_n=n$ and $y_n=n+1/n$. Then $|x_n-y_n|\to0$, whereas

$$
|y_n^2-x_n^2|=2+\frac1{n^2}\longrightarrow2.
$$

This contradicts the [sequential criterion for uniform continuity](../../../topological-analysis.md#sequential-criterion-for-uniform-continuity).

<h4 id="2e/b/ii">ii</h4>

↑ **Parent:** [B](#2e/b)

<h5 id="2e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2e/b/ii)

The square-root function is uniformly continuous on $[0,\infty)$. For $x,y\geq0$,

$$
|\sqrt x-\sqrt y|^2
\leq |x-y|,
$$

so $|\sqrt x-\sqrt y|\leq\sqrt{|x-y|}$. Given $\varepsilon>0$, choosing $\delta=\varepsilon^2$ proves uniform continuity.

<h4 id="2e/b/iii">iii</h4>

↑ **Parent:** [B](#2e/b)

<h5 id="2e/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2e/b/iii)

The function $x\mapsto\cos(1/x)$ is uniformly continuous on $[1,\infty)$. Its [derivative](../../../calculus.md#derivative) satisfies

$$
\left|\frac{\sin(1/x)}{x^2}\right|\leq1,
$$

so the [mean value theorem](../../../calculus.md#mean-value-theorem) gives

$$
|\cos(1/x)-\cos(1/y)|\leq|x-y|.
$$

**Thus the function is [Lipschitz](../../../real-analysis.md#lipschitz-continuity), which implies uniform continuity.**

## 3G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3g/a">a</h3>

↑ **Parent:** [3G](#3g)

<h4 id="3g/a/solution">Solution</h4>

↑ **Parent:** [A](#3g/a)

A [compact space](../../../topology.md#compact-space) is one for which every [open cover](../../../topology.md#open-cover) has a finite subcover. A metric space is [sequentially compact](../../../geometry-and-topology.md#sequentially-compact-space) when every [sequence](../../../real-analysis.md#sequence) in it has a [convergent subsequence](../../../real-analysis.md#convergent-subsequence) whose limit belongs to the space.

<h3 id="3g/b">b</h3>

↑ **Parent:** [3G](#3g)

<h4 id="3g/b/solution">Solution</h4>

↑ **Parent:** [B](#3g/b)

First, compactness makes $X$ [totally bounded](../../../topological-analysis.md#totally-bounded-space): for every positive integer $k$, the open cover by balls of radius $1/k$ has a finite subcover. Given a sequence, repeatedly choose a ball of radius $1/k$ containing infinitely many terms of the subsequence retained at the preceding stage. Taking a diagonal subsequence $(x_{n_k})$, any two terms with indices at least $k$ lie in one ball of radius $1/k$, so their distance is below $2/k$. The diagonal subsequence is therefore a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence).

A compact metric space is [complete](../../../topological-analysis.md#complete-metric-space). To see this without assuming sequential compactness, let $(y_n)$ be Cauchy and put $F_n=\overline{\{y_m:m\geq n\}}$. These nonempty closed sets are nested and have the [finite intersection property](../../../topology.md#finite-intersection-property); compactness gives a point $y\in\bigcap_nF_n$. Given $\varepsilon>0$, a sufficiently late tail has diameter below $\varepsilon/2$, and because $y$ lies in its closure, every point of that tail lies within $\varepsilon$ of $y$. Thus $y_n\to y$.

The Cauchy subsequence constructed above consequently converges in $X$. Hence every compact metric space is sequentially compact.

## 4D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4d/solution">Solution</h3>

↑ **Parent:** [4D](#4d)

The [Möbius transformation](../../../group-theory.md#mobius-transformation)

$$
w=i\frac{1-z}{1+z}
$$

maps the [unit disc](../../../topology.md#unit-disc) conformally onto the upper half-plane. On the upper semicircle of its boundary, $w$ approaches the positive real axis; on the lower semicircle it approaches the negative real axis. If $0<\arg w<\pi$, the harmonic function

$$
\phi(w)=\phi_0\left(1-\frac{2\arg w}{\pi}\right)
$$

has the required boundary limits.

For $z=x+iy$,

$$
w=\frac{2y+i(1-x^2-y^2)}{(1+x)^2+y^2}.
$$

Since the imaginary part is positive inside the disc,

$$
\frac\pi2-\arg w
=\arctan\frac{\operatorname{Re}w}{\operatorname{Im}w}
=\arctan\frac{2y}{1-x^2-y^2}.
$$

Therefore the solution of the [Dirichlet problem](../../../analysis.md#dirichlet-problem) is

$$
\boxed{\phi(x,y)=\frac{2\phi_0}{\pi}
\arctan\!\left(\frac{2y}{1-x^2-y^2}\right)},
\qquad x^2+y^2<1.
$$

The exceptional boundary endpoints are precisely the jump points of the prescribed data.

## 5E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

On the unit sphere, the [spherical excess formula](../../../differential-geometry.md#spherical-excess-formula) gives the area of a spherical triangle as

$$
\boxed{A=\alpha+\beta+\gamma-\pi}.
$$

For a sphere of radius $R$, the right side is multiplied by $R^2$.

Join an interior point of a convex spherical $n$-gon to its vertices by geodesics. The resulting $n$ spherical triangles contain all polygon angles and angles summing to $2\pi$ at the interior point. Adding their spherical excesses gives

$$
\boxed{A=\sum_{i=1}^n\alpha_i-(n-2)\pi}.
$$

For a regular polygon with interior angle $\alpha$, positivity of area requires $n\alpha>(n-2)\pi$, while strict convexity requires $\alpha<\pi$. Both limiting values can be approached by regular polygons, so

$$
\boxed{\frac{n-2}{n}\pi<\alpha<\pi}.
$$

## 6A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6a/solution">Solution</h3>

↑ **Parent:** [6A](#6a)

Since

$$
f''(x)=(a-1)x^{a-2}>0
$$

for $x>0$, the second-derivative criterion shows that $f(x)=x^a/a$ is [strictly convex](../../../real-analysis.md#strictly-convex-function). Put $b=a/(a-1)$, so $1/a+1/b=1$. For dual variable $p>0$, the stationary equation in the [Legendre transform](../../../convex-optimization.md#convex-conjugate) is

$$
p=f'(x)=x^{a-1},
\qquad x=p^{1/(a-1)}.
$$

It is the unique global maximizer of $px-f(x)$, and hence

$$
\boxed{f^*(p)=\frac{p^b}{b}},
\qquad p>0.
$$

Applying the same calculation with the conjugate exponent $b$ gives

$$
\boxed{(f^*)^*(x)=\frac{x^a}{a}=f(x)},
\qquad x>0.
$$

Under the [Legendre-Fenchel transform](../../../convex-optimization.md#convex-conjugate) on all real dual variables, the same supremum additionally gives $f^*(p)=0$ for $p\leq0$.

Now take $a=r$, $b=s$, and apply the [Fenchel–Young inequality](../../../convex-optimization.md#fenchel-young-inequality) $f(x)+f^*(y)\geq xy$. This yields [Young's inequality for products](../../../nonlinear-analysis.md#young-s-inequality-for-products)

$$
\boxed{\frac{x^r}{r}+\frac{y^s}{s}\geq xy}
$$

for positive $x,y$ and conjugate exponents $r,s$.

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

Let $\omega=e^{2\pi i/N}$. Using the convention

$$
\widehat x_k=\sum_{n=0}^{N-1}x_n\omega^{-kn},
\qquad 0\leq k<N,
$$

the [discrete Fourier transform](../../../numerical-analysis.md#discrete-fourier-transform) of the supplied sequence follows from the [binomial theorem](../../../combinatorics.md#binomial-theorem):

$$
x_n=\frac1N\sum_{m=0}^{N-1}\binom{N-1}{m}\omega^{mn}.
$$

The [orthogonality of roots of unity](../../../algebra.md#orthogonality-of-roots-of-unity) gives

$$
\sum_{n=0}^{N-1}\omega^{(m-k)n}
=\begin{cases}N,&m=k,\\0,&m\ne k.\end{cases}
$$

Since $m,k$ both lie between zero and $N-1$, it follows that

$$
\boxed{\widehat x_k=\binom{N-1}{k}},
\qquad k=0,\ldots,N-1.
$$

## 8B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8b/solution">Solution</h3>

↑ **Parent:** [8B](#8b)

For square-integrable wavefunctions with the stated decay, multiplication by the real coordinate $x$ is [Hermitian](../../../hilbert-space.md#hermitian-operator) because

$$
\langle\psi,x\chi\rangle=\langle x\psi,\chi\rangle.
$$

For $p_x=-i\hbar\partial_x$, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\langle\psi,p_x\chi\rangle
=\langle p_x\psi,\chi\rangle
-i\hbar\int_{-\infty}^{\infty}[\overline\psi\chi]_{x=-\infty}^{x=\infty}\,dy,
$$

and the boundary term vanishes. The same arguments apply to $y$ and $p_y$.

If $F$ and $G$ are Hermitian on a common suitable domain, then $(FG)^\dagger=GF$, so

$$
\left[\frac12(FG+GF)\right]^\dagger
=\frac12(FG+GF).
$$

Because $x$ commutes with $p_y$ and $y$ with $p_x$,

$$
L=xp_y-yp_x
$$

is Hermitian. Using $p_xx=xp_x-i\hbar$ and its $y$ analogue,

$$
D=\frac12(xp_x+p_xx+yp_y+p_yy)
=-i\hbar(x\partial_x+y\partial_y+1),
$$

so $D$ is Hermitian as well.

Finally set $R=x\partial_y-y\partial_x$ and $S=x\partial_x+y\partial_y$. Direct evaluation on a smooth test function gives $[R,S]=0$: rotations commute with radial dilations. The scalar term in $D$ also commutes with everything, and therefore

$$
\boxed{[L,D]=0}.
$$

## 9H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9h/a">a</h3>

↑ **Parent:** [9H](#9h)

<h4 id="9h/a/solution">Solution</h4>

↑ **Parent:** [A](#9h/a)

States $i,j\in S$ [communicate](../../../markov-process.md#communicating-states) when each is accessible from the other: there exist nonnegative integers $m,n$ such that $P^m(i,j)>0$ and $P^n(j,i)>0$. A [communicating class](../../../markov-process.md#communicating-class) is an equivalence class for this relation.

<h3 id="9h/b">b</h3>

↑ **Parent:** [9H](#9h)

<h4 id="9h/b/solution">Solution</h4>

↑ **Parent:** [B](#9h/b)

The [period of a state in a Markov chain](../../../markov-process.md#period-of-a-state-in-a-markov-chain) $a$ is

$$
\boxed{d(a)=\gcd\{n\geq1:P^n(a,a)>0\}}.
$$

A state is aperiodic when this greatest common divisor is one.

<h3 id="9h/c">c</h3>

↑ **Parent:** [9H](#9h)

<h4 id="9h/c/solution">Solution</h4>

↑ **Parent:** [C](#9h/c)

Suppose $a$ and $b$ communicate. Choose $r,s$ with $P^r(a,b)>0$ and $P^s(b,a)>0$. Then $r+s$ is a possible return time to $a$, so $d(a)$ divides $r+s$. If $n$ is any possible return time to $b$, concatenating the paths gives a return to $a$ of length $r+n+s$. Thus $d(a)$ also divides $r+n+s$, and subtraction shows that $d(a)$ divides every such $n$. Therefore $d(a)\mid d(b)$. Interchanging $a$ and $b$ gives the reverse divisibility, so

$$
\boxed{d(a)=d(b)}.
$$

**Hence [period is constant on a communicating class](../../../markov-process.md#period-is-constant-on-a-communicating-class).**

## 10F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10f/solution">Solution</h3>

↑ **Parent:** [10F](#10f)

The [symmetric bilinear form associated with a quadratic form](../../../linear-algebra.md#polarization-identity) is obtained by polarization:

$$
\boxed{\phi(u,v)=\frac12\bigl(q(u+v)-q(u)-q(v)\bigr)},
\qquad q(v)=\phi(v,v).
$$

To diagonalize it, argue by induction on $\dim V$. If $\phi(v,v)=0$ for every $v$, polarization gives $\phi=0$, so every basis works. Otherwise choose $e$ with $\phi(e,e)\ne0$. Then

$$
V=\operatorname{span}(e)\oplus e^\perp,
\qquad
v=\frac{\phi(v,e)}{\phi(e,e)}e+\left(v-\frac{\phi(v,e)}{\phi(e,e)}e\right),
$$

and diagonalize the restriction to $e^\perp$ inductively. Thus some basis gives a diagonal matrix with positive, negative, and zero entries. By [Sylvester's law of inertia](../../../linear-algebra.md#sylvester-s-law-of-inertia), their counts $n_+,n_-,n_0$ are basis-independent. In the convention relevant here, the [signature of a quadratic form](../../../linear-algebra.md#signature-of-a-quadratic-form) is

$$
\boxed{\operatorname{sig}(q)=n_+-n_-}.
$$

Suppose $R$ lies in the [radical of a bilinear form](../../../linear-algebra.md#radical-of-a-bilinear-form), so $\phi(r,v)=0$ for all $r\in R,v\in V$. Then $q(r)=0$ and

$$
q(v+r)=q(v)+2\phi(v,r)+q(r)=q(v).
$$

Hence $q'(v+R)=q(v)$ is a well-defined quadratic form on the [quotient vector space](../../../vector-space.md#quotient-vector-space) $V/R$. In an adapted diagonal basis, quotienting by $R$ merely removes zero diagonal directions, so $n_+$ and $n_-$, and therefore the signature, are unchanged.

Now let $W=\operatorname{span}(e,f)$. Its Gram matrix is

$$
\begin{pmatrix}0&1\\1&\phi(f,f)\end{pmatrix},
$$

which has determinant $-1$. Thus $W$ is nondegenerate and has one positive and one negative square: it is a [hyperbolic plane](../../../linear-algebra.md#hyperbolic-plane-quadratic-form) and has signature zero. Nondegeneracy gives the orthogonal direct sum

$$
\boxed{V=W\oplus U,\qquad U=W^\perp}.
$$

Signature is additive under orthogonal direct sums, so

$$
\boxed{\operatorname{sig}(q|_U)=\operatorname{sig}(q)-\operatorname{sig}(q|_W)=\operatorname{sig}(q).}
$$

## 11G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11g/a">a</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/a/solution">Solution</h4>

↑ **Parent:** [A](#11g/a)

The [Eisenstein integers](../../../commutative-algebra.md#eisenstein-integer) are $\mathbb Z[\omega]$, where $\omega^2+\omega+1=0$. Their multiplicative [algebraic norm](../../../commutative-algebra.md#eisenstein-integer-norm) is

$$
N(a+b\omega)=(a+b\omega)(a+b\overline\omega)=a^2-ab+b^2.
$$

Given $\alpha,\beta\ne0$, choose an Eisenstein integer $q$ nearest to the complex number $\alpha/\beta$. The hexagonal lattice has covering radius $1/\sqrt3$, so

$$
\left|\frac\alpha\beta-q\right|\leq\frac1{\sqrt3}<1.
$$

With $r=\alpha-q\beta$, multiplicativity gives

$$
N(r)=N(\beta)\left|\frac\alpha\beta-q\right|^2<N(\beta).
$$

Thus division with remainder decreases the nonnegative integer norm, proving that $\boxed{\mathbb Z[\omega]\text{ is a Euclidean domain}}$.

<h3 id="11g/b">b</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/b/solution">Solution</h4>

↑ **Parent:** [B](#11g/b)

Every [Euclidean domain](../../../commutative-algebra.md#euclidean-domain) is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain): in a nonzero ideal choose an element of least positive Euclidean value and divide every other element by it; minimality forces every remainder to vanish. Every principal ideal domain is a [unique factorization domain](../../../algebra.md#unique-factorization-domain): the ascending-chain condition supplies factorizations into irreducibles, and [Euclid lemma](../../../number-theory.md#euclid-lemma) follows because every irreducible generates a prime ideal. Therefore

$$
\boxed{\mathbb Z[\omega]\text{ is a unique factorization domain}}.
$$

<h3 id="11g/c">c</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/c/solution">Solution</h4>

↑ **Parent:** [C](#11g/c)

Factor the equation in the Eisenstein integers:

$$
x^2-x+1=(x+\omega)(x+\omega^2)=y^3.
$$

Let $\pi=1-\omega$. Its norm is $3$, and

$$
\pi^2=-3\omega,
$$

so $3$ is a unit times $\pi^2$. Suppose $x\equiv2\pmod3$, say $x=3k+2$. Since $\omega=1-\pi$,

$$
x+\omega=3(k+1)-\pi.
$$

The first term is divisible by $\pi^2$ and the second has [discrete valuation](../../../commutative-algebra.md#discrete-valuation) exactly one, so $v_\pi(x+\omega)=1$. Conjugation gives $v_\pi(x+\omega^2)=1$ as well. Consequently

$$
v_\pi(x^2-x+1)=2.
$$

But $v_\pi(y^3)=3v_\pi(y)$ is divisible by three, a contradiction. Hence

$$
\boxed{x\not\equiv2\pmod3}.
$$

## 12E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12e/a">a</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/a/solution">Solution</h4>

↑ **Parent:** [A](#12e/a)

A local form of the [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem) is as follows. Let $F(t,y)$ be continuous on a rectangle about $(t_0,y_0)$ and uniformly [Lipschitz](../../../real-analysis.md#lipschitz-continuity) in $y$ there. Then some interval about $t_0$ admits a unique continuously differentiable solution of

$$
y'(t)=F(t,y(t)),
\qquad y(t_0)=y_0.
$$

The solution is the unique fixed point of the associated integral operator. If $F$ is continuous on $[a,b]\times\mathbb R^n$ and globally Lipschitz in $y$ with one constant, the solution exists uniquely throughout $[a,b]$.

<h3 id="12e/b">b</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/b/i">i</h4>

↑ **Parent:** [B](#12e/b)

<h5 id="12e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#12e/b/i)

Since $1\leq t\leq b$ and $c\geq0$,

$$
b^{-c}\leq t^{-c}\leq1.
$$

Taking suprema gives

$$
\boxed{b^{-c}\|f\|_\infty\leq\|f\|_c\leq\|f\|_\infty}.
$$

**Thus the weighted norm and the usual [uniform norm](../../../functional-analysis.md#supremum-norm) are [equivalent norms](../../../functional-analysis.md#equivalent-norms).**

<h4 id="12e/b/ii">ii</h4>

↑ **Parent:** [B](#12e/b)

<h5 id="12e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12e/b/ii)

For $f,g\in X$, the Lipschitz condition gives

$$
\begin{aligned}
t^{-c}\|\phi(f)(t)-\phi(g)(t)\|
&\leq Mt^{-c}\int_1^t\|f(l)-g(l)\|\,dl\\
&\leq M\|f-g\|_c\,t^{-c}\int_1^t l^c\,dl\\
&=\frac{M}{c+1}(t-t^{-c})\|f-g\|_c\\
&\leq\frac{Mb}{c+1}\|f-g\|_c.
\end{aligned}
$$

Choose $c$ so that $c+1>Mb$. Then $\phi$ is a [contraction mapping](../../../analysis.md#contraction-mapping). The space $X$ is complete in the sup norm, and therefore also in the equivalent weighted norm.

For initial value $y_0$, define

$$
\Phi_{y_0}(f)(t)=y_0+\int_1^tF(l,f(l))\,dl.
$$

It has the same contraction constant. The [Banach fixed-point theorem](../../../analysis.md#contraction-mapping-theorem) gives a unique fixed point $f$, which satisfies the integral equation. The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) then gives

$$
f'(t)=F(t,f(t)),
\qquad f(1)=y_0.
$$

Conversely every solution satisfies that integral equation, proving uniqueness on $[1,b]$. This weighted-norm argument is the [Bielecki norm method](../../../differential-equation.md#bielecki-norm-method).

## 13F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="13f/solution">Solution</h3>

↑ **Parent:** [13F](#13f)

For a closed piecewise smooth path $\gamma$ avoiding $w$, its [winding number](../../../complex-analysis.md#winding-number) is

$$
\boxed{n(\gamma,w)=\frac1{2\pi i}\int_\gamma\frac{dz}{z-w}}.
$$

A meromorphic function has a zero of order $m>0$ at $z_0$ when

$$
f(z)=(z-z_0)^m g(z),
\qquad g(z_0)\ne0,
$$

with $g$ holomorphic; it has a pole of order $m$ at $w_0$ when $(z-w_0)^mf(z)$ extends holomorphically and nonvanishingly there.

The [argument principle](../../../complex-analysis.md#argument-principle) states that, if $f$ has no zero or pole on $\gamma$,

$$
\frac1{2\pi i}\int_\gamma\frac{f'(z)}{f(z)}\,dz
=\sum_a n(\gamma,a)\operatorname{ord}_a(f).
$$

For a positively oriented simple contour this is the number of enclosed zeros minus poles, counted with multiplicity. It follows from the [residue theorem](../../../analysis.md#residue-theorem) because the residue of $f'/f$ at a zero of order $m$ is $m$, while at a pole of order $m$ it is $-m$.

Let

$$
p(z)=z^4+10z^3+4z^2+10z+5.
$$

On the imaginary axis,

$$
p(iy)=\underbrace{(y^4-4y^2+5)}_{(y^2-2)^2+1>0}
+10iy(1-y^2).
$$

Thus $p(iy)$ always lies in the open right half-plane, has no zero there, and its continuous argument has net change zero as the imaginary-axis part of a large right-half-disc contour is traversed. On the right semicircle, $p(z)/z^4\to1$ uniformly, so the argument change tends to that of $z^4$, namely $4\pi$. The argument principle therefore gives

$$
\boxed{\frac{4\pi}{2\pi}=2}
$$

roots in the open right half-plane, counted with multiplicity.

## 14E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="14e/a">a</h3>

↑ **Parent:** [14E](#14e)

<h4 id="14e/a/solution">Solution</h4>

↑ **Parent:** [A](#14e/a)

A geodesic triangulation of a closed smooth surface decomposes it into finitely many triangular discs whose edges are geodesic arcs and whose intersections are common faces. Its Euler number is

$$
\chi=V-E+F.
$$

The [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) for a closed surface states

$$
\int_S K\,dA=2\pi\chi(S).
$$

For any triangulation of a closed surface, each triangular face has three edges and every edge belongs to two faces, so $3F=2E$. The sum of all vertex valencies is $2E$. Hence the average valency is

$$
\overline d=\frac{2E}{V}.
$$

The [torus](../../../topology.md#torus) has [Euler characteristic](../../../homology.md#euler-characteristic) $\chi=V-E+F=0$. Using $F=2E/3$ gives $V-E/3=0$, so $E=3V$ and

$$
\boxed{\overline d=6}.
$$

<h3 id="14e/b">b</h3>

↑ **Parent:** [14E](#14e)

<h4 id="14e/b/i">i</h4>

↑ **Parent:** [B](#14e/b)

<h5 id="14e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#14e/b/i)

For the [sphere](../../../geometry-and-topology.md#sphere), $\chi=2$, and the same incidence identity gives

$$
2=V-\frac E3,
\qquad E=3(V-2).
$$

Therefore

$$
\boxed{\overline d=\frac{2E}{V}=6-\frac{12}{V}<6}.
$$

<h4 id="14e/b/ii">ii</h4>

↑ **Parent:** [B](#14e/b)

<h5 id="14e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#14e/b/ii)

Subdividing one face in the stated way adds one vertex, three edges, and two net faces. Starting from any spherical triangulation and repeating this operation makes $V\to\infty$ while preserving the sphere. Since every resulting average is

$$
\overline d=6-\frac{12}{V},
$$

these averages approach six from below. Thus spherical triangulations can have average valency arbitrarily close to six.

<h3 id="14e/c">c</h3>

↑ **Parent:** [14E](#14e)

<h4 id="14e/c/solution">Solution</h4>

↑ **Parent:** [C](#14e/c)

If $K<0$ everywhere, compactness makes the integral negative, so $\chi(S)<0$. For every triangulation, $3F=2E$ again yields the general identity

$$
\overline d=6-\frac{6\chi(S)}{V}.
$$

Since $V\geq1$ and $\chi(S)<0$,

$$
\boxed{6<\overline d\leq6-6\chi(S)}.
$$

This supplies bounds depending only on the surface.

## 15D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="15d/solution">Solution</h3>

↑ **Parent:** [15D](#15d)

In the sense of [distribution theory](../../../distribution-theory.md), $H'(t)=\delta(t)$. Since $\sin(\alpha t)$ vanishes at zero,

$$
\psi'(t)=H(t)\cos(\alpha t),
\qquad
\psi''(t)=\delta(t)-\alpha H(t)\sin(\alpha t),
$$

and therefore

$$
\boxed{\psi''+\alpha^2\psi=\delta(t)}.
$$

Let $G_{\rm ret}(\mathbf x,t;\mathbf y)$ solve

$$
(\partial_t^2-c^2\nabla^2)G_{\rm ret}
=\delta(t)\delta^{(3)}(\mathbf x-\mathbf y),
\qquad G_{\rm ret}=0\quad(t<0).
$$

The spatial [Fourier transform](../../../analysis.md#fourier-transform) turns this into the preceding oscillator equation with $\alpha=ck$, so

$$
\widehat G(\mathbf k,t)=H(t)\frac{\sin(ckt)}{ck}.
$$

Inverting with the supplied radial integral gives the three-dimensional [retarded Green function](../../../quantum-field-theory.md#retarded-green-function)

$$
\boxed{G_{\rm ret}(\mathbf x,t;\mathbf y)
=\frac{H(t)}{4\pi c|\mathbf x-\mathbf y|}
\delta(|\mathbf x-\mathbf y|-ct)
=\frac{\delta(t-|\mathbf x-\mathbf y|/c)}{4\pi c^2|\mathbf x-\mathbf y|}}.
$$

For zero initial displacement and initial velocity $f$, convolution with this kernel gives the [Kirchhoff formula](../../../wave-equation.md#kirchhoff-formula)

$$
\begin{aligned}
u(\mathbf x,t)
&=\int_{\mathbb R^3}G_{\rm ret}(\mathbf x,t;\mathbf y)f(\mathbf y)\,d^3y\\
&=\frac{t}{4\pi}\int_{S^2}f(\mathbf x+ct\,\boldsymbol\omega)\,d\Omega
=t\langle f\rangle_t.
\end{aligned}
$$

**Thus the value at $(\mathbf x,t)$ depends only on the initial data on the sphere of radius $ct$, not on its interior. This is the [Huygens principle](../../../wave-equation.md#strong-huygens-principle) and describes propagation at the finite wave speed $c$.**

## 16B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="16b/solution">Solution</h3>

↑ **Parent:** [16B](#16b)

Inside the [infinite square well](../../../quantum-mechanics.md#infinite-square-well), the stationary [Schrödinger equation](../../../physics.md#schrodinger-equation) for unit mass is

$$
-\frac{\hbar^2}{2}\psi''=E\psi,
\qquad \psi(0)=\psi(\pi)=0.
$$

Its normalized eigenstates and energies are

$$
\boxed{\psi_n(x)=\sqrt{\frac2\pi}\sin(nx),
\qquad E_n=\frac{\hbar^2n^2}{2}},
\qquad n=1,2,\ldots.
$$

The general normalized time-dependent solution is

$$
\boxed{\Psi(x,t)=\sum_{n=1}^\infty c_n\psi_n(x)e^{-iE_nt/\hbar},
\qquad \sum_{n=1}^\infty|c_n|^2=1}.
$$

Immediately after removing the barrier, the normalized wavefunction is

$$
\Psi(x,0)=
\begin{cases}
\sqrt{4/\pi}\sin(2x),&0\leq x\leq\pi/2,\\
0,&\pi/2<x\leq\pi.
\end{cases}
$$

Its [Fourier sine series](../../../fourier-series.md#fourier-sine-series) coefficients in the full-well basis are

$$
c_n=\frac{\sqrt8}{\pi}\int_0^{\pi/2}\sin(nx)\sin(2x)\,dx.
$$

They are

$$
c_2=\frac1{\sqrt2},
\qquad
c_n=\frac{4\sqrt2}{\pi}\frac{\sin(n\pi/2)}{4-n^2}\quad(n\ne2).
$$

The [Born rule](../../../quantum-mechanics.md#born-rule) therefore gives

$$
\boxed{
\mathbb P(E_n)=
\begin{cases}
\dfrac12,&n=2,\\[4pt]
\dfrac{32}{\pi^2(n^2-4)^2},&n\text{ odd},\\[4pt]
0,&n\text{ even and }n\ne2.
\end{cases}}
$$

## 17A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="17a/solution">Solution</h3>

↑ **Parent:** [17A](#17a)

For a boost of speed $v$ in the $x$ direction, with

$$
\gamma=\frac1{\sqrt{1-v^2/c^2}},
$$

the [Lorentz transformation of electromagnetic fields](../../../electromagnetism.md#lorentz-transformation-of-electromagnetic-fields) is

$$
\begin{array}{lll}
E'_x=E_x,&E'_y=\gamma(E_y-vB_z),&E'_z=\gamma(E_z+vB_y),\\
B'_x=B_x,&B'_y=\gamma(B_y+vE_z/c^2),&B'_z=\gamma(B_z-vE_y/c^2).
\end{array}
$$

Expanding $E'_yB'_y+E'_zB'_z$, the mixed terms cancel and the remaining transverse terms acquire the factor $\gamma^2(1-v^2/c^2)=1$. Together with the unchanged longitudinal product, this proves the Lorentz invariant

$$
\boxed{\mathbf E'\cdot\mathbf B'=\mathbf E\cdot\mathbf B}.
$$

An independent invariant is

$$
\boxed{E^2-c^2B^2}.
$$

If only $E_y=E$ and $B_y=B$ are nonzero, then

$$
\mathbf E'=(0,\gamma E,\gamma vB),
\qquad
\mathbf B'=(0,\gamma B,-\gamma vE/c^2),
$$

and direct subtraction gives

$$
E'^2-c^2B'^2
=\gamma^2(1-v^2/c^2)(E^2-c^2B^2)
=E^2-c^2B^2.
$$

Now put $cB=\lambda E$ and $\beta=v/c$. Invariance of the dot product gives $\mathbf E'\cdot\mathbf B'=\lambda E^2/c$, while the displayed components give

$$
E'^2=\gamma^2E^2(1+\lambda^2\beta^2),
\qquad
B'^2=\frac{\gamma^2E^2}{c^2}(\lambda^2+\beta^2).
$$

Hence

$$
\boxed{\cos\theta=
\frac{\lambda(1-\beta^2)}{sqrt{(1+\lambda^2\beta^2)(\lambda^2+\beta^2)}}}.
$$

At $\beta=0$ this equals $\operatorname{sgn}\lambda$, and as $|\beta|\uparrow1$ it tends continuously to zero with the same sign. Thus boosts realize every $0\leq\theta<\pi/2$ when $\lambda>0$, and every $\pi/2<\theta\leq\pi$ when $\lambda<0$.

## 18C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="18c/solution">Solution</h3>

↑ **Parent:** [18C](#18c)

Let the perturbed interface be $z=\eta(x,y,t)$. For inviscid disturbances about rest, the initially irrotational velocities remain potential flows,

$$
\mathbf u_i=\nabla\phi_i,
\qquad \nabla^2\phi_i=0,
$$

in the upper layer $0<z<h$ and lower layer $-h<z<0$. The rigid walls impose [no-penetration boundary condition](../../../viscous-fluid-flow.md#no-penetration-boundary-condition)

$$
\partial_z\phi_1=0\ (z=h),
\qquad
\partial_z\phi_2=0\ (z=-h),
$$

and zero normal derivative at $x,y=0,2h$. Linearizing the kinematic and pressure-continuity conditions at $z=0$ gives

$$
\eta_t=\partial_z\phi_1=\partial_z\phi_2,
\qquad
\rho_1(\phi_{1t}+g\eta)=\rho_2(\phi_{2t}+g\eta).
$$

The horizontal Neumann eigenfunctions are

$$
\cos\frac{m\pi x}{2h}\cos\frac{n\pi y}{2h},
\qquad
k=\frac\pi{2h}\sqrt{m^2+n^2},
$$

where $m,n$ are nonnegative integers, not both zero. For time dependence $e^{-i\omega t}$, the vertical factors satisfying the rigid lids are

$$
\phi_1=A_1\cosh k(z-h),
\qquad
\phi_2=A_2\cosh k(z+h).
$$

The kinematic condition gives their interface values

$$
\phi_1(0)=\frac{i\omega}{k}\coth(kh)\eta,
\qquad
\phi_2(0)=-\frac{i\omega}{k}\coth(kh)\eta.
$$

Substitution into the dynamic condition yields the [interfacial gravity-wave dispersion relation](../../../gravity-wave.md#interfacial-gravity-wave-dispersion-relation)

$$
\boxed{\omega^2=\frac{\rho_2-\rho_1}{\rho_1+\rho_2}gk\tanh(kh)}.
$$

For $\rho_2>\rho_1$, the lowest nontrivial wavenumber is $k=\pi/(2h)$, with the two degenerate modes $(m,n)=(1,0)$ and $(0,1)$. If $\rho_1\ll\rho_2$, the relation reduces to the finite-depth free-surface result $\omega^2\simeq gk\tanh(kh)$. If $\rho_1>\rho_2$, then $\omega^2<0$ and disturbances grow exponentially: this is the [Rayleigh-Taylor instability](../../../continuum-mechanics.md#rayleigh-taylor-instability).

## 19C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="19c/a">a</h3>

↑ **Parent:** [19C](#19c)

<h4 id="19c/a/solution">Solution</h4>

↑ **Parent:** [A](#19c/a)

Bilinearity and symmetry follow from the corresponding properties of the [integral](../../../calculus.md#integral). Since $w(x)>0$,

$$
\langle f,f\rangle=\int_a^b f(x)^2w(x)\,dx\geq0.
$$

If this integral is zero, the nonnegative continuous integrand must vanish everywhere, so $f=0$. Therefore the displayed formula is a real [inner product](../../../linear-algebra.md#inner-product) on $C[a,b]$.

<h3 id="19c/b">b</h3>

↑ **Parent:** [19C](#19c)

<h4 id="19c/b/solution">Solution</h4>

↑ **Parent:** [B](#19c/b)

Inductively, $p_n$ is monic of degree $n$, because the leading term of $p_{n+1}$ comes only from $xp_n$. Assume $p_0,\ldots,p_n$ are mutually orthogonal. The definitions give

$$
\langle p_{n+1},p_n\rangle
=\langle xp_n,p_n\rangle-\alpha_n\langle p_n,p_n\rangle=0.
$$

Using the preceding recurrence in the form

$$
xp_{n-1}=p_n+\alpha_{n-1}p_{n-1}+\beta_{n-1}p_{n-2}
$$

gives

$$
\langle xp_n,p_{n-1}\rangle
=\langle p_n,xp_{n-1}\rangle
=\langle p_n,p_n\rangle,
$$

so $\langle p_{n+1},p_{n-1}\rangle=0$ by the definition of $\beta_n$. If $j\leq n-2$, then $xp_j$ lies in the span of $p_{j-1},p_j,p_{j+1}$, all orthogonal to $p_n$, and the remaining recurrence terms are also orthogonal to $p_j$. Hence $\langle p_{n+1},p_j\rangle=0$. Induction proves that the recurrence defines monic [orthogonal polynomials](../../../numerical-analysis.md#orthogonal-polynomial).

<h3 id="19c/c">c</h3>

↑ **Parent:** [19C](#19c)

<h4 id="19c/c/solution">Solution</h4>

↑ **Parent:** [C](#19c/c)

The [probabilists' Hermite polynomials](../../../numerical-analysis.md#probabilists-hermite-polynomial) satisfy

$$
\mathrm{He}'_n=n\mathrm{He}_{n-1},
\qquad
x\mathrm{He}_n=\mathrm{He}_{n+1}+n\mathrm{He}_{n-1},
$$

which follow by differentiating the Rodrigues formula. Thus

$$
\boxed{\mathrm{He}_{n+1}=x\mathrm{He}_n-n\mathrm{He}_{n-1}},
$$

so $\alpha_n=0$ and $\beta_n=n$.

For the squared norm, substitute the Rodrigues formula and integrate by parts $n$ times. All boundary terms vanish under the Gaussian weight, and $\mathrm{He}_n^{(n)}=n!$, giving

$$
\begin{aligned}
\langle\mathrm{He}_n,\mathrm{He}_n\rangle
&=(-1)^n\int_{-\infty}^{\infty}
\mathrm{He}_n(x)\frac{d^n}{dx^n}e^{-x^2/2}\,dx\\
&=n!\int_{-\infty}^{\infty}e^{-x^2/2}\,dx
=\boxed{n!\sqrt{2\pi}}.
\end{aligned}
$$

<h3 id="19c/d">d</h3>

↑ **Parent:** [19C](#19c)

<h4 id="19c/d/solution">Solution</h4>

↑ **Parent:** [D](#19c/d)

Let $x_1,\ldots,x_N$ be the distinct real roots of $\mathrm{He}_N$. The [Gauss-Hermite quadrature](../../../numerical-analysis.md#gauss-hermite-quadrature) rule is

$$
\int_{-\infty}^{\infty}f(x)e^{-x^2/2}\,dx
\approx\sum_{j=1}^Nw_jf(x_j),
$$

where $w_j$ is the weighted integral of the $j$th [Lagrange interpolation polynomial](../../../numerical-analysis.md#lagrange-polynomial). Equivalently,

$$
w_j=\frac{N!\sqrt{2\pi}}{N^2\mathrm{He}_{N-1}(x_j)^2}>0.
$$

The orthogonality of $\mathrm{He}_N$ makes the rule exact for every polynomial of degree at most

$$
\boxed{2N-1}.
$$

## 20H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="20h/a">a</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/a/solution">Solution</h4>

↑ **Parent:** [A](#20h/a)

The [sample mean](../../../variance.md#sample-mean) is

$$
\boxed{\overline X\sim N\left(\mu,\frac{\sigma^2}{n}\right)}.
$$

Write the Gaussian sample vector as its orthogonal projection onto the span of $(1,\ldots,1)$ plus its projection onto the orthogonal complement. These two Gaussian projections are independent. Their squared standardized lengths give [Cochran's theorem](../../../statistical-modelling.md#cochran-s-theorem):

$$
\boxed{\frac{S_{XX}}{\sigma^2}\sim\chi^2_{n-1},
\qquad \overline X\ \text{is independent of }S_{XX}}.
$$

<h3 id="20h/b">b</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/b/solution">Solution</h4>

↑ **Parent:** [B](#20h/b)

Combining the independent standard normal variable $\sqrt n(\overline X-\mu)/\sigma$ with the independent chi-squared variable $S_{XX}/\sigma^2$ gives

$$
\boxed{
\frac{\sqrt n(\overline X-\mu)}{\sqrt{S_{XX}/(n-1)}}
\sim t_{n-1}},
$$

the [Student's t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution) with $n-1$ degrees of freedom.

<h3 id="20h/c">c</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/c/i">i</h4>

↑ **Parent:** [C](#20h/c)

<h5 id="20h/c/i/solution">Solution</h5>

↑ **Parent:** [I](#20h/c/i)

Let $z_p$ denote the $p$-quantile of the standard normal distribution. Since the variance is known,

$$
\frac{\sqrt n(\overline X-\mu)}{\sigma}\sim N(0,1),
$$

so a $100(1-\alpha)\%$ [confidence interval](../../../statistical-inference.md#confidence-interval) is

$$
\boxed{\overline X\pm z_{1-\alpha/2}\frac\sigma{\sqrt n}}.
$$

<h4 id="20h/c/ii">ii</h4>

↑ **Parent:** [C](#20h/c)

<h5 id="20h/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#20h/c/ii)

Let $t_{\nu,p}$ denote the $p$-quantile of [Student's t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution). Part (b) gives the [Student t confidence interval](../../../statistical-inference.md#student-t-confidence-interval)

$$
\boxed{\overline X\pm t_{n-1,1-\alpha/2}
\sqrt{\frac{S_{XX}}{n(n-1)}}}.
$$

<h4 id="20h/c/iii">iii</h4>

↑ **Parent:** [C](#20h/c)

<h5 id="20h/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#20h/c/iii)

Let $\chi^2_{\nu,p}$ denote the $p$-quantile of the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution). Since $S_{XX}/\sigma^2\sim\chi^2_{n-1}$, inversion of the central probability event gives

$$
\boxed{
\left[
\frac{S_{XX}}{\chi^2_{n-1,1-\alpha/2}},
\frac{S_{XX}}{\chi^2_{n-1,\alpha/2}}
\right]}
$$

as a $100(1-\alpha)\%$ confidence interval for $\sigma^2$.

<h3 id="20h/d">d</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/d/solution">Solution</h4>

↑ **Parent:** [D](#20h/d)

For an independent second sample, let

$$
\widetilde S_{XX}=\sum_{j=1}^{\widetilde n}
(\widetilde X_j-\overline{\widetilde X})^2.
$$

Under $H_0:\sigma^2=\widetilde\sigma^2$, independence and the two chi-squared laws give the [F-distribution](../../../continuous-probability-distribution.md#f-distribution)

$$
\boxed{F=
\frac{S_{XX}/(n-1)}{\widetilde S_{XX}/(\widetilde n-1)}
\sim F_{n-1,\widetilde n-1}}.
$$

For the one-sided alternative $\sigma^2>\widetilde\sigma^2$, reject for large $F$, using the upper $\alpha$ critical value.

**No values of the unknown means enter this statistic:** centering by the sample means removes them. If both means are known, one may instead use sums about the known means; the corresponding degrees of freedom are $n$ and $\widetilde n$, rather than $n-1$ and $\widetilde n-1$. Thus knowledge of the means changes the degrees of freedom and critical value, while the variance-ratio principle is unchanged.

## 21H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="21h/a">a</h3>

↑ **Parent:** [21H](#21h)

<h4 id="21h/a/solution">Solution</h4>

↑ **Parent:** [A](#21h/a)

Choose a set $B$ of $m$ column indices for which the square matrix $A_B$ is invertible. The associated [basic solution](../../../mathematical-optimization.md#basic-solution) sets $x_j=0$ for $j\notin B$ and solves $A_Bx_B=b$. It is a [basic feasible solution](../../../mathematical-optimization.md#basic-feasible-solution) when all its coordinates are nonnegative.

Let $x$ be a basic feasible solution with basis $B$. If $x=(y+z)/2$ for $y,z\in X(b)$, then $x_j=0$ and nonnegativity force $y_j=z_j=0$ for every $j\notin B$. Since $A_By_B=A_Bz_B=b$ and $A_B$ is invertible, $y=z=x$. Thus $x$ is an [extreme point](../../../mathematical-optimization.md#extreme-point).

Conversely, let $x$ be extreme and let $S=\{j:x_j>0\}$. If $|S|>m$, the corresponding columns are linearly dependent, so there is a nonzero vector $d$ supported on $S$ with $Ad=0$. For sufficiently small $\varepsilon>0$, both $x+\varepsilon d$ and $x-\varepsilon d$ remain nonnegative and feasible, contradicting extremality. Hence $|S|\leq m$. Enlarge $S$ to a set $B$ of $m$ indices. By the hypotheses $A_B$ is invertible, and $x$ is the resulting basic feasible solution. Therefore

$$
\boxed{\text{the extreme points of }X(b)\text{ are exactly the basic feasible solutions}}.
$$

<h3 id="21h/b">b</h3>

↑ **Parent:** [21H](#21h)

<h4 id="21h/b/solution">Solution</h4>

↑ **Parent:** [B](#21h/b)

Introduce slack variables $s_1,s_2,s_3\geq0$ after rewriting the third inequality as $x_1-x_2+x_3\leq2$. The initial dictionary is

$$
\begin{aligned}
s_1&=14-x_1-3x_2-x_3,\\
s_2&=5-4x_1-3x_2-2x_3,\\
s_3&=2-x_1+x_2-x_3,\\
z&=4x_1+3x_2+7x_3.
\end{aligned}
$$

In the [simplex method](../../../mathematical-optimization.md#simplex-method), $x_3$ enters first because it has the largest positive objective coefficient. The ratio test makes $s_3$ leave, and substitution gives

$$
\begin{aligned}
x_3&=2-x_1+x_2-s_3,\\
s_1&=12-4x_2+s_3,\\
s_2&=1-2x_1-5x_2+2s_3,\\
z&=14-3x_1+10x_2-7s_3.
\end{aligned}
$$

Next $x_2$ enters and $s_2$ leaves. Solving for $x_2$ produces the final objective row

$$
z=16-7x_1-3s_3-2s_2.
$$

All reduced costs are now nonpositive, so the dictionary is optimal at the nonbasic values $x_1=s_2=s_3=0$. Therefore

$$
\boxed{(x_1,x_2,x_3)=\left(0,\frac15,\frac{11}{5}\right),
\qquad z_{\max}=16}.
$$

The first constraint has slack $s_1=56/5$, while the second and third constraints are active.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
