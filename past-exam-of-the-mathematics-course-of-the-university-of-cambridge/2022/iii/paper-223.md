# Paper 223

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_223.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_223.pdf)

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
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $m=F^{-1}(1/2)$ be the unique [median](../../../probability-theory.md#median). The [influence function of the sample median](../../../statistical-inference.md#influence-function-of-the-sample-median) is

$$
\operatorname{IF}(x;T,F)
=\frac{\mathbf1_{\{x>m\}}-\mathbf1_{\{x<m\}}}{2f(m)}
$$

away from $m$. Its second moment, equivalently the [asymptotic distribution of a sample median](../../../statistical-inference.md#asymptotic-distribution-of-a-sample-median), gives

$$
A(T,F)=\mathbb E_F[\operatorname{IF}(X;T,F)^2]
=\frac1{4f(F^{-1}(1/2))^2}.
$$

**No symmetry assumption is used:** the density is evaluated at the actual median of $F$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $F=(1-\epsilon)\Phi+\epsilon H$ and assume $0<\epsilon<1/2$. If $m$ is its median, then

$$
\frac{1/2-\epsilon}{1-\epsilon}
\leq\Phi(m)\leq
\frac1{2(1-\epsilon)}.
$$

Moreover its density satisfies $f(m)\geq(1-\epsilon)\phi(m)$. Since the [standard normal density](../../../probability-theory.md#standard-normal-density) decreases with $|m|$, the smallest possible density at the median occurs at either endpoint. Put

$$
q_\epsilon=\Phi^{-1}\!\left(\frac1{2(1-\epsilon)}\right)>0.
$$

The two endpoints are $\pm q_\epsilon$ by normal symmetry. The bound is attained by choosing a contaminating density supported strictly to the right of $q_\epsilon$, or symmetrically to the left of $-q_\epsilon$, with zero density at the selected median. Therefore

$$
\boxed{\max_{F\in\mathcal P_\epsilon(\Phi)}A(T,F)
=\frac1{4(1-\epsilon)^2\phi(q_\epsilon)^2}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Every symmetric contaminated distribution has median zero, so

$$
f(0)=(1-\epsilon)\phi(0)+\epsilon h(0)
\geq(1-\epsilon)\phi(0).
$$

A symmetric contaminating density supported away from zero attains equality. Hence

$$
\max_{\substack{F\in\mathcal P_\epsilon(\Phi)\\F\text{ symmetric}}}
A(T,F)
=\frac1{4(1-\epsilon)^2\phi(0)^2}
=\frac{\pi}{2(1-\epsilon)^2}.
$$

This is strictly smaller than the unrestricted answer because $q_\epsilon>0$ and $\phi(q_\epsilon)<\phi(0)$. Asymmetric contamination can move the median into a region of lower nominal density.

## 2

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The normal location score is $x-\theta$. Under a bound on [gross-error sensitivity](../../../statistical-inference.md#gross-error-sensitivity), the variance-minimizing influence curve clips this score. For $b>0$, define the [Huber score](../../../statistical-inference.md#huber-score)

$$
\psi_b(u)=[u]_{-b}^{b}
=\max(-b,\min(u,b)).
$$

The optimal [B-robust estimator](../../../statistical-inference.md#b-robust-estimator) is the [Huber location estimator](../../../statistical-inference.md#huber-location-estimator) $\widehat\theta_b$ defined by

$$
\sum_{i=1}^n\psi_b(x_i-\widehat\theta_b)=0.
$$

Equivalently, it has the explicit optimization form

$$
\widehat\theta_b
=\underset{t\in\mathbb R}{\arg\min}
\sum_{i=1}^n\rho_b(x_i-t),
$$

where the [Huber loss](../../../statistical-inference.md#huber-loss) is

$$
\rho_b(u)=
\begin{cases}
u^2/2,&|u|\leq b,\\
b|u|-b^2/2,&|u|>b.
\end{cases}
$$

At $N(\theta,1)$ its normalized influence function is

$$
\boxed{\operatorname{IF}(x;T_b,F_\theta)
=\frac{\psi_b(x-\theta)}{\mathbb P(|Z|\leq b)},
\qquad Z\sim N(0,1).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The gross-error bound corresponding to $b$ is

$$
c(b)=\frac{b}{\mathbb P(|Z|\leq b)}
=\frac{b}{2\Phi(b)-1}.
$$

It is strictly increasing because

$$
2\Phi(b)-1=\int_{-b}^b\phi(x)\,dx
>2b\phi(b),
$$

so the numerator of $c'(b)$ is positive. Furthermore

$$
\lim_{b\downarrow0}c(b)
=\frac1{2\phi(0)}=\sqrt{\frac\pi2},
\qquad
\lim_{b\to\infty}c(b)=\infty.
$$

**Thus $b\in(0,\infty)$ corresponds exactly to $c\in(\sqrt{\pi/2},\infty)$.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

As $b\downarrow0$, the Huber estimating equation approaches the sign equation

$$
\sum_i\operatorname{sgn}(x_i-\theta)=0,
$$

whose solution is the [sample median](../../../probability-theory.md#sample-median). Hence the most B-robust location M-estimator is the median, with minimum [gross-error sensitivity](../../../statistical-inference.md#gross-error-sensitivity)

$$
\boxed{\gamma^*=\frac1{2\phi(0)}=\sqrt{\frac\pi2}.}
$$

## 3

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $\Delta=\theta_1-\theta_0>0$. For one observation from the unit-variance normal location family,

$$
\log\frac{f_{\theta_1}(x)}{f_{\theta_0}(x)}
=\Delta\left(x-\frac{\theta_0+\theta_1}{2}\right).
$$

The sample log-[likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) is therefore $nT_n$. By the [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma), the level-$\alpha$ most powerful test rejects for a sufficiently large likelihood ratio, equivalently when $T_n>C_\alpha$, with $C_\alpha$ chosen to give null rejection probability $\alpha$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The functional is

$$
T(F)=\int\psi(x)\,dF(x),
\qquad
\psi(x)=\Delta\left(x-\frac{\theta_0+\theta_1}{2}\right).
$$

The [influence function](../../../statistical-inference.md#influence-function) of an expectation functional is

$$
\operatorname{IF}_{\rm test}(x;T,F_\theta)
=\psi(x)-\mathbb E_{F_\theta}\psi(X).
$$

Because $\psi$ is affine with nonzero slope, this is unbounded under both $F_{\theta_0}$ and $F_{\theta_1}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Now let

$$
\psi_{a,b}(x)
=\left[\Delta\left(x-\frac{\theta_0+\theta_1}{2}\right)\right]_a^b.
$$

Then

$$
\operatorname{IF}_{\rm test}(x;S,F_\theta)
=\psi_{a,b}(x)-\mathbb E_{F_\theta}\psi_{a,b}(X).
$$

Since $a\leq\psi_{a,b}(x)\leq b$, this influence function is bounded for both hypotheses. Clipping the log-likelihood contribution prevents one extreme observation from having unbounded effect on the statistic.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

Put $r(x)=f_{\theta_1}(x)/f_{\theta_0}(x)$. The proposed first density can be written

$$
g_{0,c}(x)=(1-\epsilon)
\max\!\left\{f_{\theta_0}(x),\frac{f_{\theta_1}(x)}c\right\}.
$$

Its integral is continuous and strictly decreasing in $c$, tends to infinity as $c\downarrow0$, and tends to $1-\epsilon$ as $c\to\infty$. Hence a unique $c>0$ makes its integral one. Since $g_{0,c}\geq(1-\epsilon)f_{\theta_0}$,

$$
g_{0,c}=(1-\epsilon)f_{\theta_0}+\epsilon h_0
$$

for the density $h_0=[g_{0,c}-(1-\epsilon)f_{\theta_0}]/\epsilon$.

Similarly,

$$
g_{1,d}(x)=(1-\epsilon)
\max\{f_{\theta_1}(x),d f_{\theta_0}(x)\}.
$$

Its integral is continuous and strictly increasing from $1-\epsilon$ to infinity as $d$ ranges from zero to infinity. The unique normalizing $d>0$ gives

$$
g_{1,d}=(1-\epsilon)f_{\theta_1}+\epsilon h_1
$$

for a density $h_1$. Thus $G_0\in\mathcal P_\epsilon(F_{\theta_0})$ and $G_1\in\mathcal P_\epsilon(F_{\theta_1})$.

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

Assume $d<c$. Directly comparing the two piecewise densities gives

$$
\frac{g_1(x)}{g_0(x)}=
\begin{cases}
d,&r(x)\leq d,\\
r(x),&d<r(x)<c,\\
c,&r(x)\geq c.
\end{cases}
$$

Since

$$
\log r(x)=\Delta\left(x-\frac{\theta_0+\theta_1}{2}\right),
$$

we obtain

$$
\log\frac{g_1(x)}{g_0(x)}
=\left[\Delta\left(x-\frac{\theta_0+\theta_1}{2}\right)\right]_{\log d}^{\log c}.
$$

**Thus the sample log-likelihood ratio is $nS_n$ with truncation values $a=\log d$ and $b=\log c$. Rejecting for large $S_n$ is exactly the likelihood-ratio test between the two least-favorable contaminated distributions.**

## 4

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Assume first that $0<\epsilon<1/2$, set $k=\lfloor\epsilon n\rfloor$, and replace the last $k$ observations by $100$. Among the remaining $m=n-k$ observations, let

$$
Y_i=\mathbf1_{\{X_i>\epsilon\}},
\qquad
p_\epsilon=\mathbb P(Z>\epsilon)=1-\Phi(\epsilon).
$$

The contaminated median exceeds $\epsilon$ whenever

$$
\sum_{i=1}^mY_i\geq\frac{n+1}{2}-k.
$$

The right-hand threshold divided by $m$ tends to

$$
q_\epsilon=\frac{1/2-\epsilon}{1-\epsilon}<p_\epsilon.
$$

Therefore, for all sufficiently large $n$, it is at most $p_\epsilon-\delta_\epsilon$ for some $\delta_\epsilon>0$. The [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) gives

$$
\mathbb P\!\left(
\sum_{i=1}^mY_i<\frac{n+1}{2}-k
\right)
\leq e^{-2m\delta_\epsilon^2}
\leq e^{-c_\epsilon n}.
$$

The supremum over adversarial perturbations is at least this explicit construction, proving the claim. When $\epsilon\geq1/2$, replacing at least half the sample makes the conclusion immediate.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Replace the same last $k$ vectors by $(100,\ldots,100)$. Applying part a to each independent Gaussian coordinate shows that the probability its contaminated coordinate median exceeds $\epsilon$ is at least $1-e^{-c_\epsilon n}$. Independence across coordinates and [Bernoulli's inequality](../../../algebra.md#bernoulli-s-inequality) give

$$
\mathbb P\!\left(
\widehat\mu_j>\epsilon\text{ for every }j
\right)
\geq(1-e^{-c_\epsilon n})^d
\geq1-de^{-c_\epsilon n}.
$$

For $n$ sufficiently large as a function of $d$ and $\epsilon$, the last expression is at least $1/2$. On this event,

$$
\|\widehat\mu\|_2>\epsilon\sqrt d,
$$

which proves the stated lower bound for the supremum over adversarial perturbations.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [coordinatewise median](../../../probability-theory.md#coordinatewise-median) suffers a contamination error of order $\epsilon\sqrt d$ with constant probability. In contrast, the [Tukey median](../../../statistical-inference.md#tukey-median) under an isotropic Gaussian model satisfies a high-probability Euclidean error bound of order

$$
\epsilon+\sqrt{\frac dn}+\sqrt{\frac{\log(1/\delta)}n}
$$

with probability at least $1-\delta$, up to universal constants. Its contamination term is dimension-free. Thus coordinatewise estimation loses a factor $\sqrt d$ in its dependence on adversarial contamination.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
