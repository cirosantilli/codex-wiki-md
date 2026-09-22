# Paper 137

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_137.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_137.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For an integer $k$ and a [congruence subgroup](../../../group-theory.md#congruence-subgroup) $\Gamma\leq SL_2(\mathbb Z)$, the space $M_k(\Gamma)$ consists of [holomorphic functions](../../../complex-analysis.md#holomorphic-function) $f:\mathfrak h\to\mathbb C$ satisfying

$$
(f|_k\gamma)(\tau)=(c\tau+d)^{-k}f(\gamma\tau)=f(\tau)
$$

for every $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma$, and which are [holomorphic at every cusp](../../../modular-function.md#holomorphic-at-a-cusp). This is the space of [modular forms](../../../modular-function.md#modular-form) of weight $k$ and level $\Gamma$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a compact subset $C\subset\mathfrak h$, the real-linear map

$$
\mathbb R^2\longrightarrow\mathbb C,
\qquad(c,d)\longmapsto c\tau+d
$$

has inverse norm bounded uniformly for $\tau\in C$. Hence there is $A_C>0$ such that

$$
|c\tau+d|\geq A_C\sqrt{c^2+d^2}.
$$

Therefore the absolute value of the defining series is bounded locally uniformly by

$$
A_C^{-k}\sum_{(c,d)\ne(0,0)}(c^2+d^2)^{-k/2},
$$

which converges for $k>2$. The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) gives locally uniform absolute convergence, so termwise holomorphy proves that $G_k^{(x,y)}$ is holomorphic.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $\gamma=\begin{pmatrix}a&b\\r&s\end{pmatrix}$. The [automorphy factor](../../../modular-function.md#automorphy-factor) identity gives

$$
(r\tau+s)^{-k}(c\gamma\tau+d)^{-k}
=((c,d)\gamma(\tau,1)^T)^{-k}.
$$

Right multiplication by $\gamma$ bijects $\mathbb Z^2\setminus\{0\}$ and carries the congruence class $(x,y)$ to $(x,y)\gamma$. Reindexing the absolutely convergent series yields

$$
\boxed{G_k^{(x,y)}|_k\gamma=G_k^{(x,y)\gamma}.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

If $\gamma\in\Gamma(N)$, then $(x,y)\gamma\equiv(x,y)\pmod N$, so part c gives invariance. It remains to check the cusps. For any $\sigma\in SL_2(\mathbb Z)$,

$$
G_k^{(x,y)}|_k\sigma=G_k^{(x,y)\sigma}.
$$

As $\operatorname{Im}\tau\to\infty$, the terms with $c=0$ give a finite constant and the locally uniform estimate for the terms with $c\ne0$ gives boundedness. A periodic holomorphic function bounded at infinity has a Fourier expansion with no negative powers. Thus every slash transform is holomorphic at infinity, which is holomorphy at every cusp. Hence $G_k^{(x,y)}$ is the [congruence-class Eisenstein series](../../../modular-function.md#congruence-class-eisenstein-series) in $M_k(\Gamma(N))$.

## 2

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For fixed $\tau=x+iy$, the set $\{|c\tau+d|:(c,d)\in\mathbb Z^2\setminus\{0\}\}$ has a positive minimum. Choose a primitive pair $(c,d)$ attaining it and complete it to a matrix $\gamma\in SL_2(\mathbb Z)$. Since

$$
\operatorname{Im}(\gamma\tau)=\frac{y}{|c\tau+d|^2},
$$

this point has maximal imaginary part in the orbit. Translate by a power of $T:\tau\mapsto\tau+1$ to arrange $|\operatorname{Re}\tau|\leq1/2$. If now $|\tau|<1$, applying $S:\tau\mapsto-1/\tau$ strictly increases the imaginary part, a contradiction. Thus $|\tau|\geq1$, proving that every orbit meets the [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group) $\mathcal F$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a cusp form $f$, the [invariant norm of a modular form](../../../modular-function.md#invariant-norm-of-a-modular-form)

$$
y^{k/2}|f(x+iy)|
$$

is modular invariant, bounded on $\mathcal F$, and tends to zero at its cusp. Part a therefore makes it bounded throughout $\mathfrak h$: $|f(x+iy)|\leq Cy^{-k/2}$.

The correct PDF expansion is $f(\tau)=\sum_{n\geq1}a_n(f)q^n$. Fourier inversion gives

$$
a_n(f)e^{-2\pi ny}=\int_0^1f(x+iy)e^{-2\pi inx}\,dx,
$$

and hence

$$
|a_n(f)|\leq Ce^{2\pi ny}y^{-k/2}.
$$

Choosing $y=1/n$ proves the [Fourier coefficient bound for a cusp form](../../../modular-function.md#fourier-coefficient-bound-for-a-cusp-form) $|a_n(f)|\leq C'n^{k/2}$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The corrected PDF integrand is

$$
f(\tau)\overline{G_k(\tau)}y^k\frac{dx\,dy}{y^2},
$$

so the integral is a [Petersson inner product](../../../modular-function.md#petersson-inner-product). On compact subsets it is harmless, while at the cusp the exponential decay of $f$ dominates the polynomial growth of the Eisenstein series; therefore it converges absolutely.

Decompose each nonzero pair uniquely into a positive common divisor times a primitive pair. For even $k$ this writes $G_k$ as $2\zeta(k)$ times the Eisenstein sum over $\Gamma_\infty\backslash SL_2(\mathbb Z)$. Unfolding the fundamental domain gives a constant multiple of

$$
\int_0^\infty\int_0^1 f(x+iy)y^{k-2}\,dx\,dy.
$$

The inner integral is the constant Fourier coefficient of the cusp form and is zero. Thus the original integral is zero, expressing the [orthogonality of cusp forms and holomorphic Eisenstein series](../../../modular-function.md#orthogonality-of-cusp-forms-and-holomorphic-eisenstein-series).

## 3

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Gamma 1 congruence subgroup](../../../group-theory.md#gamma-1-congruence-subgroup) is

$$
\Gamma_1(N)=\left\{\begin{pmatrix}a&b\\c&d\end{pmatrix}\in SL_2(\mathbb Z):
a\equiv d\equiv1\pmod N,\ c\equiv0\pmod N\right\}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The point $1/N+\Lambda_\tau$ has exact order $N$, and changing $\tau$ by $\Gamma_1(N)$ changes the pair only by a complex scaling, so the stated map is well-defined.

Conversely, scale a lattice to write it as $\mathbb Z\tau\oplus\mathbb Z$. A point of exact order $N$ is represented by $(r\tau+s)/N$, where $(r,s)$ is primitive modulo $N$. The group $SL_2(\mathbb Z)$ acts transitively on primitive vectors modulo $N$, so a basis change carries this point to $1/N$. This proves surjectivity. Two resulting normalized pairs are similar precisely when their basis-change matrix fixes $(0,1)$ modulo $N$, namely when it lies in $\Gamma_1(N)$. This proves injectivity and the [Gamma 1 level structure on a complex lattice](../../../modular-function.md#gamma-1-level-structure-on-a-complex-lattice) bijection

$$
\boxed{\Gamma_1(N)\backslash\mathfrak h\cong\mathbb C^\times\backslash\mathcal L(N).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Index-$p$ overlattices $\Lambda'$ correspond to order-$p$ subgroups of $(p^{-1}\Lambda)/\Lambda\cong\mathbb F_p^2$, hence to the $p+1$ lines in that vector space.

If $p\nmid N$, the order of $v+\Lambda'$ cannot decrease: its decrease would have a factor dividing both $p=[\Lambda':\Lambda]$ and $N$. Thus all $p+1$ overlattices are counted.

If $p\mid N$, the element $(N/p)v+\Lambda$ is a nonzero point of order $p$ in $\mathbb C/\Lambda$. Exactly one of the $p+1$ overlattices contains it; in that overlattice the image of $v$ has order $N/p$, while in every other one it retains order $N$. Therefore

$$
a_p(\Lambda,v+\Lambda)=
\begin{cases}
p+1,&p\nmid N,\\
p,&p\mid N.
\end{cases}
$$

This is the [Prime-index overlattices preserving a Gamma 1 level structure](../../../modular-function.md#prime-index-overlattices-preserving-a-gamma-1-level-structure) count.

## 4

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a full [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice) $\Lambda\subseteq\mathbb R^n$, its [dual lattice](../../../fourier-analysis.md#dual-lattice) is

$$
\Lambda^\vee=\{y:\langle x,y\rangle\in\mathbb Z\text{ for every }x\in\Lambda\}.
$$

For a Schwartz function, the [Poisson summation formula for a Euclidean lattice](../../../fourier-analysis.md#poisson-summation-formula-for-a-euclidean-lattice) states

$$
\sum_{\lambda\in\Lambda}f(\lambda)
=m(\Lambda)^{-1}\sum_{\mu\in\Lambda^\vee}\widehat f(\mu),
\qquad
\widehat f(y)=\int_{\mathbb R^n}f(x)e^{-2\pi i\langle x,y\rangle}\,dx.
$$

To prove it, periodize $f$ over $\Lambda$. The resulting function on $\mathbb R^n/\Lambda$ has Fourier coefficient $m(\Lambda)^{-1}\widehat f(\mu)$ at $\mu\in\Lambda^\vee$. Evaluating its absolutely convergent Fourier series at zero gives the identity. The same proof applies under the usual weaker hypotheses ensuring convergence of both sides.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Apply part a in $\mathbb R^2$ to

$$
f_k(x,y)=(x+iy)^ke^{-\pi(x^2+y^2)}.
$$

The supplied identity $\widehat f_k=(-i)^kf_k$ gives

$$
\sum_{\lambda\in\Lambda}\lambda^ke^{-\pi|\lambda|^2}
=(-i)^km(\Lambda)^{-1}
\sum_{\mu\in\Lambda^\vee}\mu^ke^{-\pi|\mu|^2}.
$$

In the notation of the [weighted Gaussian theta sum of a complex lattice](../../../modular-function.md#weighted-gaussian-theta-sum-of-a-complex-lattice), this is

$$
\boxed{\theta_k(\Lambda)=(-i)^km(\Lambda)^{-1}\theta_k(\Lambda^\vee).}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Put $L_\tau=y^{-1/2}(\mathbb Z\tau+\mathbb Z)$, a covolume-one lattice, and define

$$
\Theta_{k,\tau}(t)=
\sum_{0\ne z\in L_\tau}\overline z^{,k}e^{-\pi t|z|^2}.
$$

Termwise Mellin transformation in the initial half-plane gives

$$
G_k(\tau,s)=
\frac{\pi^{s+k}y^{-k/2}}{\Gamma(s+k)}
\int_0^\infty\Theta_{k,\tau}(t)t^{s+k-1}\,dt.
$$

Split the integral at $t=1$. The integral over $[1,\infty)$ is entire in $s$ because the theta sum decays exponentially. Apply the [Poisson summation formula for a Euclidean lattice](../../../fourier-analysis.md#poisson-summation-formula-for-a-euclidean-lattice) and the Fourier eigenfunction calculation from part b to the interval $(0,1]$, then substitute $t\mapsto1/t$. This rewrites the small-time integral as another exponentially convergent integral over $[1,\infty)$ plus explicit elementary Mellin terms. Those terms are meromorphic, but for positive even $k$ their apparent poles are canceled by the zeros of $1/\Gamma(s+k)$. The displayed formula therefore continues holomorphically to every $s\in\mathbb C$, proving the [analytic continuation of a weight-k real-analytic Eisenstein series](../../../modular-function.md#analytic-continuation-of-a-weight-k-real-analytic-eisenstein-series).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
