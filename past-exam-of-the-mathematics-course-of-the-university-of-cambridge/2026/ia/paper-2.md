# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2026/Paperia_2_2026.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2026/Paperia_2_2026.pdf)

**Table of contents**

- [1C](#1c)
  - [Solution](#1c/solution)
- [2C](#2c)
  - [a](#2c/a)
    - [Solution](#2c/a/solution)
  - [b](#2c/b)
    - [Solution](#2c/b/solution)
- [3F](#3f)
  - [i](#3f/i)
    - [Solution](#3f/i/solution)
  - [ii](#3f/ii)
    - [Solution](#3f/ii/solution)
- [4F](#4f)
  - [i](#4f/i)
    - [Solution](#4f/i/solution)
  - [ii](#4f/ii)
    - [Solution](#4f/ii/solution)
  - [iii](#4f/iii)
    - [Solution](#4f/iii/solution)
- [5C](#5c)
  - [i](#5c/i)
    - [Solution](#5c/i/solution)
  - [ii](#5c/ii)
    - [Solution](#5c/ii/solution)
  - [iii](#5c/iii)
    - [Solution](#5c/iii/solution)
  - [iv](#5c/iv)
    - [Solution](#5c/iv/solution)
  - [v](#5c/v)
    - [Solution](#5c/v/solution)
- [6C](#6c)
  - [i](#6c/i)
    - [Solution](#6c/i/solution)
  - [ii](#6c/ii)
    - [Solution](#6c/ii/solution)
  - [iii](#6c/iii)
    - [Solution](#6c/iii/solution)
  - [iv](#6c/iv)
    - [Solution](#6c/iv/solution)
- [7C](#7c)
  - [a](#7c/a)
    - [i](#7c/a/i)
      - [Solution](#7c/a/i/solution)
    - [ii](#7c/a/ii)
      - [Solution](#7c/a/ii/solution)
    - [iii](#7c/a/iii)
      - [Solution](#7c/a/iii/solution)
  - [b](#7c/b)
    - [Solution](#7c/b/solution)
- [8C](#8c)
  - [i](#8c/i)
    - [Solution](#8c/i/solution)
  - [ii](#8c/ii)
    - [Solution](#8c/ii/solution)
  - [iii](#8c/iii)
    - [Solution](#8c/iii/solution)
- [9F](#9f)
  - [i](#9f/i)
    - [Solution](#9f/i/solution)
  - [ii](#9f/ii)
    - [Solution](#9f/ii/solution)
  - [iii](#9f/iii)
    - [Solution](#9f/iii/solution)
  - [iv](#9f/iv)
    - [Solution](#9f/iv/solution)
- [10F](#10f)
  - [i](#10f/i)
    - [Solution](#10f/i/solution)
  - [ii](#10f/ii)
    - [Solution](#10f/ii/solution)
  - [iii](#10f/iii)
    - [Solution](#10f/iii/solution)
  - [iv](#10f/iv)
    - [Solution](#10f/iv/solution)
  - [v](#10f/v)
    - [Solution](#10f/v/solution)
- [11F](#11f)
  - [a](#11f/a)
    - [Solution](#11f/a/solution)
  - [b](#11f/b)
    - [i](#11f/b/i)
      - [Solution](#11f/b/i/solution)
    - [ii](#11f/b/ii)
      - [Solution](#11f/b/ii/solution)
- [12F](#12f)
  - [i](#12f/i)
    - [Solution](#12f/i/solution)
  - [ii](#12f/ii)
    - [Solution](#12f/ii/solution)
  - [iii](#12f/iii)
    - [Solution](#12f/iii/solution)
  - [iv](#12f/iv)
    - [Solution](#12f/iv/solution)

## 1C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1c/solution">Solution</h3>

↑ **Parent:** [1C](#1c)

[Differentiation](../../../calculus.md#differentiation) under the [integral](../../../calculus.md#integral) gives $I\prime\prime=\int_0^1y^4e^{xy}dy$. Integrating the [derivative](../../../calculus.md#derivative) of $e^{xy}(xy^3-3y^2)$ and then once more yields $x^2\int_0^1y^4e^{xy}dy-12\int_0^1y^2e^{xy}dy=e^x(x-4)$.

## 2C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2c/a">a</h3>

↑ **Parent:** [2C](#2c)

<h4 id="2c/a/solution">Solution</h4>

↑ **Parent:** [A](#2c/a)

With $y=z/x^2$ the equation becomes $z\prime\prime+z=0$. Thus $y_1=\cos x/x^2$, $y_2=\sin x/x^2$, and $W(y_1,y_2)=x^{-4}\ne0$.

<h3 id="2c/b">b</h3>

↑ **Parent:** [2C](#2c)

<h4 id="2c/b/solution">Solution</h4>

↑ **Parent:** [B](#2c/b)

The transformed inhomogeneous equation is $z\prime\prime+z=x^2$. Taking $z=x^2-2$ gives the particular [integral](../../../calculus.md#integral) $y_p=1-2/x^2$.

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/i">i</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/i/solution">Solution</h4>

↑ **Parent:** [I](#3f/i)

Completing the square gives $X,Y\sim N(0,4/3)$, so each marginal is $\sqrt3(2\sqrt{2\pi})^{-1}e^{-3x^2/8}$. Their covariance is $2/3$, so they are not independent.

<h3 id="3f/ii">ii</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3f/ii)

From part (i),

$$
\operatorname{var}(X)=\operatorname{var}(Y)=\frac43,
\qquad \operatorname{cov}(X,Y)=\frac23.
$$

The conditional-normal formula therefore gives

$$
Y\mid X=x\sim
N\left(\frac{\operatorname{cov}(X,Y)}{\operatorname{var}(X)}x,
\operatorname{var}(Y)-
\frac{\operatorname{cov}(X,Y)^2}{\operatorname{var}(X)}\right)
=N\left(\frac x2,1\right).
$$

Consequently the [Gaussian conditional expectation](../../../statistical-modelling.md#gaussian-conditional-expectation) is

$$
\boxed{\mathbb E[Y\mid X]=\frac X2.}
$$

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/i">i</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/i/solution">Solution</h4>

↑ **Parent:** [I](#4f/i)

Writing $S_n=\sum I_i$, each $\mathbb EI_i=1/n$. Distinct indicators have joint probability $1/[n(n-1)]$ and zero covariance, so $\mathbb ES_n=1$ and $\operatorname{var}S_n=n(1/n)(1-1/n)=1-1/n$.

<h3 id="4f/ii">ii</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4f/ii)

[Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) applied to $X1_{X\gt 0}$ gives $(\mathbb EX)^2\le\mathbb E(X^2)\mathbb P(X\gt 0)$.

<h3 id="4f/iii">iii</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4f/iii)

Apply part (ii): $\mathbb P(S_n\gt 0)\ge1/\mathbb E(S_n^2)=1/(2-1/n)\ge1/2$.

## 5C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5c/i">i</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/i/solution">Solution</h4>

↑ **Parent:** [I](#5c/i)

$y_0\prime\prime=(x^2-1)y_0$, so $\alpha=1$.

<h3 id="5c/ii">ii</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5c/ii)

Substitution and cancellation give $f\prime\prime-2xf\prime+(\alpha-1)f=0$.

<h3 id="5c/iii">iii</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5c/iii)

Equating powers gives $(n+2)(n+1)a_{n+2}+(\alpha-1-2n)a_n=0$.

<h3 id="5c/iv">iv</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5c/iv)

$y\prime(0)=0$ forces the odd [series](../../../real-analysis.md#series-mathematics) to vanish. The even recurrence terminates at degree $2N$ precisely when $\alpha=4N+1$.

<h3 id="5c/v">v</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/v/solution">Solution</h4>

↑ **Parent:** [V](#5c/v)

After division by $e^{-x^2/2}$, $f\prime\prime-2xf\prime+8f=2$. The initial data and evenness give $f=1-3x^2+x^4$, hence $y=e^{-x^2/2}(1-3x^2+x^4)$.

## 6C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6c/i">i</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/i/solution">Solution</h4>

↑ **Parent:** [I](#6c/i)

$\nabla U=(3x^2-3+y^2,2y(x+1))$, so the [critical points](../../../analysis.md#critical-point) are $(\pm1,0)$. The [Hessian matrix](../../../calculus.md#hessian-matrix) at $(1,0)$ is $\operatorname{diag}(6,4)$, making it the [local minimum](../../../analysis.md#local-minimum); $(-1,0)$ is degenerate and not a minimum.

<h3 id="6c/ii">ii</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6c/ii)

$dU/dt=\nabla U\cdot(-\nabla U)=-|\nabla U|^2\le0$. The descending [gradient flow](../../../analysis.md#gradient-flow) trajectory from $(2,1)$ stays in its bounded contour basin and tends to the only [critical point](../../../analysis.md#critical-point) there, $(1,0)$.

<h3 id="6c/iii">iii</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6c/iii)

Writing $\xi=x-1$, $\eta=y$, the [linearization of a dynamical system](../../../algebra.md#linearization-of-a-dynamical-system) is $\dot\xi=-6\xi$, $\dot\eta=-4\eta$. Eliminating $t$ gives $\eta=C\xi^{2/3}$.

<a id="6c/iii/image-contours-and-descending-gradient-flow-for-the-2026-paper-ia-2-potential"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-2-gradient-flow.png)

**[Figure 1](#6c/iii/image-contours-and-descending-gradient-flow-for-the-2026-paper-ia-2-potential). Contours and descending gradient flow for the 2026 Paper IA 2 potential**. Contour lines of U equal x cubed minus 3x plus open parenthesis x plus 1 close parenthesis y squared are overlaid with the descending gradient field. The highlighted trajectory starts at open parenthesis 2 comma 1 close parenthesis and tends to the local minimum at open parenthesis 1 comma 0 close parenthesis; the other marked critical point is degenerate.

<h3 id="6c/iv">iv</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6c/iv)

Now $\dot U=-|\nabla U|^2+U_y\cos\omega t$, whose second term has either sign. Near the minimum, $\xi=C e^{-6t}$ and $\dot\eta+4\eta=\cos\omega t$, so

$$
\eta=C_2e^{-4t}+\frac{4\cos\omega t+\omega\sin\omega t}{16+\omega^2}.
$$

## 7C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7c/a">a</h3>

↑ **Parent:** [7C](#7c)

<h4 id="7c/a/i">i</h4>

↑ **Parent:** [A](#7c/a)

<h5 id="7c/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7c/a/i)

Spatial [derivatives](../../../calculus.md#derivative) vanish for $u=y(t)$, giving $\ddot y+\gamma\dot y+\omega^2y=f(t)$.

<h4 id="7c/a/ii">ii</h4>

↑ **Parent:** [A](#7c/a)

<h5 id="7c/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7c/a/ii)

The roots are $r=(-\gamma\pm\sqrt{\gamma^2-4\omega^2})/2$. They give oscillatory decay for $\gamma\lt 2\omega$, two exponential decays for $\gamma\gt 2\omega$, and $(A+Bt)e^{-\gamma t/2}$ at equality. All tend to zero.

<h4 id="7c/a/iii">iii</h4>

↑ **Parent:** [A](#7c/a)

<h5 id="7c/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7c/a/iii)

Put $T=\pi/\omega$, $t_0=T/2$, and $\Omega=\omega/2$. A solution satisfying both endpoint conditions is

$$
y=Ae^{-\gamma t/2}\sin(\Omega t)+\frac I\Omega e^{-\gamma(t-t_0)/2}\sin(\Omega(t-t_0))H(t-t_0),
$$

where $A=-\sqrt2I\omega^{-1}e^{\sqrt3\pi/4}$. The [derivative](../../../calculus.md#derivative) jumps by $I$ at $t_0$, as required.

<h3 id="7c/b">b</h3>

↑ **Parent:** [7C](#7c)

<h4 id="7c/b/solution">Solution</h4>

↑ **Parent:** [B](#7c/b)

Substitution gives $(\dot X^2-c^2)\phi\prime\prime-(\ddot X+\gamma\dot X)\phi\prime+\omega^2\phi=0$. Multiply by $\phi\prime$ and integrate over $\mathbb R$; decay kills the first and last [integrals](../../../calculus.md#integral), leaving $(\ddot X+\gamma\dot X)\int(\phi\prime)^2=0$. Thus a nonconstant profile requires $X=X_\infty+Ce^{-\gamma t}$ and approaches a fixed position.

## 8C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8c/i">i</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/i/solution">Solution</h4>

↑ **Parent:** [I](#8c/i)

During warming, $\dot\theta=\alpha(\theta_1-\theta)$ and $\theta=\theta_1-(\theta_1-\theta_0)e^{-\alpha t}$. During cooling, with $\tau=t-T$, $\dot\theta=-\alpha(\theta-\theta_0)$ and $\theta=\theta_0+(\theta_1-\theta_0)(1-e^{-\alpha T})e^{-\alpha\tau}$.

<h3 id="8c/ii">ii</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8c/ii)

$N(2T)/N(0)=\exp[-\int_0^{2T}\beta(\theta(t))dt]$. Evaluation gives the implicit equation

$$
\boxed{\beta_{\max}\left[T-\frac{e^{-\alpha T}(1-e^{-\alpha T})}{\alpha}\right]=\log100.}
$$

<h3 id="8c/iii">iii</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8c/iii)

For $x=\alpha T\ll1$, $e^{-x}(1-e^{-x})=x-\tfrac32x^2+O(x^3)$. Hence $\tfrac32\beta_{\max}\alpha T^2\sim\log100$ and

$$
\boxed{T\sim\sqrt{\frac{2\log100}{3\beta_{\max}\alpha}}.}
$$

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/i">i</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/i/solution">Solution</h4>

↑ **Parent:** [I](#9f/i)

Each of the $\binom n3$ triples is a triangle with probability $p^3$, so $\mathbb ET=\binom n3p^3$.

<h3 id="9f/ii">ii</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9f/ii)

[Markov inequality](../../../probability-inequality.md#markov-inequality) gives $\mathbb P(T\gt 0)\le\mathbb ET=O(n^{3-3\alpha})\to0$ when $\alpha\gt 1$.

<h3 id="9f/iii">iii</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#9f/iii)

[Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) gives $\mathbb P(T=0)\le\mathbb P(|T-\mathbb ET|\ge\mathbb ET)\le\operatorname{var}(T)/(\mathbb ET)^2\to0$.

<h3 id="9f/iv">iv</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#9f/iv)

Only triangle pairs sharing an edge have nonzero covariance, so

$$
\operatorname{var}T=\binom n3(p^3-p^6)+2\binom n2\binom{n-2}2(p^5-p^6).
$$

After division by $(\mathbb ET)^2$ this is $O(n^{-3}p^{-3}+n^{-2}p^{-1})\to0$ for $p=n^{-\alpha}$, $0\lt \alpha\lt 1$; use part (iii).

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/i">i</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/i/solution">Solution</h4>

↑ **Parent:** [I](#10f/i)

The waiting time is geometric with mean $1/p$.

<h3 id="10f/ii">ii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10f/ii)

First-step equations for states “no trailing H” and “one trailing H” give $E_0=1+qE_0+pE_1$, $E_1=1+qE_0$, hence $E_0=(1+p)/p^2$.

<h3 id="10f/iii">iii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10f/iii)

The word $HT$ has no proper self-overlap, so its mean waiting time is the reciprocal of its probability: $1/[p(1-p)]$. This also follows from two first-step equations.

<h3 id="10f/iv">iv</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#10f/iv)

The standard run recursion gives $E_n=1+p^{-1}+\cdots+p^{-n}=(1-p^n)/[(1-p)p^n]$.

<h3 id="10f/v">v</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/v/solution">Solution</h4>

↑ **Parent:** [V](#10f/v)

For $k\ge n$, $p_k(n)=\binom{k-1}{n-1}p^n(1-p)^{k-n}$. It is the sum of $n$ independent geometric variables, so the [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) applies with mean $n/p$ and standard deviation $\sqrt{n(1-p)}/p$. Take  
$k_a(n)=\lceil n/p+a\sqrt{n(1-p)}/p\rceil$ and $k_b(n)=\lfloor n/p+b\sqrt{n(1-p)}/p\rfloor$.

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

Shift the absorbing interval to $\{0,\ldots,a+1\}$ and start at $1$. The gambler’s-ruin harmonic [functions](../../../function.md) give $\mathbb P(\tau_a\lt \tau_{-1})=1/(a+1)$ and $\mathbb ET=1(a+1-1)=a$.

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/i">i</h4>

↑ **Parent:** [B](#11f/b)

<h5 id="11f/b/i/solution">Solution</h5>

↑ **Parent:** [I](#11f/b/i)

At time $T_k$ the visited vertices form a contiguous arc and the walk is at an endpoint. Exiting an interval of $k$ visited vertices, starting one step from an absorbing endpoint, has mean $k$. Therefore $\mathbb E(T_{k+1}-T_k)=k$ and $\mathbb ET_n=\sum_{k=1}^{n-1}k=n(n-1)/2$.

<h4 id="11f/b/ii">ii</h4>

↑ **Parent:** [B](#11f/b)

<h5 id="11f/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11f/b/ii)

For each $j\ne0$, cut the cycle at $j$. The event that $j$ is last is the event that the lifted walk covers the other $n-1$ residues before crossing that cut. Gambler’s ruin (or cyclic symmetry of the two expanding endpoints) gives $\mathbb P(Z=j)=1/(n-1)$.

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/i">i</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/i/solution">Solution</h4>

↑ **Parent:** [I](#12f/i)

Conditioning on generation $n$ and using independence gives $F_{n+1}(s)=F_n(F_1(s))$.

<h3 id="12f/ii">ii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12f/ii)

Differentiating at $s=1$ gives $\mathbb EX_{n+1}=\mu\mathbb EX_n$, hence $\mathbb EX_n=\mu^n$.

<h3 id="12f/iii">iii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12f/iii)

The extinction probability is the smallest fixed point of the convex generating [function](../../../function.md) $F_1$ in $[0,1]$. Since $F_1\prime(1)=\mu\le1$ and $p_0,p_2\gt 0$ make strict convexity relevant, the only fixed point is $1$.

<h3 id="12f/iv">iv</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#12f/iv)

Here $F_1(s)=1/(2-s)$ and $\mu=1$, so extinction is certain. Iteration gives

$$
F_n(s)=\frac{n-(n-1)s}{n+1-ns},
$$

and $\mathbb P(X_n=0)=F_n(0)=n/(n+1)$.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
