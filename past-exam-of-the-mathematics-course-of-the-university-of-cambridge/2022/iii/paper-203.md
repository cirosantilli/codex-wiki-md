# Paper 203

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_203.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_203.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded, relatively closed set $A\subset\mathbb H$ such that $\mathbb H\setminus A$ is simply connected. Its [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is the unique conformal bijection

$$
g_A:\mathbb H\setminus A\longrightarrow\mathbb H
$$

with hydrodynamic normalization

$$
g_A(z)=z+\frac{\operatorname{hcap}(A)}z+O(|z|^{-2})
\quad(z\to\infty).
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Uniqueness under [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity) gives

$$
g_{rA}(z)=r\,g_A(z/r)
$$

and

$$
g_{A+x}(z)=x+g_A(z-x).
$$

Indeed, each right-hand side maps the required complement conformally onto $\mathbb H$ and has expansion $z+O(1/z)$. This is the [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**False.** Here $\mathbb H\setminus S=\{z:\operatorname{Im}z>1\}$. If a normalized map $g_S$ existed, then

$$
h(w)=g_S(w+i)
$$

would be a conformal automorphism of $\mathbb H$. Hence

$$
h(w)=\frac{aw+b}{cw+d}
$$

with real coefficients and $ad-bc=1$. Hydrodynamic normalization forces $h(w)\to\infty$ linearly, so $c=0$ and $h(w)=\alpha w+\beta$ with $\alpha>0$ and $\beta\in\mathbb R$. But

$$
g_S(z)=\alpha(z-i)+\beta,
$$

and $g_S(z)-z\to0$ would require $\alpha=1$ and $\beta=i$, contradicting $\beta\in\mathbb R$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Suppose a subsequence had $\operatorname{Im}g_A(z_n)\geq\epsilon>0$. The images cannot tend to infinity, because the inverse mapping-out function satisfies $g_A^{-1}(w)=w+o(1)$ at infinity while $z_n$ remains bounded. A further subsequence therefore converges to some $w\in\mathbb H$. Continuity of $g_A^{-1}$ inside $\mathbb H$ would give

$$
z=g_A^{-1}(w)\in\mathbb H\setminus A,
$$

contradicting $z\in A$. Thus $\operatorname{Im}g_A(z_n)\to0$.

Convergence of the real parts can fail. For the vertical slit

$$
A=\{iy:0<y\leq1\},
\qquad
g_A(z)=\sqrt{z^2+1},
$$

the two sides of the slit at $z=iy$, $0<y<1$, map to the two boundary values $\pm\sqrt{1-y^2}$. Alternating sequences approaching $iy$ from the two sides make $g_A(z_n)$ alternate between neighborhoods of these distinct limits.

## 2

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $B$ be [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started at $z\in D$, let $\tau_D$ be its exit time, and let $\phi:D\to D'$ be conformal. Define

$$
C_s=\int_0^{s\wedge\tau_D}|\phi'(B_r)|^2\,dr,
\qquad
\sigma_t=\inf\{s:C_s>t\}.
$$

The [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) states that

$$
\widetilde B_t=\phi(B_{\sigma_t}),
\qquad 0\leq t<C_{\tau_D},
$$

is Brownian motion started at $\phi(z)$ and stopped when it exits $D'$. Thus conformal maps preserve Brownian paths after this random time-change.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

**No.** A conformal bijection is a homeomorphism and therefore induces an isomorphism of [fundamental groups](../../../algebraic-topology.md#fundamental-group). The simply connected domain $D$ has trivial fundamental group, whereas

$$
\pi_1(\mathbb C\setminus\{0\})\cong\mathbb Z.
$$

This contradiction rules out such a map.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

By conformal invariance, $g_A(B)$ after its quadratic-variation time-change is Brownian motion in $\mathbb H$, started at

$$
g_A(iy)=x_y+i v_y,
\qquad x_y\to0,\quad v_y/y\to1.
$$

Since $E\subset\mathbb R\setminus[-1,1]$ and $A\subset\overline{\mathbb D}$, the boundary correspondence is regular there, and the exit event maps to $g_A(E)$. The [Poisson kernel](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) of $\mathbb H$ therefore gives

$$
\mathbb P^{iy}(B_{\tau_A}\in E)
=\int_{g_A(E)}
\frac{v_y}{(u-x_y)^2+v_y^2}\,\frac{du}{\pi}.
$$

For bounded subsets, multiplication by $y$ makes the integrand converge uniformly to $1/\pi$. Approximation by increasing bounded subsets and [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) then gives

$$
\lim_{y\to\infty}
y\,\mathbb P^{iy}(B_{\tau_A}\in E)
=\frac{\operatorname{Leb}(g_A(E))}{\pi},
$$

with both sides allowed to be infinite.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $\tau_{\mathbb D}$ be the first hit of the closed unit disc. The conformal map $z\mapsto1/z$ sends its exterior to the punctured unit disc and sends $iy$ to $-i/y$. By conformal invariance, the hitting distribution on the unit circle is harmonic measure viewed from $-i/y$. As $y\to\infty$, this point tends to zero, where harmonic measure is normalized arc length by rotational invariance. Hence for every Borel $E\subset\partial\mathbb D$,

$$
\boxed{\lim_{y\to\infty}
\mathbb P^{iy}(B_{\tau_{\mathbb D}}\in E)
=\frac{\operatorname{length}(E)}{2\pi}.}
$$

## 3

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a continuous real driving function $U$, solve the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation)

$$
\partial_tg_t(z)=\frac2{g_t(z)-U_t},
\qquad g_0(z)=z,
$$

up to the first time $T_z$ at which $g_t(z)-U_t$ tends to zero. The generated hulls are

$$
K_t=\{z\in\mathbb H:T_z\leq t\}.
$$

They form an increasing [Loewner chain](../../../stochastic-process.md#loewner-chain) of compact H-hulls, satisfy $\operatorname{hcap}(K_t)=2t$, and $g_t$ is the mapping-out function of $K_t$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) says that, conditionally on $(K_s)_{s\leq t}$, the future hulls

$$
\widetilde K_s=(g_t-U_t)(K_{t+s}\setminus K_t)
$$

have the law of a fresh SLE in $(\mathbb H,0,\infty)$ and are independent of the past, with the usual interpretation of mapping out the old hull.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Under the Loewner correspondence, mapping out the past replaces the driver by

$$
\widetilde U_s=U_{t+s}-U_t.
$$

The conformal Markov property therefore makes $U$ a continuous process with stationary independent increments. Every such process has the form

$$
U_t=at+\sqrt\kappa B_t.
$$

Scale invariance of SLE says that $r^{-1}U_{r^2t}$ has the same law as $U_t$. Comparing means forces $ar=a$ for every $r>0$, hence $a=0$; comparison of variances leaves the constant $\kappa$. Nondegeneracy gives $\kappa>0$, so

$$
\boxed{U_t=\sqrt\kappa B_t.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For $t<T_x$, differentiate the Loewner equation with respect to $x$:

$$
\partial_tg_t'(x)
=-\frac{2g_t'(x)}{(g_t(x)-U_t)^2},
\qquad g_0'(x)=1.
$$

Therefore

$$
g_t'(x)=
\exp\left(-\int_0^t
\frac{2\,ds}{(g_s(x)-U_s)^2}\right).
$$

The exponent is nonpositive and decreases with $t$, so $0<g_t'(x)\leq1$ and $g_t'(x)$ is decreasing before $x$ is swallowed.

## 4

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The required set is

$$
\boxed{\Lambda=(4,\infty).}
$$

This is the boundary-intersection threshold in the [Phase classification of the SLE trace](../../../stochastic-process.md#phase-classification-of-the-sle-trace).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $x\in\mathbb R\setminus\{0\}$, the centered Loewner image

$$
Y_t=\frac{g_t(x)-U_t}{\sqrt\kappa}
$$

is the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle), a Bessel process of dimension

$$
d=1+\frac4\kappa.
$$

When $\kappa>4$, one has $d<2$, and the [Hitting-zero classification for a Bessel process](../../../brownian-motion.md#hitting-zero-classification-for-a-bessel-process) says that $Y$ hits zero almost surely. Thus every fixed nonzero boundary point is swallowed in finite time.

A hull generated by a continuous trace cannot swallow a real point while the trace remains strictly inside $\mathbb H$: before any contact with the real line, the trace is a crosscut-free interior curve and no boundary interval is disconnected from infinity. Consequently finite swallowing forces the trace to meet $\mathbb R$ away from its initial point. SLE therefore almost surely intersects the boundary for every $\kappa\in\Lambda$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Stop after a positive initial segment and map it out. By the [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle), the future is a fresh SLE in the remaining domain. Part b says that it hits that domain's boundary away from its current and terminal points. Choosing a bounded crosscut neighborhood whose real-boundary part is shielded from the future forces such a hit to occur on the image of the earlier trace with positive probability. Scale invariance and repeated conditional trials upgrade this to probability one. Thus the trace has self-intersections for $\kappa>4$, in agreement with the [Phase classification of the SLE trace](../../../stochastic-process.md#phase-classification-of-the-sle-trace).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

**False.** The displayed probability is zero. Let $\tau$ be the first exit from the fixed domain $\mathbb D$ and choose $x_n>0$ tending to zero. The Bessel scaling in part b gives

$$
T_{x_n}\overset d=x_n^2T_1.
$$

Hence $T_{x_n}\to0$ in probability, while continuity of the trace gives $\tau>0$ almost surely. Therefore

$$
\mathbb P(T_{x_n}<\tau)\longrightarrow1.
$$

Swallowing $x_n$ before leaving $\mathbb D$ forces a boundary contact away from zero before $\tau$. Taking the limit shows that such a contact occurs almost surely, so

$$
\boxed{\mathbb P\bigl(\eta([0,\tau])\cap\mathbb R=\{0\}\bigr)=0.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
