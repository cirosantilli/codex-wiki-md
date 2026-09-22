# Paper 223

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_223.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_223.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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

## 1

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $m=F^{-1}(1/2)$. Since $F$ has an everywhere positive density, it is continuous and strictly increasing, so $F(m)=1/2$. Membership in the [Kolmogorov neighborhood of a distribution](../../../statistical-inference.md#kolmogorov-neighborhood-of-a-distribution) gives

$$
\Phi(m)-\varepsilon\leq\frac12\leq\Phi(m)+\varepsilon.
$$

By the symmetry of the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution),

$$
-\Phi^{-1}\left(\frac12+\varepsilon\right)
\leq m\leq
\Phi^{-1}\left(\frac12+\varepsilon\right).
$$

The stated asymptotic-bias formula for the [sample median](../../../probability-theory.md#sample-median) therefore yields

$$
\boxed{\sup_{F\in\mathcal P_\varepsilon^K(\Phi)\cap\mathcal M}
b(\{T_n\},F)\leq b_1},
\qquad
b_1=\Phi^{-1}\left(\frac12+\varepsilon\right).
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write

$$
\mu_+=\lim_{n\to\infty}\mathbb E_{F_+}T_n.
$$

If $X_+\sim F_+$, then $X_+-2b_1\sim F_-$ because $F_-(t)=F_+(t+2b_1)$. The [translation-invariant estimator](../../../statistical-inference.md#translation-invariant-estimator) property gives

$$
\mu_-:=\lim_{n\to\infty}\mathbb E_{F_-}T_n
=\mu_+-2b_1.
$$

For every real $u$,

$$
\max\{|u|,|u-2b_1|\}\geq b_1.
$$

Taking $u=\mu_+$ shows that every admissible estimator has maximum asymptotic bias at least $b_1$ on the pair $\{F_+,F_-\}$. Therefore

$$
\inf_{\{T_n\}\subset\mathcal T}
\sup_{F\in\mathcal P_\varepsilon^K(\Phi)\cap\mathcal M}
b(\{T_n\},F)\geq b_1.
$$

Together with part a, this proves the [minimax asymptotic bias](../../../statistical-inference.md#minimax-asymptotic-bias) optimality of the median.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Define

$$
F_+(t)=\frac12\{\Phi(t)+\Phi(t-2b_1)\},
\qquad
F_-(t)=F_+(t+2b_1)
=\frac12\{\Phi(t)+\Phi(t+2b_1)\}.
$$

Thus $F_+$ is the equal mixture of $N(0,1)$ and $N(2b_1,1)$, while $F_-$ is the equal mixture of $N(0,1)$ and $N(-2b_1,1)$. They have finite variance and everywhere positive densities. Normal symmetry shows that $F_+$ is symmetric about $b_1$ and $F_-$ about $-b_1$.

For every $t$,

$$
0\leq\Phi(t)-\Phi(t-2b_1)
\leq\Phi(b_1)-\Phi(-b_1)=2\varepsilon,
$$

where the maximum occurs at $t=b_1$. Consequently

$$
|F_+(t)-\Phi(t)|
=\frac12|\Phi(t-2b_1)-\Phi(t)|
\leq\varepsilon.
$$

The same argument, shifted and reflected, applies to $F_-$. Hence both distributions belong to $\mathcal P_\varepsilon^K(\Phi)\cap\mathcal M$ and satisfy the required translation relation.

## 2

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $q_s=F^{-1}(s)$ and $k=-F^{-1}(\alpha)>0$. Symmetry gives $F^{-1}(1-\alpha)=k$. Differentiating the [trimmed mean](../../../statistical-inference.md#trimmed-mean) functional along $F_t=(1-t)F+t\Delta_x$ gives

$$
\operatorname{IF}(x;T,F)
=\frac1{1-2\alpha}
\int_\alpha^{1-\alpha}
\frac{s-\mathbf1_{\{x\leq q_s\}}}{f(q_s)}\,ds.
$$

Under the substitution $y=q_s$, symmetry implies

$$
\int_\alpha^{1-\alpha}\frac{s}{f(q_s)}\,ds
=\int_{-k}^kF(y)\,dy=k,
$$

while

$$
\int_\alpha^{1-\alpha}
\frac{\mathbf1_{\{x\leq q_s\}}}{f(q_s)}\,ds
=\int_{-k}^k\mathbf1_{\{x\leq y\}}\,dy.
$$

Evaluating the last integral in the three regions $x<-k$, $|x|\leq k$, and $x>k$ yields

$$
\boxed{
\operatorname{IF}(x;T,F)
=\frac1{1-2\alpha}
\begin{cases}
-k,&x<-k,\\
x,&|x|\leq k,\\
k,&x>k.
\end{cases}}
$$

This is the [influence function of a trimmed mean](../../../statistical-inference.md#influence-function-of-a-trimmed-mean), namely the [Huber score](../../../statistical-inference.md#huber-score) with clipping parameter $k$, divided by $1-2\alpha$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $m=\lfloor\alpha n\rfloor$. If at most $m$ observations are replaced arbitrarily, every order statistic retained between ranks $m+1$ and $n-m$ remains between the minimum and maximum of the unreplaced observations. The trimmed mean is therefore bounded as the replacement values diverge.

If more than $m$ observations are replaced by a common value tending to $+\infty$, at least one replacement remains after the largest $m$ observations are trimmed, and the trimmed mean tends to $+\infty$. The analogous construction tends to $-\infty$. Thus the largest fraction of arbitrary replacements for which boundedness is guaranteed is

$$
\boxed{\varepsilon_n^*=\frac{\lfloor\alpha n\rfloor}{n}}.
$$

This is the convention for the finite-sample [replacement breakdown point](../../../statistical-inference.md#replacement-breakdown-point) used in the question; the alternative convention based on the smallest breaking fraction reports $(m+1)/n$.

## 3

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write $y_i=|x_i|$. If $n$ is odd, the [sample median](../../../probability-theory.md#sample-median) $t=T_n$ equals one observation, with equally many $y_i$ below and above it; the corresponding terms $\operatorname{sign}(y_i/t-1)$ cancel and the median term is zero. If $n$ is even, the conventional median lies strictly between the two middle observations when the $y_i$ are distinct, so exactly half the terms are $-1$ and half are $+1$. In either case

$$
\frac1n\sum_{i=1}^n\psi(x_i/t)=0,
\qquad
\psi(u)=\operatorname{sign}(|u|-1).
$$

**Hence $T_n$ is a [Scale M-estimator](../../../statistical-inference.md#scale-m-estimator).**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

If $X\sim N(0,\theta^2)$, then $Y=|X|$ has a scaled [half-normal distribution](../../../probability-theory.md#half-normal-distribution) with

$$
G_\theta(y)=2\Phi(y/\theta)-1,
\qquad
g_\theta(y)=\frac2\theta\phi(y/\theta),
\qquad y>0.
$$

Put $c=\Phi^{-1}(3/4)$. The population median is $t_0=\theta c$, and the [asymptotic distribution of a sample median](../../../statistical-inference.md#asymptotic-distribution-of-a-sample-median) gives

$$
\boxed{
\sqrt n(T_n-\theta c)
\Longrightarrow
N\left(0,\frac{\theta^2}{16\phi(c)^2}\right)}.
$$

Under $H_0:\theta^2=1$, positivity of the scale means $\theta=1$. If $z_{1-\alpha}$ is the $(1-\alpha)$-quantile of the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution), an asymptotically level-$\alpha$ test rejects for

$$
\boxed{
T_n>c+\frac{z_{1-\alpha}}{4\phi(c)\sqrt n}}.
$$

Larger scale makes the population median $\theta c$ larger, so this is the appropriate one-sided rejection region.

## 4

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The upper envelope for $\psi$ implies

$$
e^{\psi(\theta x)}
\leq1+\theta x+\frac{\theta^2x^2}{2}.
$$

Writing $\mu_i=\mathbb E[X_i]$, taking expectations, and using $1+u\leq e^u$ gives

$$
\mathbb E e^{\psi(\theta X_i)-\theta\mu_i}
\leq e^{-\theta\mu_i}
\left(1+\theta\mu_i+\frac{\theta^2}{2}\mathbb E[X_i^2]\right)
\leq\exp\left(\frac{\theta^2}{2}\mathbb E[X_i^2]\right).
$$

[Independent random variables](../../../random-variable.md#independent-random-variables) then yield

$$
\boxed{
\mathbb E\exp\left\{\sum_{i=1}^n
(\psi(\theta X_i)-\theta\mathbb E[X_i])\right\}
\leq
\exp\left\{\frac{\theta^2}{2}\sum_{i=1}^n\mathbb E[X_i^2]\right\}}.
$$

Applying the lower envelope to $-\psi(\theta x)$ similarly gives

$$
\boxed{
\mathbb E\exp\left\{\sum_{i=1}^n
(\theta\mathbb E[X_i]-\psi(\theta X_i))\right\}
\leq
\exp\left\{\frac{\theta^2}{2}\sum_{i=1}^n\mathbb E[X_i^2]\right\}}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Markov inequality](../../../probability-inequality.md#markov-inequality) applied to the first exponential-moment bound gives

$$
\mathbb P\left\{
\frac1\theta\sum_{i=1}^n
(\psi(\theta X_i)-\theta\mu)\geq t
\right\}
\leq
\exp\left(-\theta t+\frac{\theta^2\sigma^2n}{2}\right).
$$

The second bound controls the lower tail. The [union bound](../../../probability-inequality.md#boole-s-inequality) therefore gives

$$
\mathbb P\left\{
\left|\frac1\theta\sum_{i=1}^n
(\psi(\theta X_i)-\theta\mu)\right|\geq t
\right\}
\leq
2\exp\left(-\theta t+\frac{\theta^2\sigma^2n}{2}\right).
$$

Since

$$
\widehat\mu_\theta-\mu
=\frac1{n\theta}\sum_{i=1}^n
(\psi(\theta X_i)-\theta\mu),
$$

putting $L=\log(2/\delta)$,

$$
\theta=\sqrt{\frac{2L}{\sigma^2n}},
\qquad
t=\sqrt{2\sigma^2nL}
$$

makes the exponent equal to $-L$. It follows that the [Catoni mean estimator](../../../statistical-inference.md#catoni-mean-estimator) satisfies

$$
\boxed{
\mathbb P\left(
|\widehat\mu_\theta-\mu|
\geq\sigma\sqrt{\frac{2\log(2/\delta)}n}
\right)\leq\delta}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
