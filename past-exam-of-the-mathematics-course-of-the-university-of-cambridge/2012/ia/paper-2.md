# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2012/PaperIA_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2012/PaperIA_2.pdf)

**Table of contents**

- [1A](#1a)
  - [Solution](#1a/solution)
- [2A](#2a)
  - [Solution](#2a/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5A](#5a)
  - [Solution](#5a/solution)
- [6A](#6a)
  - [Solution](#6a/solution)
- [7A](#7a)
  - [Solution](#7a/solution)
- [8A](#8a)
  - [i](#8a/i)
    - [Solution](#8a/i/solution)
  - [ii](#8a/ii)
    - [Solution](#8a/ii/solution)
  - [iii](#8a/iii)
    - [Solution](#8a/iii/solution)
  - [iv](#8a/iv)
    - [Solution](#8a/iv/solution)
- [9F](#9f)
  - [i](#9f/i)
    - [Solution](#9f/i/solution)
  - [ii](#9f/ii)
    - [Solution](#9f/ii/solution)
  - [iii](#9f/iii)
    - [Solution](#9f/iii/solution)
- [10F](#10f)
  - [i](#10f/i)
    - [Solution](#10f/i/solution)
  - [ii](#10f/ii)
    - [Solution](#10f/ii/solution)
- [11F](#11f)
  - [i](#11f/i)
    - [Solution](#11f/i/solution)
  - [ii](#11f/ii)
    - [Solution](#11f/ii/solution)
  - [iii](#11f/iii)
    - [Solution](#11f/iii/solution)
- [12F](#12f)
  - [Solution](#12f/solution)

## 1A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1a/solution">Solution</h3>

↑ **Parent:** [1A](#1a)

The [repeated-root constant-coefficient differential equation](../../../differential-equation.md#repeated-root-constant-coefficient-differential-equation) has characteristic polynomial $(r+2)^2$. Its two fundamental solutions are

$$
\boxed{y_1=e^{-2x},\qquad y_2=xe^{-2x}}.
$$

They are [linearly independent](../../../vector-space.md#linear-independence): their [Wronskian](../../../differential-equation.md#wronskian) is $e^{-4x}$, which never vanishes. For the forced equation, exploit the repeated factor by writing $y=e^{-2x}u$. Direct differentiation gives $(D+2)^2y=e^{-2x}u''$, so the forcing reduces to $u''=1$. The initial data imply $u(0)=0$ and $u'(0)=0$, hence $u=x^2/2$. Therefore

$$
\boxed{y(x)=\frac{x^2}{2}e^{-2x},\qquad x\geq0}.
$$

The extra factor $x^2$ reflects resonance of the forcing with the repeated characteristic root; the exponential substitution obtains it without guessing a particular solution.

## 2A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2a/solution">Solution</h3>

↑ **Parent:** [2A](#2a)

A constant orbit is a [fixed point](../../../function.md#fixed-point) of $F(u)=u(1+u)/2$. Solving $F(u)=u$ gives $u(u-1)=0$, hence

$$
\boxed{u_n\equiv0\quad\text{and}\quad u_n\equiv1}.
$$

For [fixed point stability for an iteration](../../../dynamical-systems.md#fixed-point-stability-for-an-iteration), perturb a fixed point $u_*$ by $v_n$. Its local evolution is $v_{n+1}=F'(u_*)v_n+O(v_n^2)$, where $F'(u)=u+1/2$. At zero, $F'(0)=1/2$, so perturbations contract: **zero is locally asymptotically stable**. For example, if $|u|\leq r<1$, then $|F(u)|\leq(1+r)|u|/2$; this gives an invariant neighborhood and geometric convergence to zero.

At one, $F'(1)=3/2$, so perturbations expand: **one is unstable**. More explicitly, putting $u_n=1+v_n$ gives $v_{n+1}=3v_n/2+v_n^2/2$, whose magnitude increases while a nonzero perturbation remains sufficiently small. The derivative test concerns local stability; it does not assert attraction from every real initial value.

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

For events with $P(B)>0$, the [conditional probability](../../../probability-theory.md#conditional-probability) is $P(A\mid B)=P(A\cap B)/P(B)$. Applying the definition in both orders gives [Bayes' theorem](../../../probability-theory.md#bayes-theorem):

$$
P(B\mid A)=\frac{P(A\cap B)}{P(A)}=P(A\mid B)\frac{P(B)}{P(A)}.
$$

Conditionally on $N=n$, independent fair tosses give a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) for the head count, so $P(H=1\mid N=n)=n2^{-n}$. The joint [probability mass function](../../../probability-theory.md#probability-mass-function) is consequently

$$
P(N=n,H=1)=n4^{-n}.
$$

Use the [law of total probability](../../../probability-theory.md#law-of-total-probability) and the differentiated [geometric series](../../../real-analysis.md#geometric-series), $\sum_{n\geq1}nr^n=r/(1-r)^2$, to obtain $P(H=1)=4/9$. The [posterior coin count after exactly one head](../../../probability-theory.md#posterior-coin-count-after-exactly-one-head) is therefore

$$
\boxed{P(N=n\mid H=1)=\frac{9n}{4^{n+1}},\qquad n\geq1}.
$$

These [probabilities](../../../probability-theory.md#probability) sum to one by the same series identity. The conditioning weights possible coin counts by their likelihood of producing exactly one head.

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

For a nonnegative integer-valued [random variable](../../../random-variable.md), the [probability generating function](../../../probability-theory.md#probability-generating-function) is

$$
G_X(s)=\mathbb E[s^X]=\sum_{j=0}^\infty P(X=j)s^j,
$$

with $0\leq s\leq1$ always allowed. Its derivative at $1$ from below gives the [expectation](../../../probability-theory.md#expected-value) when finite.

The waiting time $N$ has the positive-integer [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) $P(N=j)=pq^{j-1}$. For the [capped geometric waiting time](../../../discrete-probability-distribution.md#capped-geometric-waiting-time), $X=j<k$ exactly when $N=j$, while $X=k$ occurs whenever $N\geq k$. Thus the terminal mass is $q^{k-1}$, giving

$$
\boxed{G_X(s)=p\sum_{j=1}^{k-1}q^{j-1}s^j+q^{k-1}s^k
=\frac{ps+q^ks^k(1-s)}{1-qs}}.
$$

The finite sum is a polynomial; any apparent singularity of the rational expression is removable. This includes $k=1$, where $G_X(s)=s$.

Differentiating the rational form at $s=1$ yields

$$
G_X'(1)=\frac{(p-q^k)p+pq}{p^2}=\boxed{\frac{1-q^k}{p}}.
$$

As a second interpretation, the [expectation](../../../probability-theory.md#expected-value) is the sum of the tail [probabilities](../../../probability-theory.md#probability) $P(X\geq j)=q^{j-1}$ for $1\leq j\leq k$. Their finite geometric sum gives the same answer.

## 5A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5a/solution">Solution</h3>

↑ **Parent:** [5A](#5a)

Use a [power-series solution of a differential equation](../../../differential-equation.md#power-series-solution-of-a-differential-equation), $y=\sum_{n\geq0}c_nx^n$. Comparing coefficients gives

$$
(n-1)(n-2)c_n=c_{n-2},\qquad c_{-1}=c_{-2}=0.
$$

In particular $c_0=0$, while $c_1$ and $c_2$ are free. The two prescribed derivative pairs select $(c_1,c_2)=(a,0)$ and $(0,b)$. The next coefficients are $c_3=c_1/2$, $c_4=c_2/6$, $c_5=c_1/24$, $c_6=c_2/120$. Hence

$$
\boxed{y_1(x)=a\left(x+\frac{x^3}{2}+\frac{x^5}{24}+O(x^7)\right)},\qquad
\boxed{y_2(x)=b\left(x^2+\frac{x^4}{6}+\frac{x^6}{120}+O(x^8)\right)}.
$$

These are the first three nonzero terms when the respective parameter is nonzero; if $a=0$ or $b=0$, the corresponding solution vanishes identically.

For closed forms, set $y=xu$. Cancellation of the first-derivative terms reduces the equation, for $x\ne0$, to $u''-u=0$. The analytic solutions extend across zero, and their [hyperbolic cosine](../../../calculus.md#hyperbolic-cosine) and [hyperbolic sine](../../../calculus.md#hyperbolic-sine) expansions identify

$$
\boxed{y_1=ax\cosh x,\qquad y_2=bx\sinh x}.
$$

This is the [hyperbolic reduction of a regular-singular differential equation](../../../complex-analysis.md#hyperbolic-reduction-of-a-regular-singular-differential-equation): although the original leading coefficient vanishes at zero, both selected [power-series solutions of a differential equation](../../../differential-equation.md#power-series-solution-of-a-differential-equation) are entire.

## 6A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6a/solution">Solution</h3>

↑ **Parent:** [6A](#6a)

Completing squares reveals the geometry of the [sheared quartic double-well gradient flow](../../../analysis.md#sheared-quartic-double-well-gradient-flow):

$$
V=(x^2-1)^2+(x+y)^2-1.
$$

The [critical points](../../../analysis.md#critical-point) satisfy $2(x+y)=0$ and $4x^3-2x+2y=0$, so they are $(0,0)$, $(1,-1)$ and $(-1,1)$. The [Hessian matrix](../../../calculus.md#hessian-matrix) is

$$
\operatorname{Hess}V=\begin{pmatrix}12x^2-2&2\\2&2\end{pmatrix}.
$$

At the origin its determinant is $-8$, so $(0,0)$ is a [saddle point](../../../analysis.md#saddle-point), with $V=0$. At either other [critical point](../../../analysis.md#critical-point), the determinant is $16$ and the upper-left entry is $10$, so it is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix). They are strict [local minima](../../../analysis.md#local-minimum); the completed squares show that both are global minima, with $V=-1$.

A contour at level $c$ obeys

$$
(x+y)^2=c+1-(x^2-1)^2,\qquad
 y=-x\pm\sqrt{c+1-(x^2-1)^2}.
$$

There are no contours for $c<-1$, two isolated minimum points for $c=-1$, and two separate closed ovals for $-1<c<0$. At $c=0$ the two lobes meet at the [saddle point](../../../analysis.md#saddle-point); near the origin their tangents are $y=(-1\pm\sqrt2)x$. For $c>0$ one closed contour surrounds both minima.

<a id="6a/image-sheared-quartic-potential-contours-and-the-trajectory-to-the-positive-x-minimum"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2-double-well-contours.png)

**[Figure 1](#6a/image-sheared-quartic-potential-contours-and-the-trajectory-to-the-positive-x-minimum). Sheared quartic potential contours and the trajectory to the positive-x minimum**.

Along the [gradient flow](../../../analysis.md#gradient-flow), the [gradient-flow dissipation identity](../../../analysis.md#gradient-flow-dissipation-identity) is

$$
\boxed{\frac{dV}{dt}=V_x\dot x+V_y\dot y=-V_x^2-V_y^2\leq0}.
$$

At the stated initial point, $V(1,-1/2)=-3/4$. Its trajectory stays in the [invariant sublevel set](../../../dynamical-systems.md#invariant-sublevel-set) $V\leq-3/4$. This set is compact because $V$ is a [coercive function](../../../real-analysis.md#coercive-function). It also excludes every point with $x=0$, where $V=y^2\geq0$; continuity therefore keeps the trajectory in its positive-$x$ component.

To justify its limit rather than merely infer it from the sketch, integrate the dissipation identity: $\int_0^\infty\|\nabla V\|^2dt$ is finite. On this compact set the gradient and its time derivative are bounded, so $\|\nabla V\|^2$ is uniformly continuous. A nonnegative uniformly continuous function with finite integral tends to zero: otherwise separated intervals of a fixed positive height and width would force an infinite integral. Every accumulation point is consequently a [critical point](../../../analysis.md#critical-point). In the positive-$x$ component below this energy level the only one is $(1,-1)$. Compactness then implies convergence, and

$$
\boxed{(x(t),y(t))\longrightarrow(1,-1)\quad(t\to\infty)}.
$$

This is a [compact gradient-flow trapping criterion](../../../dynamical-systems.md#compact-gradient-flow-trapping-criterion); the drawn trajectory illustrates, rather than replaces, the convergence proof.

## 7A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7a/solution">Solution</h3>

↑ **Parent:** [7A](#7a)

Write the [linear system of differential equations](../../../differential-equation.md#linear-system-of-differential-equations) as

$$
\mathbf z'=\frac1tA\mathbf z+\mathbf b,\qquad
A=\begin{pmatrix}4&-2\\-1&5\end{pmatrix},\quad\mathbf b=\binom{-9}{3}.
$$

A homogeneous power $t^\lambda\mathbf v$ solves this [Cauchy-Euler differential system](../../../differential-equation.md#cauchy-euler-differential-system) precisely when $A\mathbf v=\lambda\mathbf v$. The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $3$ and $6$, with [eigenvectors](../../../linear-operator-theory.md#eigenvector) $(2,1)^T$ and $(1,-1)^T$. The homogeneous solution is therefore $C t^3(2,1)^T+D t^6(1,-1)^T$.

For a particular solution, put $\mathbf z_p=t\mathbf c$. Then $(I-A)\mathbf c=\mathbf b$, which gives $\mathbf c=(3,0)^T$. At $t=1$, the two initial conditions become $2C+D+3=0$ and $C-D=0$, so $C=D=-1$. Thus

$$
\boxed{x(t)=3t-2t^3-t^6,\qquad y(t)=t^6-t^3,\qquad t\geq1}.
$$

The two powers correspond to the two [eigenvalues](../../../linear-operator-theory.md#eigenvalue); the lower-degree particular term accounts for the constant forcing. Substitution gives both original right sides and the zero initial data.

## 8A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8a/i">i</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/i/solution">Solution</h4>

↑ **Parent:** [I](#8a/i)

For the [damped harmonic oscillator](../../../analysis.md#damped-harmonic-oscillator), the characteristic roots are $-k\pm i\omega$. For $\omega\ne0$, the real general solution is

$$
\boxed{y_1(t)=e^{-kt}\left(A\cos\omega t+B\sin\omega t\right)}.
$$

If the frequency parameter is zero, the characteristic root is repeated and the complete limiting basis is $e^{-kt},te^{-kt}$, so $y_1=e^{-kt}(A+Bt)$. No sign restriction on $k$ is needed for these formulas, although $k>0$ corresponds to decay.

<h3 id="8a/ii">ii</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8a/ii)

Before the impulse the zero initial data force $y_2=0$. An impulse modeled by the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) requires continuity of $y_2$: a jump in $y_2$ would introduce an unwanted derivative of a delta in $y_2''$. Integrating the equation across $t=a$ then gives the velocity jump $y_2'(a+)-y_2'(a-)=1$.

The [causal Green function of a damped oscillator](../../../analysis.md#causal-green-function-of-a-damped-oscillator) is

$$
g(s)=e^{-ks}\frac{\sin\omega s}{\omega},\qquad g(0)=0,\quad g'(0)=1.
$$

The jump conditions give the causal impulse response

$$
\boxed{y_2(t,a)=H(t-a)e^{-k(t-a)}\frac{\sin[\omega(t-a)]}{\omega}}.
$$

Here $H$ is the [Heaviside step function](../../../analysis.md#heaviside-step-function). For $\omega=0$, interpret the quotient continuously as $t-a$, giving $H(t-a)(t-a)e^{-k(t-a)}$. Both initial values are zero because $a>0$.

<h3 id="8a/iii">iii</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8a/iii)

The [step response of a damped oscillator](../../../analysis.md#step-response-of-a-damped-oscillator) is the time integral of its [causal Green function of a damped oscillator](../../../analysis.md#causal-green-function-of-a-damped-oscillator). Put $s=t-b$ and define $K(s)=\int_0^s e^{-ku}\sin(\omega u)/\omega\,du$ for $s\geq0$. Then $K(0)=K'(0)=0$ and its oscillator equation has constant right side $1$. Integrating explicitly gives

$$
\boxed{y_3(t,b)=\frac{H(t-b)}{k^2+\omega^2}\left\{1-e^{-k(t-b)}\left[\cos\omega(t-b)+\frac k\omega\sin\omega(t-b)\right]\right\}}.
$$

This formula applies when $\omega\ne0$. It is a [convolution](../../../fourier-analysis.md#convolution) of the causal impulse response with the shifted [Heaviside step function](../../../analysis.md#heaviside-step-function), so the response is zero before the forcing starts and has the stated zero initial data.

The integral definition also handles the degenerate parameters without division ambiguities. For $\omega=0,k\ne0$,

$$
y_3=H(s)\frac{1-e^{-ks}(1+ks)}{k^2};
$$

for $\omega=k=0$, $y_3=H(s)s^2/2$. These are the continuous zero-frequency limits of the step response.

<h3 id="8a/iv">iv</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#8a/iv)

Use the [shift derivative of a step response](../../../analysis.md#shift-derivative-of-a-step-response), writing $y_3(t,b)=H(s)K(s)$ with $s=t-b$. Differentiate with respect to the forcing location:

$$
-\frac{\partial y_3}{\partial b}=\delta(s)K(s)+H(s)K'(s).
$$

The possible delta term vanishes because $K(0)=0$, while $K'(s)=g(s)$. Therefore, as a distribution and also as the ordinary piecewise response,

$$
\boxed{-\frac{\partial y_3(t,b)}{\partial b}=H(t-b)g(t-b)=y_2(t,b)}.
$$

Moving the start of a unit step differentiates its forcing into a negative impulse. The zero initial conditions and [linearity](../../../vector-space.md#linearity) ensure that the corresponding responses obey the same identity, including the zero-frequency cases.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/i">i</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/i/solution">Solution</h4>

↑ **Parent:** [I](#9f/i)

The [moment-generating function](../../../probability-theory.md#moment-generating-function) is $M_X(t)=\mathbb E[e^{tX}]$ at real $t$ for which that expectation is finite; $M_X(0)=1$. For independent [random variables](../../../random-variable.md), the joint law factorizes, so

$$
M_{aX+bY}(t)=\mathbb E[e^{atX}e^{btY}]=\mathbb E[e^{atX}]\mathbb E[e^{btY}]
=\boxed{M_X(at)M_Y(bt)}.
$$

This is the transform form of [independence](../../../random-variable.md#independent-random-variables). Its ordinary finite-valued interpretation applies where both factors are finite, with the transform of a zero multiple equal to $1$.

<h3 id="9f/ii">ii</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9f/ii)

Finiteness of the [moment-generating function](../../../probability-theory.md#moment-generating-function) on an open neighborhood of zero gives its differentiability there. Using the permitted interchange of differentiation and [expectation](../../../probability-theory.md#expected-value),

$$
M_X'(t)=\mathbb E[Xe^{tX}],\qquad M_X''(t)=\mathbb E[X^2e^{tX}].
$$

Hence $M_X(0)=1$, $M_X'(0)=\mu$ and $M_X''(0)=s^2$. The second-order [Taylor expansion](../../../calculus.md#taylor-expansion) with its Peano remainder gives

$$
\boxed{M_X(t)=1+\mu t+\frac12s^2t^2+o(t^2)}.
$$

Here $s^2$ is the raw second moment, not the [variance](../../../variance.md): $\operatorname{Var}(X)=s^2-\mu^2$. This distinction matters before specializing to a centered variable.

<h3 id="9f/iii">iii</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#9f/iii)

Let $S=X+Y$ and $D=X-Y$. Since they are independent, applying the product rule for [moment-generating functions](../../../probability-theory.md#moment-generating-function) to $S+D=2X$ gives

$$
M(2t)=M_S(t)M_D(t)=M(t)^2M(t)M(-t)=\boxed{M(t)^3M(-t)}.
$$

All factors are finite and strictly positive for every real $t$ by the stated hypothesis. Applying the same identity to $-t$ and dividing yields $\psi(2t)=\psi(t)^2$, or

$$
\boxed{\psi(t)=\psi(t/2)^2},\qquad \psi(t)=\frac{M(t)}{M(-t)}.
$$

The centered unit-variance [Taylor expansion](../../../calculus.md#taylor-expansion) from part (ii) gives $M(h)=1+h^2/2+o(h^2)$ and the same expansion for $M(-h)$. Consequently $\psi(h)=1+o(h^2)$.

For the first step of [dyadic rigidity of a moment-generating function](../../../probability-theory.md#dyadic-rigidity-of-a-moment-generating-function), take logarithms, which are allowed because $\psi>0$. For each fixed $t$ and every integer $m$,

$$
\log\psi(t)=2^m\log\psi(t/2^m).
$$

Since $\log\psi(h)=o(h^2)$, the right side tends to zero: it is $2^m o(t^2/4^m)$. Thus $\psi(t)=1$ for every $t$, and the [moment-generating function](../../../probability-theory.md#moment-generating-function) is even.

The original identity now becomes $M(2t)=M(t)^4$. Iterating this time with the correct fourth-power scaling gives

$$
\log M(t)=4^m\log M(t/2^m).
$$

Near zero, $\log M(h)=h^2/2+o(h^2)$, so the right side tends to $t^2/2$. Therefore

$$
\boxed{M(t)=e^{t^2/2}\quad\text{for all real }t}.
$$

This is the [moment-generating function of a standard normal variable](../../../probability-theory.md#moment-generating-function-of-a-standard-normal-variable). By the [uniqueness theorem for moment-generating functions](../../../probability-theory.md#uniqueness-theorem-for-moment-generating-functions), each of $X$ and $Y$ has the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). The proof establishes the [Gaussian characterization by independent sum and difference](../../../probability-theory.md#gaussian-characterization-by-independent-sum-and-difference) directly from the two functional identities and the first two moments.

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/i">i</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/i/solution">Solution</h4>

↑ **Parent:** [I](#10f/i)

The [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) is $F(x)=P(X\leq x)$. For the differentiable distribution in the question, its [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is $f(x)=F'(x)$, so [probabilities](../../../probability-theory.md#probability) over intervals are obtained by integrating $f$. The survival [probability](../../../probability-theory.md#probability) is $P(X>x)=1-F(x)$. Differentiating immediately gives

$$
\boxed{f(x)=-\frac d{dx}P(X>x)}.
$$

The strict inequality is consistent with the definition using $X\leq x$. This relation connects the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) with the decline of the survival [probability](../../../probability-theory.md#probability).

<h3 id="10f/ii">ii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10f/ii)

The independent [uniform distributions](../../../continuous-probability-distribution.md#continuous-uniform-distribution) give a constant [joint probability density](../../../continuous-probability-distribution.md#joint-probability-density) $1$ on the unit square. For $0<x<1$, integrate over $x<u<v^2$:

$$
P(V^2>U>x)=\int_x^1\int_{\sqrt u}^1dv\,du=\int_x^1(1-\sqrt u)du
=\boxed{\frac13-x+\frac23x^{3/2}}.
$$

For the [random quadratic with uniform coefficients](../../../continuous-probability-distribution.md#random-quadratic-with-uniform-coefficients), real roots require its [discriminant](../../../polynomial.md#discriminant) to be nonnegative, equivalently $U\leq V^2$. The boundary has [probability](../../../probability-theory.md#probability) zero, and the area under this parabola is

$$
\boxed{P(\text{real roots})=\int_0^1v^2dv=\frac13}.
$$

On that event the roots are $-V\pm\sqrt{V^2-U}$, both nonpositive. Bounding both absolute values by one therefore amounts to bounding the more negative root:

$$
V+\sqrt{V^2-U}\leq1.
$$

Since $0\leq V\leq1$, squaring the inequality is legitimate and gives $U\geq2V-1$. The admissible unit-square region is $\max(0,2v-1)\leq u\leq v^2$. Its [probability](../../../probability-theory.md#probability) is

$$
\int_0^{1/2}v^2dv+\int_{1/2}^1(v^2-2v+1)dv=\frac1{24}+\frac1{24}=\frac1{12}.
$$

Dividing by the real-root [probability](../../../probability-theory.md#probability) gives the requested [conditional probability](../../../probability-theory.md#conditional-probability):

$$
\boxed{P(|R_1|\leq1,|R_2|\leq1\mid\text{real roots})=\frac14}.
$$

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/i">i</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/i/solution">Solution</h4>

↑ **Parent:** [I](#11f/i)

For a [Galton-Watson process](../../../probability-and-statistics.md#galton-watson-process), condition on the number $K$ of children of the initial individual. The descendants of these children over the next $n$ generations are independent copies of $X_n$. The [probability generating function](../../../probability-theory.md#probability-generating-function) of their total, conditional on $K=k$, is $G_n(s)^k$. Averaging over the family-size law gives

$$
G_{n+1}(s)=\mathbb E[G_n(s)^K]=\boxed{G(G_n(s))},\qquad G_0(s)=s.
$$

This is the [branching-process generating-function iteration](../../../probability-and-statistics.md#branching-process-generating-function-iteration). Conditioning instead on the last generation gives $G_n(G(s))$; both orders agree because $G_n$ is the $n$th iterate of the same function $G$. The argument holds on the usual [PGF](../../../probability-theory.md#probability-generating-function) domain $|s|\leq1$, with larger domains available when the corresponding expectations converge.

<h3 id="11f/ii">ii</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11f/ii)

The geometric family law on the nonnegative integers has [probability generating function](../../../probability-theory.md#probability-generating-function)

$$
\boxed{G(s)=\sum_{k\geq0}2^{-k-1}s^k=\frac1{2-s}},\qquad |s|<2.
$$

Its [expected value](../../../probability-theory.md#expected-value) is $G'(1)=1$, so this is a [geometric-offspring critical branching process](../../../probability-and-statistics.md#geometric-offspring-critical-branching-process). Starting from $G_0(s)=s$, verify the rational iterate by induction. If $G_n(s)=[n-(n-1)s]/[n+1-ns]$, then

$$
G(G_n(s))=\frac1{2-G_n(s)}=\frac{n+1-ns}{n+2-(n+1)s},
$$

which has the same form with $n$ replaced by $n+1$. Thus, for $n\geq1$,

$$
\boxed{G_n(s)=\frac{n-(n-1)s}{n+1-ns},\qquad |s|<1+\frac1n}.
$$

The stated disk is the actual power-series convergence domain, not merely a place where the rational continuation can be evaluated. Its simple pole is at $s=1+1/n$.

The extinction [probability](../../../probability-theory.md#probability) at generation $n$ is the constant coefficient:

$$
\boxed{P(X_n=0)=G_n(0)=\frac n{n+1}}.
$$

For later use, expanding the remaining [geometric series](../../../real-analysis.md#geometric-series) gives

$$
P(X_n=j)=\frac1{(n+1)^2}\left(\frac n{n+1}\right)^{j-1},\qquad j\geq1.
$$

In particular $P(X_n>0)=1/(n+1)$. At $n=0$ the initial population is one deterministically; its [PGF](../../../probability-theory.md#probability-generating-function) is $s$, and the displayed radius involving $1/n$ is used only for $n\geq1$.

<h3 id="11f/iii">iii</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11f/iii)

For $n\geq1$, substitute $s=e^{t/n}$ in the [probability generating function](../../../probability-theory.md#probability-generating-function). The [moment-generating function](../../../probability-theory.md#moment-generating-function) of $X_n/n$ is

$$
\boxed{M_{X_n/n}(t)=\frac{n-(n-1)e^{t/n}}{n+1-ne^{t/n}}},\qquad
\boxed{t<n\log(1+1/n)}.
$$

The domain follows from convergence of the generating series; at or above that positive threshold the expectation diverges, even though a rational continuation can be written.

Conditioning on survival, the [probability mass function](../../../probability-theory.md#probability-mass-function) from part (ii) becomes a positive-integer [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution):

$$
P(X_n=j\mid X_n>0)=\frac1{n+1}\left(\frac n{n+1}\right)^{j-1},\qquad j\geq1.
$$

Its conditional [moment-generating function](../../../probability-theory.md#moment-generating-function) is $e^{t/n}/[n+1-ne^{t/n}]$, tending to $1/(1-t)$ for fixed $t<1$. We can prove the required limit directly, without invoking a continuity theorem. Set $r_n=n/(n+1)$. For every $x\geq0$, the strict upper tail is exactly

$$
P(X_n/n>x\mid X_n>0)=r_n^{\lfloor nx\rfloor}.
$$

Since $\log r_n=-1/n+O(n^{-2})$ and $\lfloor nx\rfloor/n\to x$,

$$
\boxed{P(X_n/n>x\mid X_n>0)\longrightarrow e^{-x}}.
$$

At $x=0$ both tails equal one. This is the [exponential limit of surviving geometric branching](../../../probability-and-statistics.md#exponential-limit-of-surviving-geometric-branching). Conditioning is essential: the unconditional variable has [probability](../../../probability-theory.md#probability) $n/(n+1)$ of being zero, whereas the rare surviving population has size of order $n$.

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/solution">Solution</h3>

↑ **Parent:** [12F](#12f)

For independent [random variables](../../../random-variable.md), $\{\min(X,Y)>u\}=\{X>u,Y>u\}$ and $\{\max(X,Y)\leq v\}=\{X\leq v,Y\leq v\}$. Factor their [probabilities](../../../probability-theory.md#probability) to obtain the [distribution functions of independent minima and maxima](../../../probability-theory.md#distribution-functions-of-independent-minima-and-maxima):

$$
\boxed{F_U(u)=1-[1-F_X(u)][1-F_Y(u)],\qquad F_V(v)=F_X(v)F_Y(v)}.
$$

These formulas also allow atoms; no [probability density function](../../../continuous-probability-distribution.md#probability-density-function) assumption is needed.

For independent unit-rate [exponential distributions](../../../continuous-probability-distribution.md#exponential-distribution), $P(U>u)=e^{-2u}$ for $u\geq0$, so $U\sim\operatorname{Exp}(2)$. To establish the [independent minimum and gap of two exponential variables](../../../probability-theory.md#independent-minimum-and-gap-of-two-exponential-variables), set $D=V-U$. On either ordering branch, the change of variables is $(X,Y)=(u,u+d)$ or $(u+d,u)$ with unit absolute [Jacobian determinant](../../../calculus.md#jacobian-determinant). Both contribute $e^{-2u-d}$; ties have [probability](../../../probability-theory.md#probability) zero. Thus the [joint probability density](../../../continuous-probability-distribution.md#joint-probability-density) is

$$
f_{U,D}(u,d)=2e^{-2u-d}=(2e^{-2u})(e^{-d}),\qquad u,d>0.
$$

It factors into normalized exponential [probability density functions](../../../continuous-probability-distribution.md#probability-density-function), proving $U\sim\operatorname{Exp}(2)$, $D\sim\operatorname{Exp}(1)$ and their [independence](../../../random-variable.md#independent-random-variables).

The maximum is $V=U+D$. A half-scaled unit-rate exponential has rate two, so the independent pair $(D,U)$ has the same joint law as $(X,Y/2)$. Consequently

$$
\boxed{V\overset d=X+\frac12Y}.
$$

Using the [expected values](../../../probability-theory.md#expected-value), [variances](../../../variance.md) and [independence](../../../random-variable.md#independent-random-variables) of the summands,

$$
\boxed{\mathbb E V=\frac32,\qquad\operatorname{Var}(V)=\frac54}.
$$

The spacing factorization explains why an order statistic can be represented as a sum of independent waiting times.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
