# Paper 318

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_318.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_318.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 318](paper-318.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The trigonometric [Chebyshev alternation theorem](../../../uniform-approximation.md#equioscillation-theorem) says that $p_n^*\in\mathcal T_n$ is best exactly when its error has at least $2n+2$ cyclically ordered extrema of equal magnitude and alternating sign. Let $5^m\leq n<5^{m+1}$ and set $x_j=j\pi/5^{m+1}$. For every $k\geq m+1$,

$$
\cos(5^kx_j)=\cos(j\pi5^{k-m-1})=(-1)^j.
$$

Thus

$$
g(x_j)-\sum_{k=0}^mc_k\cos(5^kx_j)=(-1)^j\sum_{k=m+1}^\infty c_k.
$$

There are $2\cdot5^{m+1}\geq2n+2$ such extrema, while the [triangle inequality](../../../topological-analysis.md#triangle-inequality) bounds the tail by their common magnitude. Hence

$$
\boxed{p_n^*(x)=\sum_{k=0}^mc_k\cos(5^kx)},\qquad
\boxed{E_n(g)=\sum_{k=m+1}^\infty c_k}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [inverse theorem for trigonometric approximation](../../../uniform-approximation.md#inverse-theorem-for-trigonometric-approximation) gives

$$
\omega(f,n^{-1})\leq\frac Cn\sum_{\nu=0}^nE_\nu(f).
$$

Summing $\nu^{-\alpha}$ proves

$$
\boxed{\omega(f,n^{-1})=
\begin{cases}O(n^{-\alpha}),&0<\alpha<1,\\O(n^{-1}\log n),&\alpha=1.\end{cases}}
$$

For $c_k=a^{-k}$, part (a) gives $E_n(g)\asymp a^{-m}\asymp n^{-\log_5a}$. If $a<5$, an increment $h=\pi/5^{m+2}\leq1/n$ at $x=0$ has nonnegative summands and its $k=m+2$ term is $\asymp n^{-\log_5a}$. Part (c) handles $a=5$. Therefore

$$
\boxed{\omega(g,n^{-1})\asymp
\begin{cases}n^{-\log_5a},&1<a<5,\\n^{-1}\log n,&a=5.\end{cases}}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Since $5^k\equiv1\pmod4$,

$$
g\left(\frac\pi2+\frac1n\right)-g\left(\frac\pi2\right)
=-\sum_{k=0}^\infty5^{-k}\sin(5^k/n).
$$

Choose $5^m\leq n<5^{m+1}$. For $k\leq m$, $\sin(5^k/n)\geq c5^k/n$, so each of these $m+1$ same-sign terms has magnitude at least $c/n$. The remaining tail is $O(5^{-m})=O(n^{-1})$. Hence

$$
\boxed{\left|g\left(\frac\pi2+\frac1n\right)-g\left(\frac\pi2\right)\right|
\geq c\frac{\log n}{n}},\qquad
\boxed{\omega(g,n^{-1})\geq c\frac{\log n}{n}}.
$$

**Thus $E_n(f)=O(n^{-1})$ does not imply $\omega(f,n^{-1})=O(n^{-1})$; the logarithmic gap prevents a characterization of that approximation class by this first modulus alone.**

## 2

↑ **Parent:** [Paper 318](paper-318.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Substituting the [Fourier coefficient](../../../fourier-series.md#fourier-coefficient)s into the [Fourier partial sum](../../../fourier-series.md#fourier-partial-sum) and summing the finite geometric series gives

$$
s_n(f,x)=\frac1{2\pi}\int_{\mathbb T}f(t)\sum_{k=-n}^ne^{ik(x-t)}dt
=\frac1\pi\int_{\mathbb T}D_n(x-t)f(t)dt,
$$

where

$$
\boxed{D_n(u)=\frac{\sin((n+\tfrac12)u)}{2\sin(u/2)}}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Fejér kernel](../../../fourier-series.md#fejer-kernel) is nonnegative, and preservation of constants gives

$$
\boxed{\pi^{-1}\int_{\mathbb T}|F_n(t)|dt=1}.
$$

By evenness,

$$
\sigma_n(f,x)-f(x)=\frac1{2\pi}\int_{\mathbb T}F_n(t)[f(x-t)-2f(x)+f(x+t)]dt.
$$

Put $\delta=n^{-1/2}$. Use $\omega_2(f,|t|)\leq(|t|/\delta+1)^2\omega_2(f,\delta)$ together with $F_n(t)\leq n/2$ and $F_n(t)\leq C/(nt^2)$. Splitting at $1/n$ and $\delta$ shows that the remaining weighted integral is uniformly bounded, so

$$
\boxed{\lVert\sigma_n(f)-f\rVert_\infty\leq C\omega_2(f,n^{-1/2})}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Twice applying the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives

$$
f(x+h)-2f(x)+f(x-h)=\int_0^h\int_{-s}^{s}f''(x+u)\,du\,ds,
$$

hence $\boxed{\omega_2(f,t)\leq t^2\lVert f''\rVert_\infty}$. Part (b) gives $\lVert\sigma_n(f)-f\rVert_\infty=O(n^{-1})$. This cannot be little-$o$ for every $C^2$ function: for $f_0(x)=\cos x$,

$$
\sigma_n(f_0)=(1-n^{-1})\cos x,\qquad
\boxed{\lVert\sigma_n(f_0)-f_0\rVert_\infty=n^{-1}}.
$$

## 3

↑ **Parent:** [Paper 318](paper-318.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The explicit [divided difference](../../../numerical-analysis.md#divided-difference) formula makes $M_i(t)$ a finite linear combination of $(t_j-t)_+^{k-1}$. It is therefore polynomial of degree at most $k-1$ between knots and globally $C^{k-2}$. For $t<t_i$, the nodal data come from a polynomial of degree $k-1$, whose order-$k$ divided difference vanishes; for $t\geq t_{i+k}$ all truncated powers vanish. Thus

$$
\boxed{\operatorname{supp}M_i=[t_i,t_{i+k}]},
$$

and normalization does not change the degree, smoothness, knots, or support.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Apply the [Leibniz rule for divided differences](../../../numerical-analysis.md#leibniz-rule-for-divided-differences) to $(x-t)_+^{k-1}=(x-t)(x-t)_+^{k-2}$. Only the zeroth and first divided differences of the linear factor survive. After applying the normalization, this gives the [Cox-de Boor recursion formula](../../../uniform-approximation.md#cox-de-boor-recursion-formula)

$$
\boxed{N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)
+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t)}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Induct on $k$, using the recursive divided-difference formula. After substituting the two induction hypotheses, use

$$
f[t_1,\ldots,t_m]-f[t_0,\ldots,t_{m-1}]
=(t_m-t_0)f[t_0,\ldots,t_m]
$$

and the analogous identity for $g$; adjacent terms telescope. This proves

$$
\boxed{(fg)[t_0,\ldots,t_k]
=\sum_{m=0}^kf[t_0,\ldots,t_m]g[t_m,\ldots,t_k]}.
$$

## 4

↑ **Parent:** [Paper 318](paper-318.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem) states that positive linear operators $L_n:C[0,1]\to C[0,1]$ converge uniformly to the identity on every continuous function if they do so on the three test functions $1,t,t^2$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $e_m$ denote the $m$th [elementary symmetric polynomial](../../../polynomial.md#elementary-symmetric-polynomial) of $t_{i+1},\ldots,t_{i+k-1}$. Expanding both sides of the [Marsden identity](../../../uniform-approximation.md#marsden-identity) in powers of $x$ and equating the coefficient of $x^{k-1-m}$ gives

$$
\boxed{a_{m,i}=
\frac{e_m(t_{i+1},\ldots,t_{i+k-1})}{\binom{k-1}{m}}},
\qquad0\leq m\leq k-1.
$$

**Thus $a_{0,i}=1$, while $a_{1,i}$ and $a_{2,i}$ are respectively the means of the interior knots and of their pairwise products.**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [Schoenberg spline operator](../../../uniform-approximation.md#schoenberg-spline-operator) is positive and $V_n1=1$. If $\xi_i=a_{1,i}$, then both $\tau_i$ and $\xi_i$ lie in $[t_i,t_{i+k}]$, so

$$
\lVert V_nt-t\rVert_\infty\leq k|\Delta_n|\to0.
$$

Because $a_{2,i}$ averages products of knots in the same interval and all points lie in $[0,1]$,

$$
\lVert V_nt^2-t^2\rVert_\infty\leq2k|\Delta_n|\to0.
$$

The [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem) now proves

$$
\boxed{\lVert V_n(f)-f\rVert_{C[0,1]}\to0}
$$

for every $f\in C[0,1]$.

## 5

↑ **Parent:** [Paper 318](paper-318.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

An [orthonormal wavelet](../../../fourier-analysis.md#orthonormal-wavelet) is $\psi\in L^2(\mathbb R)$ such that $\{2^{j/2}\psi(2^jx-k)\}_{j,k\in\mathbb Z}$ is an orthonormal basis. A [multiresolution analysis](../../../fourier-analysis.md#multiresolution-analysis) is a nested family of closed spaces $V_j$ with trivial intersection, dense union, dyadic scaling, integer-translation invariance of $V_0$, and a generator $\phi$ whose integer translates form an orthonormal basis of $V_0$. The [Meyer-Mallat theorem](../../../fourier-analysis.md#meyer-mallat-theorem) says every such analysis has an orthonormal wavelet whose translates span $V_{j+1}\ominus V_j$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Fourier transforming the refinement equation and changing variables gives

$$
f(2t)=m(t)f(t),\qquad
\boxed{m(t)=\frac12\sum_na_ne^{-int}}.
$$

By [Parseval identity](../../../fourier-analysis.md#parseval-identity), orthonormality of the translates is equivalent to

$$
\frac1{2\pi}\int_{\mathbb R}|f(t)|^2e^{int}dt=\delta_{n0}.
$$

These are precisely the Fourier coefficients of the periodization $P(t)=\sum_k|f(t+2\pi k)|^2$. Therefore

$$
\boxed{\{\phi(\cdot-n)\}\text{ is orthonormal}\iff
\sum_k|f(t+2\pi k)|^2=1\ \text{a.e.}}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For $f=\mathbf1_{[-\pi,\pi)}$, its $2\pi$-periodization is one almost everywhere. The refinement mask is the periodic function equal to one on $[-\pi/2,\pi/2)$ and zero on the rest of $[-\pi,\pi)$. Fourier inversion gives the [Shannon scaling function](../../../fourier-analysis.md#shannon-scaling-function)

$$
\boxed{\phi(x)=\frac{\sin\pi x}{\pi x}}.
$$

Since $m(t)=\tfrac12\sum_na_ne^{-int}$, its Fourier coefficients give

$$
\boxed{a_0=1,\qquad a_n=\frac{2\sin(n\pi/2)}{\pi n}\quad(n\ne0)}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
