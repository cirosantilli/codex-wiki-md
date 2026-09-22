# Paper 217

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20217.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20217.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 217](paper-217.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Because $V$ is measurable for the [cylinder sigma-algebra](../../../probability-theory.md#cylinder-sigma-algebra), membership in $V$ depends on only countably many coordinates $T_0=\{t_1,t_2,\ldots\}$. Its image in $\mathbb R^{T_0}$ is a measurable linear subspace $V_0$, and

$$
\{X\in V\}=\{(X(t_j))_{j\geq1}\in V_0\}.
$$

By successively applying the finite-dimensional Gaussian regression formula, realize this Gaussian sequence as a lower-triangular linear transform of independent standard normal variables:

$$
(X(t_j))_{j\geq1}=\sum_{k\geq1}g_k a_k,
$$

where every coordinate of the sum contains only finitely many terms. If some deterministic column $a_k$ does not belong to $V_0$, then, after conditioning on every $g_j$ except $g_k$, at most one value of $g_k$ can put the sum in $V_0$. The continuous normal distribution gives probability zero. If every $a_k$ belongs to $V_0$, changing finitely many $g_k$ does not change the membership event. It is then a [tail event](../../../probability-theory.md#tail-event), and the [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law) gives probability zero or one. This proves the [Gaussian zero-one law for measurable linear subspaces](../../../stochastic-process.md#gaussian-zero-one-law-for-measurable-linear-subspaces).

Now let $X(t)=\sqrt t,g_t$ for independent standard normal variables $g_t$. Define

$$
V=\left\{x\in\mathbb R^{\mathbb N}:\frac{x_t}{t}\longrightarrow0\right\},
\qquad
W=\ell^2.
$$

Both are cylinder-measurable infinite-dimensional linear subspaces. For every $\varepsilon>0$,

$$
\sum_{t=1}^\infty\mathbb P(|g_t|>\varepsilon\sqrt t)<\infty,
$$

so the [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas) imply $g_t/\sqrt t\to0$ almost surely and hence $\mathbb P(X\in V)=1$. On the other hand, $g_t^2\geq1$ infinitely often almost surely, again by Borel-Cantelli, so

$$
\sum_{t=1}^\infty|X(t)|^2=\sum_{t=1}^\infty t g_t^2=\infty
$$

almost surely. Therefore $\mathbb P(X\in W)=0$.

## 2

↑ **Parent:** [Paper 217](paper-217.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let

$$
A_k=\{\lVert S_j\rVert\leq t\text{ for }j<k, \lVert S_k\rVert>t\}
$$

be the event that the partial sums first cross level $t$ at time $k$. On $A_k$, write $R_k=S_n-S_k$. Conditional on $X_1,\ldots,X_k$, the random variable $R_k$ is independent and symmetric. Since

$$
2\lVert S_k\rVert
\leq\lVert S_k+R_k\rVert+\lVert S_k-R_k\rVert,
$$

at least one of the two norms on the right exceeds $t$. Symmetry of $R_k$ consequently gives

$$
\mathbb P(\lVert S_n\rVert>t\mid X_1,\ldots,X_k)\geq\frac12
$$

on $A_k$. The events $A_k$ are disjoint, so summation proves the [Lévy maximal inequality](../../../probability-inequality.md#levy-maximal-inequality)

$$
\mathbb P\left(\max_{1\leq k\leq n}\lVert S_k\rVert>t\right)
\leq2\mathbb P(\lVert S_n\rVert>t).
$$

For the Gaussian series, put $S_m=\sum_{j=1}^mg_ju_j$. Apply the inequality to the symmetric independent increments from $n+1$ through $m$, followed by [Markov inequality](../../../probability-inequality.md#markov-inequality) in squared norm:

$$
\begin{aligned}
\mathbb P\left(\max_{n<k\leq m}\lVert S_k-S_n\rVert_V>\varepsilon\right)
&\leq2\mathbb P(\lVert S_m-S_n\rVert_V>\varepsilon)\\
&\leq\frac2{\varepsilon^2}\mathbb E\lVert S_m-S_n\rVert_V^2
=\frac2{\varepsilon^2}\sum_{j=n+1}^m\lVert u_j\rVert_V^2.
\end{aligned}
$$

Here the cross terms vanish by [orthogonality of independent centered Hilbert-space random variables](../../../random-variable.md#orthogonality-of-independent-centered-hilbert-space-random-variables). Letting $m\to\infty$ and then $n\to\infty$ shows

$$
\mathbb P\left(\sup_{k\geq n}\lVert S_k-S_n\rVert_V>\varepsilon\right)\longrightarrow0.
$$

The convergence criterion in the question now shows that $\sum_jg_ju_j$ converges almost surely in $V$.

## 3

↑ **Parent:** [Paper 217](paper-217.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The spectral characterization of the [Reproducing-kernel Hilbert space of a stationary Gaussian process](../../../probability-and-statistics.md#reproducing-kernel-hilbert-space-of-a-stationary-gaussian-process) says that its elements are precisely the functions whose Fourier transforms satisfy

$$
\lVert f\rVert_{\mathcal H_K}^2
=c\int_{\mathbb R}\frac{|\widehat f(u)|^2}{\widehat K(u)}\,du<\infty,
$$

with $c$ determined only by the [Fourier transform](../../../analysis.md#fourier-transform) convention. Here $\widehat K(u)=(1+u^2)^{-1}$, so

$$
\lVert f\rVert_{\mathcal H_K}^2
=c\int_{\mathbb R}(1+u^2)|\widehat f(u)|^2\,du.
$$

This is an equivalent norm for the [Sobolev space](../../../sobolev-space.md) $H^1(\mathbb R)$, and hence the RKHS equals $H^1(\mathbb R)$ as a set.

Since $\widehat K$ is integrable, $K$ is continuous and the process has a jointly measurable separable version. For every finite Borel measure $\nu$ on $\mathbb R$, [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) gives

$$
\mathbb E\lVert X\rVert_{L^2(\nu)}^2
=\int_{\mathbb R}\mathbb E|X(t)|^2\,d\nu(t)
=K(0)\nu(\mathbb R)<\infty.
$$

Thus $X\in L^2(\mathbb R,\nu)$ almost surely and is a Borel random variable there. Every continuous linear functional of $X$ is a centered normal random variable: approximate its $L^2(\nu)$ integral by finite linear combinations of process values and pass to the $L^2$ limit. Therefore the induced law is a [Gaussian Borel measure](../../../stochastic-process.md#gaussian-measure) on $L^2(\mathbb R,\nu)$.

## 4

↑ **Parent:** [Paper 217](paper-217.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $e_n(t)=\sqrt2\sin(n\pi t)$, let $(g_n)$ be independent standard normal variables, and choose $a_n=e^{-n^2}$. Define

$$
X(t)=\sum_{n=1}^\infty a_ng_ne_n(t).
$$

Finite collections of values are limits of centered Gaussian vectors, so this is a centered [Gaussian process](../../../stochastic-process.md#gaussian-process).

The functions $(e_n)$ are an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $H=L^2(0,1)$. Hence

$$
\mathbb E\lVert X\rVert_H^2=\sum_{n=1}^\infty a_n^2<\infty,
$$

which proves $\mu_X(H)=1$. For every integer $k\geq0$,

$$
\mathbb E\sum_{n=1}^\infty
|a_ng_n|\lVert e_n^{(k)}\rVert_\infty
\leq C_k\mathbb E|g_1|\sum_{n=1}^\infty e^{-n^2}n^k<\infty.
$$

Thus, almost surely and simultaneously for all $k$, the differentiated series converges uniformly on $(0,1)$. Termwise differentiation gives an almost surely infinitely differentiable version.

Finally, let $F\subset H$ be finite-dimensional. Choose a nonzero $h\in F^\perp$. Then

$$
\langle X,h\rangle_H
=\sum_{n=1}^\infty a_ng_n\langle e_n,h\rangle_H
$$

is a centered normal variable of variance

$$
\sum_{n=1}^\infty a_n^2|\langle e_n,h\rangle_H|^2>0,
$$

because every $a_n$ is positive and $(e_n)$ is complete. The event $\{X\in F\}$ is contained in $\{\langle X,h\rangle_H=0\}$, which has probability zero because a nondegenerate normal distribution has no atoms. Therefore $\mu_X(F)=0$ for every finite-dimensional linear subspace $F$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
