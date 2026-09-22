# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2020/paperia_1_2020.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2020/paperia_1_2020.pdf)

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
  - [v](#1c/v)
    - [Solution](#1c/v/solution)
- [2A](#2a)
  - [Solution](#2a/solution)
- [3E](#3e)
  - [a](#3e/a)
    - [Solution](#3e/a/solution)
  - [b](#3e/b)
    - [Solution](#3e/b/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5C](#5c)
  - [a](#5c/a)
    - [Solution](#5c/a/solution)
  - [b](#5c/b)
    - [Solution](#5c/b/solution)
- [6A](#6a)
  - [Solution](#6a/solution)
- [7A](#7a)
  - [Solution](#7a/solution)
- [8A](#8a)
  - [Solution](#8a/solution)
- [9D](#9d)
  - [a](#9d/a)
    - [Solution](#9d/a/solution)
  - [b](#9d/b)
    - [i](#9d/b/i)
      - [Solution](#9d/b/i/solution)
    - [ii](#9d/b/ii)
      - [Solution](#9d/b/ii/solution)
    - [iii](#9d/b/iii)
      - [Solution](#9d/b/iii/solution)
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
  - [c](#10f/c)
    - [Solution](#10f/c/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12F](#12f)
  - [a](#12f/a)
    - [Solution](#12f/a/solution)
  - [b](#12f/b)
    - [Solution](#12f/b/solution)
  - [c](#12f/c)
    - [Solution](#12f/c/solution)

## 1C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1c/i">i</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/i/solution">Solution</h4>

↑ **Parent:** [I](#1c/i)

Using [Euler's formula](../../../complex-analysis.md#euler-s-formula), the [complex exponential function](../../../calculus.md#complex-exponential-function) satisfies

$$
e^{x+iy}=e^x(\cos y+i\sin y).
$$

Hence

$$
\boxed{\operatorname{Re}(e^z)=e^x\cos y,
\qquad \operatorname{Im}(e^z)=e^x\sin y}.
$$

<h3 id="1c/ii">ii</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1c/ii)

The [complex sine function](../../../calculus.md#complex-sine-function) obeys

$$
\sin(x+iy)=\sin x\cosh y+i\cos x\sinh y.
$$

Thus

$$
\boxed{\operatorname{Re}(\sin z)=\sin x\cosh y,
\qquad \operatorname{Im}(\sin z)=\cos x\sinh y}.
$$

<h3 id="1c/iii">iii</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1c/iii)

Since $z\overline z=|z|^2=x^2+y^2$, the [complex conjugate](../../../complex-analysis.md#complex-conjugate) gives

$$
\frac1z-\frac1{\overline z}
=\frac{\overline z-z}{|z|^2}
=-\frac{2iy}{x^2+y^2}.
$$

Therefore

$$
\boxed{\operatorname{Re}=0,
\qquad \operatorname{Im}=-\frac{2y}{x^2+y^2}}.
$$

<h3 id="1c/iv">iv</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1c/iv)

Factor the expression using the [complex conjugate](../../../complex-analysis.md#complex-conjugate):

$$
\begin{aligned}
z^3-z^2\overline z-z\overline z^2+\overline z^3
&=(z+\overline z)(z-\overline z)^2\\
&=(2x)(2iy)^2=-8xy^2.
\end{aligned}
$$

It is real, so

$$
\boxed{\operatorname{Re}=-8xy^2,
\qquad \operatorname{Im}=0}.
$$

<h3 id="1c/v">v</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/v/solution">Solution</h4>

↑ **Parent:** [V](#1c/v)

All values of the [complex logarithm](../../../analysis.md#complex-logarithm) are

$$
w=\log|z|+i(\arg z+2\pi n),
\qquad n\in\mathbb Z.
$$

Because $x>0$, one may take the [complex argument](../../../complex-analysis.md#argument-complex-analysis) $\arg z=\arctan(y/x)$. Consequently

$$
\boxed{\operatorname{Re}w=\frac12\log(x^2+y^2),
\qquad
\operatorname{Im}w=\arctan\frac yx+2\pi n,quad n\in\mathbb Z}.
$$

## 2A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2a/solution">Solution</h3>

↑ **Parent:** [2A](#2a)

Invert the equation and regard $x$ as a function of $y$:

$$
\frac{dx}{dy}-x=e^{2y}.
$$

This is a [first-order linear differential equation](../../../differential-equation.md#first-order-linear-differential-equation). Multiplication by the [integrating factor](../../../differential-equation.md#integrating-factor) $e^{-y}$ gives

$$
\frac d{dy}(xe^{-y})=e^y,
$$

so $x=e^{2y}+Ce^y$. The initial condition $x=1$ at $y=0$ gives $C=0$. Hence $x=e^{2y}$ and

$$
\boxed{y(x)=\frac12\log x},
\qquad x>0.
$$

## 3E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3e/a">a</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/a/solution">Solution</h4>

↑ **Parent:** [A](#3e/a)

Define $F(x)=\int_a^x f(t)\,dt$. By the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus), $F'=f$. The [chain rule](../../../calculus.md#chain-rule) gives

$$
\frac d{du}F(g(u))=f(g(u))g'(u).
$$

Integrating from $\alpha$ to $\beta$ and using $g(\alpha)=a$, $g(\beta)=b$ yields the [change of variables formula](../../../calculus.md#change-of-variables-formula)

$$
\int_\alpha^\beta f(g(u))g'(u)\,du
=F(b)-F(a)=\int_a^b f(x)\,dx.
$$

The argument also covers a decreasing $g$ because both integrals are oriented.

<h3 id="3e/b">b</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/b/solution">Solution</h4>

↑ **Parent:** [B](#3e/b)

For $0<\varepsilon<e^{-1}$, set $u=\log(1/x)$. The ordinary [change of variables formula](../../../calculus.md#change-of-variables-formula) gives

$$
\int_\varepsilon^{e^{-1}}
\frac{dx}{x(\log(1/x))^\theta}
=\int_1^{\log(1/\varepsilon)}u^{-\theta}\,du.
$$

Taking $\varepsilon\downarrow0$ is exactly the defining [limit](../../../calculus.md#limit-of-a-function) of the [improper integral](../../../real-analysis.md#improper-integral). By the [improper power integral](../../../real-analysis.md#improper-power-integral), it converges for $\theta>1$, and

$$
\boxed{\int_0^{e^{-1}}
\frac{dx}{x(\log(1/x))^\theta}
=\int_1^\infty u^{-\theta}\,du
=\frac1{\theta-1}}.
$$

## 4F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

Let $Z_n$ be the size of generation $n$. This is a [Galton-Watson process](../../../probability-and-statistics.md#galton-watson-process) with offspring mean

$$
m=0\cdot\frac1{12}+1\cdot\frac12
+2\cdot\frac13+3\cdot\frac1{12}
=\frac{17}{12}.
$$

The [expected generation size in a Galton-Watson process](../../../probability-and-statistics.md#expected-generation-size-in-a-galton-watson-process) is therefore

$$
\boxed{\mathbb E Z_n=\left(\frac{17}{12}\right)^n}.
$$

Its [probability generating function](../../../probability-theory.md#probability-generating-function) is

$$
G(s)=\frac1{12}+\frac12s+\frac13s^2+\frac1{12}s^3.
$$

By the [Galton-Watson extinction fixed point](../../../probability-and-statistics.md#galton-watson-extinction-fixed-point), the extinction probability $q$ is the smallest solution in $[0,1]$ of $G(q)=q$. Factoring gives

$$
q^3+4q^2-6q+1=(q-1)(q^2+5q-1)=0,
$$

so $q=(\sqrt{29}-5)/2$. The probability of production continuing forever is

$$
\boxed{1-q=\frac{7-\sqrt{29}}2}.
$$

## 5C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5c/a">a</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/a/solution">Solution</h4>

↑ **Parent:** [A](#5c/a)

Expanding the squared [Euclidean distances](../../../topological-analysis.md#euclidean-distance) gives

$$
|\mathbf x-\mathbf a|^2=|\mathbf x-\mathbf b|^2
\iff
2(\mathbf b-\mathbf a)\mathbin\cdot\mathbf x
=|\mathbf b|^2-|\mathbf a|^2.
$$

Thus one may take

$$
\boxed{\mathbf n_{AB}=\frac{\mathbf b-\mathbf a}{|\mathbf b-\mathbf a|},
\qquad
p_{AB}=\frac{|\mathbf b|^2-|\mathbf a|^2}{2|\mathbf b-\mathbf a|}}.
$$

The normal is parallel to $\overrightarrow{AB}$, so $L_{AB}$ is its [perpendicular bisector](../../../geometry-and-topology.md#perpendicular-bisector). If $\mathbf x$ lies on both $L_{AB}$ and $L_{BC}$, then $|\mathbf x-\mathbf a|=|\mathbf x-\mathbf b|=|\mathbf x-\mathbf c|$, hence it also lies on $L_{CA}$. Geometrically, the three perpendicular bisectors of the noncollinear triangle concur at its [circumcenter](../../../geometry-and-topology.md#circumcenter).

<h3 id="5c/b">b</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/b/solution">Solution</h4>

↑ **Parent:** [B](#5c/b)

Assume the direction vectors are nonzero. The [cross product](../../../vector-space.md#cross-product) equation is equivalent to

$$
(\mathbf x-\mathbf a)\times\mathbf u=0,
$$

so $\mathbf x-\mathbf a$ is parallel to $\mathbf u$ and the locus is the line $\mathbf x=\mathbf a+\lambda\mathbf u$.

For nonparallel directions, $\mathbf u_1\times\mathbf u_2$ is normal to both lines. Projecting their displacement onto the corresponding [unit vector](../../../vector-space.md#unit-vector) gives the [distance between skew lines](../../../geometry-and-topology.md#distance-between-skew-lines)

$$
\boxed{d=
\frac{|(\mathbf a_2-\mathbf a_1)\mathbin\cdot
(\mathbf u_1\times\mathbf u_2)|}
{|\mathbf u_1\times\mathbf u_2|}}.
$$

If the directions are parallel, the corresponding formula is

$$
\boxed{d=\frac{|(\mathbf a_2-\mathbf a_1)\times\mathbf u_1|}{|\mathbf u_1|}}.
$$

## 6A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6a/solution">Solution</h3>

↑ **Parent:** [6A](#6a)

A matrix is [Hermitian](../../../hilbert-space.md#hermitian-operator) when $A^\dagger=A$, and [unitary](../../../linear-operator-theory.md#unitary-matrix) when $U^\dagger U=UU^\dagger=I$.

If $A\mathbf u=\lambda\mathbf u$ with $\mathbf u\ne0$, then

$$
\lambda\,\mathbf u^\dagger\mathbf u
=\mathbf u^\dagger A\mathbf u
=(\mathbf u^\dagger A\mathbf u)^*
=\lambda^*\mathbf u^\dagger\mathbf u,
$$

so every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is real. If $A\mathbf u=\lambda\mathbf u$ and $A\mathbf v=\mu\mathbf v$, then

$$
\mu\mathbf u^\dagger\mathbf v
=\mathbf u^\dagger A\mathbf v
=(A\mathbf u)^\dagger\mathbf v
=\lambda\mathbf u^\dagger\mathbf v.
$$

Distinct eigenvalues therefore have [orthogonal eigenvectors](../../../linear-algebra.md#orthogonal-vectors).

The normalized eigenvectors form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), so the matrix $U=(\mathbf u_1\ \cdots\ \mathbf u_n)$ satisfies $U^\dagger U=I$ and is unitary. With

$$
D=\operatorname{diag}(\lambda_1,\ldots,\lambda_n),
$$

the equations $A\mathbf u_j=\lambda_j\mathbf u_j$ say $AU=UD$, hence $A=UDU^\dagger$. This is the finite-dimensional [unitary diagonalization of a normal matrix](../../../linear-operator-theory.md#unitary-diagonalization-of-a-normal-matrix).

A unitary conjugate of an arbitrary [diagonal matrix](../../../linear-algebra.md#diagonal-matrix) need not be Hermitian: $U=(1)$ and $D=(i)$ give $UDU^\dagger=(i)$. It is Hermitian exactly when all diagonal entries of $D$ are real.

For the displayed matrix, one valid decomposition is

$$
\boxed{
U=\begin{pmatrix}
 i/\sqrt2&0&-i/\sqrt2\\
 0&1&0\\
 1/\sqrt2&0&1/\sqrt2
\end{pmatrix},
\qquad
D=\operatorname{diag}(5,2,-1)}.
$$

The columns are orthonormal eigenvectors, so direct multiplication gives $UDU^\dagger=A$.

## 7A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7a/solution">Solution</h3>

↑ **Parent:** [7A](#7a)

For the [heat kernel](../../../diffusion-equation.md#heat-kernel)

$$
K(x,t)=(4\pi t)^{-1/2}e^{-x^2/(4t)},
$$

direct [partial differentiation](../../../calculus.md#partial-derivative) gives

$$
K_t=\left(-\frac1{2t}+\frac{x^2}{4t^2}\right)K
=K_{xx}.
$$

Thus $K$ solves the [heat equation](../../../diffusion-equation.md#heat-equation). For bounded continuous $f$, [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) gives

$$
u_t=\int_{-\infty}^{\infty}K_t(x-y,t)f(y)\,dy
=\int_{-\infty}^{\infty}K_{xx}(x-y,t)f(y)\,dy=u_{xx}.
$$

With $Y=(x-y)/\sqrt{4t}$,

$$
u(x,t)=\frac1{\sqrt\pi}\int_{-\infty}^{\infty}
e^{-Y^2}f(x-2\sqrt t\,Y)\,dY.
$$

The [Gaussian integral](../../../calculus.md#gaussian-integral) makes the weight have total mass one, and the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives $u(x,t)\to f(x)$. This is the [Gaussian approximate identity](../../../diffusion-equation.md#gaussian-approximate-identity).

For the [viscous Burgers equation](../../../partial-differential-equation.md#viscous-burgers-equation) with unit viscosity, the [Cole-Hopf transformation](../../../partial-differential-equation.md#cole-hopf-transformation) $w=-2u_x/u$ reduces the equation to $u_t=u_{xx}$. To obtain initial value $g$, choose

$$
f(x)=\exp\left[-\frac12\int_0^x g(s)\,ds\right]
$$

(up to an irrelevant positive constant), and set $u=K_t*f$. Therefore

$$
\boxed{w(x,t)=-2\,\partial_x\log\!\left[
\int_{-\infty}^{\infty}K(x-y,t)f(y)\,dy
\right]}.
$$

Equivalently,

$$
w(x,t)=\frac1t
\frac{\int (x-y)K(x-y,t)f(y)\,dy}
{\int K(x-y,t)f(y)\,dy},
$$

and the approximate-identity limit gives $w(x,t)\to g(x)$.

## 8A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8a/solution">Solution</h3>

↑ **Parent:** [8A](#8a)

The first and third equations form a constant-coefficient [linear system of differential equations](../../../differential-equation.md#linear-system-of-differential-equations)

$$
\frac d{dt}\binom{x}{z}
=\begin{pmatrix}-1&3\\3&-1\end{pmatrix}\binom{x}{z}.
$$

The [eigenvectors](../../../linear-operator-theory.md#eigenvector) $(1,1)$ and $(1,-1)$ have [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $2$ and $-4$. Applying the initial data gives

$$
x(t)=\frac{e^{2t}-e^{-4t}}2,
\qquad
z(t)=\frac{e^{2t}+e^{-4t}}2.
$$

The remaining equation becomes

$$
y'-2y=-3e^{-4t}+\cos t-2\sin t.
$$

An [integrating factor](../../../differential-equation.md#integrating-factor), or the usual exponential and trigonometric particular solutions, gives

$$
\boxed{x(t)=\frac{e^{2t}-e^{-4t}}2,
\quad y(t)=\sin t+\frac{e^{-4t}-e^{2t}}2,
\quad z(t)=\frac{e^{2t}+e^{-4t}}2}.
$$

These values satisfy all three initial conditions.

## 9D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9d/a">a</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/a/solution">Solution</h4>

↑ **Parent:** [A](#9d/a)

[Rolle theorem](../../../calculus.md#rolle-theorem) states that if $h$ is continuous on the closed interval between two distinct points, differentiable between them, and has equal endpoint values, then $h'$ vanishes at an interior point.

Let $P_N(t)=\sum_{j=0}^Nf^{(j)}(0)t^j/j!$ and, for $x\ne0$, put

$$
M=\frac{f(x)-P_N(x)}{x^{N+1}},
\qquad h(t)=f(t)-P_N(t)-Mt^{N+1}.
$$

Then $h(x)=0$ and $h^{(j)}(0)=0$ for $0\leq j\leq N$. Applying Rolle's theorem successively $N+1$ times gives a point $\xi=\theta x$, $0<\theta<1$, where $h^{(N+1)}(\xi)=0$. Hence

$$
M=\frac{f^{(N+1)}(\theta x)}{(N+1)!},
$$

which is the stated [Taylor theorem with Lagrange remainder](../../../calculus.md#taylor-theorem-with-lagrange-remainder).

If $f'=0$, the $N=0$ case gives $f(x)=f(0)+xf'(\theta x)=f(0)$. Thus $f$ is constant; equivalently this is the immediate corollary of the [mean value theorem](../../../calculus.md#mean-value-theorem).

<h3 id="9d/b">b</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/b/i">i</h4>

↑ **Parent:** [B](#9d/b)

<h5 id="9d/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9d/b/i)

Differentiate

$$
F(x)=s(x)c(a-x)+c(x)s(a-x).
$$

Using $s'=c$ and $c'=-s$ gives

$$
F'(x)=c(x)c(a-x)+s(x)s(a-x)
-s(x)s(a-x)-c(x)c(a-x)=0.
$$

By the [zero derivative on a connected open set](../../../calculus.md#zero-derivative-on-a-connected-open-set), $F$ is independent of $x$.

<h4 id="9d/b/ii">ii</h4>

↑ **Parent:** [B](#9d/b)

<h5 id="9d/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9d/b/ii)

The constant from part (i) is found by setting $x=0$:

$$
F(0)=s(a).
$$

Taking $a=x+y$ therefore gives the [sine addition formula](../../../geometry-and-topology.md#sine-addition-formula)

$$
\boxed{s(x+y)=s(x)c(y)+c(x)s(y)}.
$$

<h4 id="9d/b/iii">iii</h4>

↑ **Parent:** [B](#9d/b)

<h5 id="9d/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9d/b/iii)

Differentiation gives

$$
\frac d{dx}(s(x)^2+c(x)^2)=2sc-2cs=0.
$$

The initial conditions set the constant to one, so

$$
\boxed{s(x)^2+c(x)^2=1},
$$

the [Pythagorean trigonometric identity](../../../geometry-and-topology.md#pythagorean-trigonometric-identity).

Since $|c|\leq1$, [Taylor theorem with Lagrange remainder](../../../calculus.md#taylor-theorem-with-lagrange-remainder) gives

$$
c(1)=1-\frac12c(\xi)>0
$$

for some $0<\xi<1$, while

$$
c(2)=1-\frac{2^2}{2}+\frac{2^4}{4!}c(\eta)
\leq-1+\frac23<0
$$

for some $0<\eta<2$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) supplies $k\in(1,2)$ with $c(k)=0$. The sine addition formula gives $s(2k)=2s(k)c(k)=0$. The analogous [cosine addition formula](../../../geometry-and-topology.md#cosine-addition-formula) gives $c(2k)=c(k)^2-s(k)^2=-1$, so

$$
s(x+2k)=-s(x),
\qquad
\boxed{s(x+4k)=s(x)}.
$$

**Thus $s$ is a [periodic function](../../../function.md#periodic-function).**

## 10F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

Choose a closed interval containing the [bounded sequence](../../../real-analysis.md#bounded-sequence). Bisect it and retain a half containing infinitely many terms; repeat. The resulting intervals are nested and their lengths tend to zero. By the [nested interval theorem](../../../real-analysis.md#nested-interval-theorem) they have one common point $x$, and choosing successively indexed terms from these intervals produces a subsequence converging to $x$. This proves the [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem).

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

Boundedness of $(z_n)$ makes both real sequences $(x_n)$ and $(y_n)$ bounded. The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) first gives a subsequence $(z_{n_j})$ for which $(x_{n_j})$ converges. Applying it again to $(y_{n_j})$ gives a subsubsequence for which the imaginary parts also converge. Since convergence of [complex numbers](../../../complex-analysis.md#complex-number) is equivalent to convergence of their [real parts](../../../complex-analysis.md#real-part) and [imaginary parts](../../../complex-analysis.md#imaginary-part), this subsubsequence converges in $\mathbb C$.

<h3 id="10f/c">c</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/c/solution">Solution</h4>

↑ **Parent:** [C](#10f/c)

Construct the nested index sequences inductively. Start with $N^{(0)}=(1,2,\ldots)$. Having chosen $N^{(i-1)}$, apply the [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) to the bounded sequence of $i$th coordinates along those indices, and let $N^{(i)}$ be an increasing subsequence along which that coordinate converges. Because each new sequence is nested inside all earlier ones, coordinates $1,\ldots,i$ all converge along $N^{(i)}$.

Now take the [diagonal subsequence argument](../../../real-analysis.md#diagonal-subsequence-argument)

$$
m_j=n_j^{(j)}.
$$

Nestedness implies

$$
m_{j+1}=n_{j+1}^{(j+1)}\geq n_{j+1}^{(j)}>n_j^{(j)}=m_j,
$$

so $(m_j)$ is strictly increasing. For every fixed $i$, the tail $(m_j)_{j\geq i}$ is a subsequence of $N^{(i)}$; hence $(x_{m_j}^{(i)})$ converges. This single diagonal subsequence works for every coordinate.

## 11F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

For events $A_1,\ldots,A_n$, the probabilistic [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) is

$$
\boxed{\mathbb P\left(\bigcup_{i=1}^nA_i\right)
=\sum_{\varnothing\ne J\subseteq\{1,\ldots,n\}}
(-1)^{|J|+1}\mathbb P\left(\bigcap_{j\in J}A_j\right)}.
$$

To prove it, fix an outcome lying in exactly $r$ events. Its total coefficient on the right is

$$
\sum_{k=1}^r(-1)^{k+1}\binom rk=1
$$

by the [binomial theorem](../../../combinatorics.md#binomial-theorem); outcomes in no event contribute zero. Taking expectations of this pointwise indicator identity proves the formula. Truncating after the pair terms gives the [Bonferroni inequalities](../../../combinatorics.md#bonferroni-inequalities)

$$
\mathbb P\left(\bigcup_iA_i\right)
\geq\sum_i\mathbb P(A_i)-\sum_{i<j}\mathbb P(A_i\cap A_j).
$$

For the final bound, let $X=\sum_i\mathbf1_{A_i}$ and $S=\mathbb EX=\sum_i\mathbb P(A_i)$. The intersection assumption gives

$$
\mathbb E[X^2]
=S+2\sum_{i<j}\mathbb P(A_i\cap A_j)
\leq S+n-1.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) applied to $X\mathbf1_{X>0}$ yields $S^2\leq\mathbb E[X^2]\mathbb P(X>0)\leq S+n-1$. Therefore

$$
S\leq\frac{1+\sqrt{4n-3}}2\leq2\sqrt n,
$$

so the required universal constant may be taken as $\boxed{c=2}$. This is a [second moment method](../../../probability-inequality.md#second-moment-method) estimate.

## 12F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/solution">Solution</h4>

↑ **Parent:** [A](#12f/a)

The [standard normal density](../../../probability-theory.md#standard-normal-density) is

$$
\phi(z)=\frac1{\sqrt{2\pi}}e^{-z^2/2},
\qquad z\in\mathbb R.
$$

It is nonnegative, and the [Gaussian integral](../../../calculus.md#gaussian-integral) gives $\int_{-\infty}^{\infty}\phi(z)\,dz=1$, so it is a [probability density function](../../../continuous-probability-distribution.md#probability-density-function). Completing the square gives the [moment-generating function of a standard normal variable](../../../probability-theory.md#moment-generating-function-of-a-standard-normal-variable)

$$
M_Z(\theta)=\int e^{\theta z}\phi(z)\,dz
=e^{\theta^2/2}.
$$

Thus $\mathbb EZ=M_Z'(0)=0$ and

$$
\boxed{\operatorname{var}(Z)=M_Z''(0)-M_Z'(0)^2=1.}
$$

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/solution">Solution</h4>

↑ **Parent:** [B](#12f/b)

The [linear combination of independent normal random variables](../../../probability-theory.md#linear-combination-of-independent-normal-random-variables) is normal. Hence

$$
S_n\sim N(0,n),
\qquad
\boxed{U_n=\frac{S_n}{\sqrt n}\sim N(0,1)}.
$$

This also follows by multiplying the [moment-generating functions](../../../probability-theory.md#moment-generating-function) of the [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables).

<h3 id="12f/c">c</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/c/solution">Solution</h4>

↑ **Parent:** [C](#12f/c)

Since $Y_1=X_1^2$ and a standard normal variable has second and fourth moments $1$ and $3$,

$$
\boxed{\mu=\mathbb EY_1=1,
\qquad \sigma^2=\operatorname{var}(Y_1)=3-1=2}.
$$

Thus $T_n$ has the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $n$ degrees of freedom and

$$
V_n=\frac{T_n-n}{\sqrt{2n}}.
$$

[Convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) $W_n\Rightarrow W$ means that the [cumulative distribution functions](../../../probability-theory.md#cumulative-distribution-function) satisfy $F_{W_n}(x)\to F_W(x)$ at every continuity point of $F_W$. The [Lévy continuity theorem](../../../probability-theory.md#levy-continuity-theorem) states that this is equivalent to pointwise convergence of [characteristic functions](../../../probability-theory.md#characteristic-function) to the characteristic function of $W$, provided the limiting function is continuous at zero.

For fixed $t$, independence and a Gaussian integral give

$$
\varphi_{V_n}(t)
=\left[e^{-it/\sqrt{2n}}
\left(1-i t\sqrt{\frac2n}\right)^{-1/2}\right]^n.
$$

Using $\log(1-z)=-z-z^2/2+O(z^3)$,

$$
\log\varphi_{V_n}(t)
=n\left[-\frac{it}{\sqrt{2n}}
-\frac12\log\left(1-it\sqrt{\frac2n}\right)\right]
=-\frac{t^2}{2}+O(n^{-1/2}).
$$

Therefore $\varphi_{V_n}(t)\to e^{-t^2/2}$, the characteristic function of the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). Lévy's theorem now gives

$$
\boxed{V_n\Rightarrow Z}.
$$

This derives the limit directly, without assuming the central limit theorem.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2020](../../2020.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
