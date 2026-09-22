# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperia_2_2018.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperia_2_2018.pdf)

**Table of contents**

- [1B](#1b)
  - [Solution](#1b/solution)
- [2B](#2b)
  - [Solution](#2b/solution)
- [3F](#3f)
  - [i](#3f/i)
    - [Solution](#3f/i/solution)
  - [ii](#3f/ii)
    - [Solution](#3f/ii/solution)
- [4F](#4f)
  - [a](#4f/a)
    - [Solution](#4f/a/solution)
  - [b](#4f/b)
    - [Solution](#4f/b/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6B](#6b)
  - [i](#6b/i)
    - [Solution](#6b/i/solution)
  - [ii](#6b/ii)
    - [Solution](#6b/ii/solution)
- [7B](#7b)
  - [Solution](#7b/solution)
- [8B](#8b)
  - [Solution](#8b/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [Solution](#9f/b/solution)
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
  - [c](#10f/c)
    - [Solution](#10f/c/solution)
- [11F](#11f)
  - [a](#11f/a)
    - [Solution](#11f/a/solution)
  - [b](#11f/b)
    - [Solution](#11f/b/solution)
- [12F](#12f)
  - [i](#12f/i)
    - [Solution](#12f/i/solution)
  - [ii](#12f/ii)
    - [Solution](#12f/ii/solution)
  - [iii](#12f/iii)
    - [Solution](#12f/iii/solution)

## 1B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1b/solution">Solution</h3>

↑ **Parent:** [1B](#1b)

Let $f(u)=au(1-u^2)$. A [fixed point](../../../function.md#fixed-point) satisfies $u=f(u)$, so

$$
u=0\quad\hbox{or}\quad u_\pm=\pm\sqrt{1-\frac1a}.
$$

The nonzero fixed points exist for $a<0$ or $a>1$. Local stability requires $|f'(u_*)|<1$, and

$$
f'(0)=a,\qquad f'(u_\pm)=3-2a.
$$

Away from the boundary values:

- $a<-1$: all three fixed points are unstable.
- $-1<a<0$: $0$ is stable and $u_\pm$ are unstable.
- $0<a<1$: only $0$ exists, and it is stable.
- $1<a<2$: $0$ is unstable and $u_\pm$ are stable.
- $a>2$: all three are unstable.

At $a=-1,1,2$ a multiplier has modulus one and linear stability is inconclusive; at $a=0$, $0$ is strongly stable.

## 2B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2b/solution">Solution</h3>

↑ **Parent:** [2B](#2b)

The [chain rule](../../../calculus.md#chain-rule) gives $dF(x,y(x))/dx=F_x+F_yy'$. Equality with $P+Qy'$ for every $y(x)$ therefore requires $F_x=P$ and $F_y=Q$, which implies $P_y=Q_x$. Conversely, on the plane this compatibility condition makes $P\,dx+Q\,dy$ an [exact differential](../../../differential-form.md#exact-differential), so a potential $F$ exists.

Here $P=4x^3+3y$, $Q=2y+3x$, and $P_y=Q_x=3$. Integrating gives $F=x^4+3xy+y^2$, hence

$$
\boxed{x^4+3xy+y^2=C.}
$$

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/i">i</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/i/solution">Solution</h4>

↑ **Parent:** [I](#3f/i)

By [independence](../../../random-variable.md#independent-random-variables) and the [binomial theorem](../../../combinatorics.md#binomial-theorem),

$$
\mathbb P(X+Y=n)
=\sum_{k=0}^n e^{-\lambda}\frac{\lambda^k}{k!}e^{-\mu}\frac{\mu^{n-k}}{(n-k)!}
=e^{-(\lambda+\mu)}\frac{(\lambda+\mu)^n}{n!}.
$$

Therefore **$X+Y\sim\operatorname{Poisson}(\lambda+\mu)$**.

<h3 id="3f/ii">ii</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3f/ii)

For $0\leq k\leq n$,

$$
\mathbb P(X=k\mid X+Y=n)
=\binom nk\left(\frac{\lambda}{\lambda+\mu}\right)^k
\left(\frac{\mu}{\lambda+\mu}\right)^{n-k}.
$$

Thus

$$
\boxed{X\mid(X+Y=n)\sim\operatorname{Binomial}\left(n,\frac{\lambda}{\lambda+\mu}\right).}
$$

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/a">a</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/a/solution">Solution</h4>

↑ **Parent:** [A](#4f/a)

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) is $|\mathbb E(XY)|^2\leq\mathbb E(X^2)\mathbb E(Y^2)$. [Markov inequality](../../../probability-inequality.md#markov-inequality) says that for $X\geq0$ and $a>0$, $\mathbb P(X\geq a)\leq\mathbb EX/a$.

[Jensen inequality](../../../real-analysis.md#jensen-s-inequality) states that for convex $\phi$,

$$
\boxed{\phi(\mathbb EX)\leq\mathbb E\phi(X).}
$$

Let $\mu=\mathbb EX$. A supporting line at $\mu$ gives $\phi(x)\geq\phi(\mu)+c(x-\mu)$. Taking expectations makes the linear term vanish.

<h3 id="4f/b">b</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/b/solution">Solution</h4>

↑ **Parent:** [B](#4f/b)

With $\mu=\mathbb EX$,

$$
\operatorname{Var}X=\sum_x\mathbb P(X=x)(x-\mu)^2.
$$

Every summand is nonnegative. If the sum is zero, every value of positive probability equals $\mu$, so **$\mathbb P(X=\mu)=1$**.

## 5B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

After multiplying by the inverse of the derivative matrix, the system is

$$
\dot z+Az=e^{-4t}\binom{2}{3b/2-1}+e^{-t}\binom{c-1}{-c/2-1},
\quad
A=\begin{pmatrix}2&-1\\-2&3\end{pmatrix}.
$$

Choose eigenvectors $(1,1)^T$ and $(-1/2,1)^T$ of eigenvalues $1$ and $4$, and write

$$
\binom xy=
\begin{pmatrix}1&-1/2\\1&1\end{pmatrix}\binom{w_1}{w_2}.
$$

Then

$$
\begin{aligned}
\dot w_1+w_1&=(b/2+1)e^{-4t}+(c/2-1)e^{-t},\\
\dot w_2+4w_2&=(b-2)e^{-4t}-ce^{-t}.
\end{aligned}
$$

The zero initial data give

$$
\boxed{\begin{aligned}
w_1&=\frac{b+2}{6}(e^{-t}-e^{-4t})+\frac{c-2}{2}te^{-t},\\
w_2&=(b-2)te^{-4t}-\frac c3(e^{-t}-e^{-4t}),\\
x&=w_1-\frac12w_2,\qquad y=w_1+w_2.
\end{aligned}}
$$

The $te^{-4t}$ and $te^{-t}$ terms are [resonant responses](../../../dynamical-systems.md#resonance). When $b=2$ or $c=2$, respectively, the corresponding resonant forcing vanishes and so does that secular factor.

## 6B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6b/i">i</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/i/solution">Solution</h4>

↑ **Parent:** [I](#6b/i)

Since $\partial_x=\alpha\partial_\xi+\beta\partial_\eta$ and $\partial_y=\partial_\xi+\partial_\eta$,

$$
\boxed{\begin{aligned}
A(\alpha,\beta)&=a\alpha^2+b\alpha+c,\\
B(\alpha,\beta)&=2a\alpha\beta+b(\alpha+\beta)+2c,\\
C(\alpha,\beta)&=a\beta^2+b\beta+c.
\end{aligned}}
$$

If $\alpha,\beta$ are the distinct real roots of $as^2+bs+c$, then $A=C=0$ and $B=(4ac-b^2)/a\ne0$. Thus $v_{\xi\eta}=0$. For $s^2+3s+2=(s+1)(s+2)$, take $\xi=y-x$, $\eta=y-2x$, obtaining

$$
\boxed{u(x,y)=f(y-x)+g(y-2x)}
$$

for arbitrary twice differentiable functions $f,g$.

<h3 id="6b/ii">ii</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6b/ii)

If $\alpha=-b/(2a)$ is a repeated root, then $A=0$ and both coefficients of $\beta$ in $B$ vanish, so $B=0$ for every $\beta$. Choose $\beta\ne\alpha$, giving $C\ne0$ and hence $v_{\eta\eta}=0$. For $(s+1)^2$, take $\xi=y-x$, $\eta=y$, and obtain

$$
\boxed{u(x,y)=f(y-x)+y\,g(y-x).}
$$

## 7B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7b/solution">Solution</h3>

↑ **Parent:** [7B](#7b)

After division by $x^2$, the equation is $y''+x^{-1}y'-(1+\alpha^2x^{-2})y=0$. Every $x\ne0$ is an [ordinary point](../../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation). The origin is singular, but it is a [regular singular point](../../../complex-analysis.md#regular-singular-point) because $xP(x)=1$ and $x^2Q(x)=-(x^2+\alpha^2)$ are analytic there. An ordinary point has analytic normalized coefficients $P,Q$; a singular point failing the displayed regularity test is irregular.

The [Frobenius method](../../../complex-analysis.md#frobenius-method) ansatz $y=x^r\sum_{n\geq0}a_nx^n$ gives the indicial equation $r^2-\alpha^2=0$, $a_1=0$, and

$$
a_n=\frac{a_{n-2}}{(n+r)^2-\alpha^2}.
$$

For nonintegral $\alpha$, two independent solutions are

$$
\boxed{\begin{aligned}
y_+&=x^\alpha\left(1+\frac{x^2}{4(\alpha+1)}
+\frac{x^4}{32(\alpha+1)(\alpha+2)}+\cdots\right),\\
y_-&=x^{-\alpha}\left(1+\frac{x^2}{4(1-\alpha)}
+\frac{x^4}{32(1-\alpha)(2-\alpha)}+\cdots\right).
\end{aligned}}
$$

For integral $\alpha$, put $m=|\alpha|$. In the $r=-m$ recurrence the denominator vanishes at $n=2m$, so that series fails or coincides in the exceptional $m=0$ case. Up to scale the single Frobenius series is

$$
\boxed{y_1=x^m\left(1+\frac{x^2}{4(m+1)}
+\frac{x^4}{32(m+1)(m+2)}+\cdots\right),\quad
a_{2k}=\frac{a_{2k-2}}{4k(m+k)}.}
$$

For $\alpha=1$, $y_1=x(1+x^2/8+\cdots)$, so

$$
\frac1{s\,y_1(s)^2}=s^{-3}-\frac1{4s}+O(s).
$$

Its integral contains both $s^{-2}$ and $\log s$; multiplying by $y_1$ leaves a pole and a logarithmic term. Thus the reduction-of-order solution is not a power series at zero.

## 8B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8b/solution">Solution</h3>

↑ **Parent:** [8B](#8b)

Put $\theta=T-T_r$ and $u=U-T_r$. The term $-a\theta$ models oven cooling to the room, $Q$ is heater input, and $-bu=b\theta-bu$ makes the pizza relax toward the oven temperature. Both protocols supply unit total heat because $\int\delta(t)\,dt=1$ and the rectangular pulse has height $1/\tau$ and width $\tau$.

For the impulse, $\theta$ jumps by one at zero while $u$ remains continuous:

$$
\boxed{\theta_1(t)=e^{-at},\qquad
u_1(t)=\frac{b}{b-a}(e^{-at}-e^{-bt})}
$$

for $a\ne b$; when $a=b$, $u_1=bte^{-bt}$.

Define causal functions

$$
G_a(t)=H(t)\frac{1-e^{-at}}a,\qquad
K(t)=H(t)\frac{b}{b-a}\left(\frac{1-e^{-at}}a-\frac{1-e^{-bt}}b\right).
$$

The rectangular-pulse solutions are

$$
\boxed{\theta_2(t)=\frac{G_a(t)-G_a(t-\tau)}{\tau},\qquad
u_2(t)=\frac{K(t)-K(t-\tau)}{\tau}.}
$$

Finally $T_i=T_r+\theta_i$, $U_i=T_r+u_i$. These formulas make $T_2,U_2$ continuous at $0,\tau$; only $T_1$ jumps at the delta impulse. As $\tau\to0$, the difference quotients tend to $G_a'=\theta_1$ and $K'=u_1$, because the rectangular pulse is an [approximate identity](../../../fourier-analysis.md#approximate-identity).

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

Independence gives $\mathbb EE(Z)=\sum_{z,y}F(y,z)\mathbb P(Y=y)\mathbb P(Z=z)=\mathbb EF(Y,Z)$. Moreover, $\mathbb EV(Z)=\mathbb E(F(Y,Z)^2)-\mathbb E(E(Z)^2)$, while $\operatorname{Var}E(Z)=\mathbb E(E(Z)^2)-(\mathbb EF(Y,Z))^2$. Adding proves the [law of total variance](../../../probability-theory.md#law-of-total-variance)

$$
\boxed{\operatorname{Var}F(Y,Z)=\mathbb EV(Z)+\operatorname{Var}E(Z).}
$$

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

For one Bernoulli variable, direct expansion gives $\operatorname{Var}F(X_1)=p(1-p)(F(1)-F(0))^2$. Applying the law of total variance successively to the coordinates gives the [variance tensorization](../../../probability-inequality.md#variance-tensorization)

$$
\boxed{\operatorname{Var}F(X)\leq p(1-p)\sum_{i=1}^n
\mathbb E\bigl(F(X)-F(X^i)\bigr)^2.}
$$

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

For any $x,z\in\{\pm1\}$ there is exactly one $y=xz$, so $\mathbb P(X=x,Z=z)=1/4=\mathbb P(X=x)\mathbb P(Z=z)$. Similarly $(Y,Z)$ is independent, and $(X,Y)$ is independent by assumption. They are pairwise independent but **not jointly independent**, because $XYZ=1$ surely.

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

Using $\max\{X^2,Y^2\}=(X^2+Y^2+|X^2-Y^2|)/2$ and [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality),

$$
\mathbb E\max\{X^2,Y^2\}
\leq1+\frac12\sqrt{\mathbb E(X-Y)^2\,\mathbb E(X+Y)^2}
=\boxed{1+\sqrt{1-\rho^2}}.
$$

<h3 id="10f/c">c</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/c/solution">Solution</h4>

↑ **Parent:** [C](#10f/c)

At most two of $X_1>X_2$, $X_2>X_3$, and $X_3>X_1$ can hold in any outcome. Taking expectations gives $a_{12}+a_{23}+a_{31}\leq2$, and hence **$\min\{a_{12},a_{23},a_{31}\}\leq2/3$**.

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

Let $q_n=\mathbb P(X_n=0)$ for a [Galton-Watson process](../../../probability-and-statistics.md#galton-watson-process) starting from one ancestor. Conditional on $X_1=k$, extinction by generation $n+1$ requires $k$ independent descendant processes to be extinct by generation $n$, so

$$
q_{n+1}=F(q_n),\qquad q_0=0.
$$

Because zero is absorbing, $q_n\uparrow q$, the eventual extinction probability, and continuity gives $q=F(q)$. If $r\geq0$ is any fixed point, monotonicity of $F$ and $q_0\leq r$ give $q_n\leq r$ inductively. Thus $q$ is the smallest nonnegative fixed point.

Here $F(s)=s/4+3s^3/4$. Every individual has at least one child, so **$q=0$**. The offspring mean is $F'(1)=5/2$, hence

$$
\boxed{\mathbb EX_n=(5/2)^n.}
$$

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/solution">Solution</h4>

↑ **Parent:** [B](#11f/b)

Represent $Y_n$ as a sum of $n$ independent $\operatorname{Poisson}(1)$ variables. The [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) gives

$$
\boxed{\frac{Y_n-n}{\sqrt n}\xrightarrow{\mathrm d}N(0,1).}
$$

Since zero is a continuity point of the standard normal distribution,

$$
e^{-n}\sum_{k=0}^n\frac{n^k}{k!}
=\mathbb P(Y_n\leq n)\longrightarrow\boxed{\frac12}.
$$

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/i">i</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/i/solution">Solution</h4>

↑ **Parent:** [I](#12f/i)

For $x\geq m$, $X_n=x$ implies $M_n\geq m$. For $x<m$, reflect every step after the first visit to $m$. The [reflection principle for simple symmetric random walk](../../../martingale.md#reflection-principle-for-simple-symmetric-random-walk) bijects such paths ending at $x$ with unrestricted paths ending at $2m-x$. Therefore

$$
\boxed{\mathbb P(M_n\geq m,X_n=x)=
\begin{cases}\mathbb P(X_n=x),&x\geq m,\\
\mathbb P(X_n=2m-x),&x<m.
\end{cases}}
$$

<h3 id="12f/ii">ii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12f/ii)

Summing part i and reindexing gives

$$
\boxed{\mathbb P(M_n\geq m)=\mathbb P(X_n=m)+2\sum_{x>m}\mathbb P(X_n=x).}
$$

Subtracting the formula for $m+1$ yields

$$
\boxed{\mathbb P(M_n=m)=\mathbb P(X_n=m)+\mathbb P(X_n=m+1).}
$$

<h3 id="12f/iii">iii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12f/iii)

Using part ii and symmetry of the [simple random walk](../../../markov-process.md#simple-random-walk),

$$
\mathbb EX_n^2-\mathbb EM_n^2
=\sum_{k\geq1}(2k-1)\mathbb P(X_n=k)>0
$$

for $n\geq1$. Thus **$\mathbb EM_n^2<\mathbb EX_n^2=n$**.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
