# Paper 208

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20208.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20208.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 208](paper-208.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Disintegrate $Q$ successively as

$$
Q(dy)=Q_1(dy_1)Q_2(dy_2\mid y_1)\cdots Q_N(dy_N\mid y_{<N}).
$$

For each history $y_{<i}$, choose an optimal coupling of $P_i$ and $Q_i(\cdot\mid y_{<i})$. Sampling these couplings recursively produces a joint law of $(X,Y)$ with $Y\sim Q$. Its conditional $X_i$-marginal is always $P_i$ and is independent of the past, so $X\sim P_1\otimes\cdots\otimes P_N=P$. It is therefore a coupling $\pi\in\Pi(P,Q)$.

Write $c_i(y_{<i})$ for the conditional expected cost $w(X_i,Y_i)$ in the chosen coordinate coupling. The assumed one-coordinate [transport-entropy inequality](../../../probability-inequality.md#transport-entropy-inequality) gives

$$
\phi(c_i(y_{<i}))
\leq D\bigl(Q_i(\cdot\mid y_{<i})\Vert P_i\bigr).
$$

By [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) and the [chain rule for relative entropy](../../../probability-and-statistics.md#chain-rule-for-relative-entropy),

$$
\sum_{i=1}^N\phi\bigl(\mathbb E_\pi w(X_i,Y_i)\bigr)
\leq\sum_{i=1}^N\mathbb E_Q\phi(c_i(Y_{<i}))
\leq\sum_{i=1}^N\mathbb E_QD(Q_i(\cdot\mid Y_{<i})\Vert P_i)
=D(Q\Vert P).
$$

Taking the infimum over all couplings proves the [tensorization of a transport-entropy inequality](../../../probability-inequality.md#tensorization-of-a-transport-entropy-inequality).

## 2

↑ **Parent:** [Paper 208](paper-208.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $\mu=\mathbb EZ$ and $h(u)=(1+u)\log(1+u)-u$. For $\lambda>0$, the [Chernoff bound](../../../probability-inequality.md#chernoff-bound) and the assumed cumulant-generating-function estimate give

$$
\mathbb P(Z-\mu\geq t)
\leq\inf_{\lambda>0}
\exp\{-\lambda t+\mu(e^\lambda-\lambda-1)\}.
$$

The optimizer satisfies $e^\lambda=1+t/\mu$, and hence

$$
\mathbb P(Z-\mu\geq t)
\leq e^{-\mu h(t/\mu)}
\leq\exp\!\left(-\frac{t^2}{2\mu+2t/3}\right).
$$

For the left tail, apply the same argument at a negative parameter. If $0<t<\mu$ the optimizer satisfies $e^{-\lambda}=1-t/\mu$, giving

$$
\mathbb P(Z-\mu\leq-t)
\leq\exp\{-\mu[(1-t/\mu)\log(1-t/\mu)+t/\mu]\}
\leq e^{-t^2/(2\mu)}.
$$

For $t\geq\mu$, nonnegativity of $Z$ makes the strict lower-tail event empty, with the boundary handled directly.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $d_i=f(X)-f_i(X^{(i)})$. The [self-bounding function](../../../probability-inequality.md#self-bounding-function) assumptions say $0\leq d_i\leq1$ and $\sum_i d_i\leq Z$. Apply [tensorization of entropy](../../../probability-inequality.md#tensorization-of-entropy) to $e^{\lambda Z}$ and the one-coordinate entropy inequality. Since $\varphi(u)=e^u-u-1$ is convex and $\varphi(td)\leq d\varphi(t)$ for $0\leq d\leq1$, the resulting bound is

$$
\operatorname{Ent}(e^{\lambda Z})
\leq\varphi(-\lambda)\mathbb E[Ze^{\lambda Z}].
$$

Writing $\psi(\lambda)=\log\mathbb E e^{\lambda(Z-\mu)}$ and dividing by the moment-generating function reduces this to

$$
\left(\frac{\psi(\lambda)}{e^\lambda-1}\right)'
\leq\mu\left(\frac{-\lambda}{e^\lambda-1}\right)'.
$$

Both sides have finite limits at zero and $\psi(0)=\psi'(0)=0$. Integrating from zero to $\lambda$, with the direction interpreted correctly when $\lambda<0$, yields

$$
\psi(\lambda)\leq\mu(e^\lambda-\lambda-1)=\mu\varphi(\lambda),
$$

which is the required inequality.

## 3

↑ **Parent:** [Paper 208](paper-208.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [bounded differences property](../../../probability-inequality.md#bounded-differences-property) with $c_i=1$ means that changing only coordinate $i$ changes $f$ by at most one:

$$
|f(x)-f(x')|\leq1
$$

whenever $x_j=x'_j$ for all $j\ne i$.

The function is $g$-[certifiable](../../../probability-inequality.md#certifiable-function) when, whenever $f(x)=k$, there is a coordinate set $I$ with $|I|\leq g(k)$ such that every $y$ agreeing with $x$ on $I$ satisfies $f(y)\geq k$. The coordinates in $I$ form a certificate for the assertion that the value is at least $k$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The lower-tail form of the [entropy method for certifiable functions](../../../probability-inequality.md#entropy-method-for-certifiable-functions) states that a unit-bounded-difference, $g$-certifiable nonnegative integer-valued function satisfies

$$
\log\mathbb E e^{-\lambda(Z-\mathbb EZ)}
\leq\frac{\lambda^2}{2}\mathbb E[g(Z)]
\qquad(\lambda\geq0).
$$

It follows by applying entropy tensorization to a minimal certificate: only its at most $g(Z)$ coordinates can contribute to the one-sided variance proxy, and changing any one contributes at most one.

The Chernoff bound therefore gives

$$
\mathbb P(Z-\mathbb EZ\leq-t)
\leq\inf_{\lambda>0}
\exp\!\left(-\lambda t+\frac{\lambda^2}{2}\mathbb E[g(Z)]\right).
$$

Choosing $\lambda=t/\mathbb E[g(Z)]$ proves

$$
\mathbb P(Z-\mathbb EZ\leq-t)
\leq\exp\!\left(-\frac{t^2}{2\mathbb E[g(Z)]}\right).
$$

## 4

↑ **Parent:** [Paper 208](paper-208.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

There are $m=\binom n2$ independent edge indicators. Conditional on all indicators except one, changing that edge changes the [maximum matching number](../../../graph-theory.md#matching-number) by at most one. The conditional range is therefore at most one, so [Popoviciu inequality on variances](../../../variance.md#popoviciu-s-inequality-on-variances) bounds each conditional variance by $1/4$. The tensorized conditional-variance inequality gives

$$
\boxed{\operatorname{Var}(f(G))
\leq\sum_{e=1}^m\mathbb E\operatorname{Var}(f(G)\mid X_{-e})
\leq\frac m4=\frac1{4}\binom n2.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The same edge exposure shows that $f$ has bounded differences constants $c_e=1$ for its $m=\binom n2$ independent inputs. [McDiarmid inequality](../../../probability-inequality.md#mcdiarmid-s-inequality) therefore gives both one-sided bounds

$$
\boxed{\mathbb P(f(G)-\mathbb Ef(G)\geq t),
\quad
\mathbb P(f(G)-\mathbb Ef(G)\leq-t)
\leq\exp\!\left(-\frac{2t^2}{\binom n2}\right).}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Group the edge indicators into $n-1$ independent blocks

$$
B_i=(X_{ij}:j>i),
\qquad1\leq i<n.
$$

All edges in one block share vertex $i$. Replacing the entire block can change the maximum matching number by at most one: after deleting the at most one matched edge incident to $i$, a matching from either graph remains valid in the other. Applying [McDiarmid inequality](../../../probability-inequality.md#mcdiarmid-s-inequality) to these $n-1$ blocks gives

$$
\boxed{\mathbb P(f(G)-\mathbb Ef(G)\geq t),
\quad
\mathbb P(f(G)-\mathbb Ef(G)\leq-t)
\leq\exp\!\left(-\frac{2t^2}{n-1}\right).}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Part (a) only gives a standard-deviation scale of order $n$, and part (b) gives the same concentration scale. Part (c) improves this to order $\sqrt n$. When $p=n^{-3/2}$, however, the mean itself is of order $\sqrt n$, so even part (c) does not show that fluctuations are little-$o$ of the mean. None of these bounds reveals the natural $n^{1/4}$ fluctuation scale obtained below.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

As a function of the independent edge indicators, the maximum matching number is unit-Lipschitz. The event $f(G)\geq k$ is certified by exhibiting the $k$ present edges of a matching, so $f$ is $g(k)=k$ certifiable. The [Talagrand concentration inequality for certifiable functions](../../../probability-inequality.md#talagrand-concentration-inequality-for-certifiable-functions) around a median $M$ gives, for universal constants in the displayed standard version,

$$
\mathbb P(f(G)\leq M-t)\leq2e^{-t^2/(4M)},
\qquad
\mathbb P(f(G)\geq M+t)\leq2e^{-t^2/[4(M+t)]}.
$$

Here $M\asymp\sqrt n$. If $t/n^{1/4}\to\infty$, then $t^2/(M+t)\to\infty$, as does $t^2/M$ whenever the corresponding event is possible. Both tail probabilities therefore tend to zero. Thus deviations of any order larger than $n^{1/4}$ are unlikely.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
