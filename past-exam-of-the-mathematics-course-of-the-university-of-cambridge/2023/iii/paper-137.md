# Paper 137

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_137.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_137.pdf)

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

## 1

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $\tau=x+iy\in\mathfrak h$. For

$$
\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma(1),
$$

the imaginary part of the [Möbius transformation](../../../group-theory.md#mobius-transformation) is

$$
\operatorname{Im}(\gamma\tau)=\frac{y}{|c\tau+d|^2}.
$$

Among the primitive integer pairs $(c,d)$, choose one minimizing the nonzero quantity $|c\tau+d|$. Such a minimum exists because only finitely many [lattice points](../../../quantum-mechanics.md#lattice-point) lie in a bounded region. Complete $(c,d)$ to a matrix $\gamma\in SL_2(\mathbb Z)$. Then $\gamma\tau$ has maximal imaginary part in its [modular group](../../../modular-function.md#modular-group) orbit.

Applying an integral translation does not change that imaginary part, so arrange

$$
-\frac12\leq\operatorname{Re}(\gamma\tau)\leq\frac12.
$$

If $\operatorname{Im}(\gamma\tau)<\sqrt3/2$, then $|\gamma\tau|<1$. The modular inversion $S:z\mapsto-1/z$ would give

$$
\operatorname{Im}(S\gamma\tau)
=\frac{\operatorname{Im}(\gamma\tau)}{|\gamma\tau|^2}
>\operatorname{Im}(\gamma\tau),
$$

contradicting maximality. Hence every orbit meets the stated region. This is the [reduction to the standard modular region](../../../modular-function.md#reduction-to-the-standard-modular-region) argument.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $\tau=x+iy$. The modular transformation law and

$$
\operatorname{Im}(\gamma\tau)=\frac{y}{|c\tau+d|^2}
$$

show that the [invariant norm of a modular form](../../../modular-function.md#invariant-norm-of-a-modular-form)

$$
y^{k/2}|f(\tau)|
$$

is invariant under $\Gamma(1)$. On the region from part (a), it is bounded: it is continuous on every truncated region, while the [cusp form](../../../modular-function.md#cusp-form) condition makes it tend to zero as $y\to\infty$. Thus

$$
|f(x+iy)|\leq C_0y^{-k/2}
$$

for all $x\in\mathbb R$ and $y>0$.

The [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) formula on one period gives

$$
a_n=e^{2\pi ny}\int_0^1f(x+iy)e^{-2\pi inx}\,dx,
$$

and hence

$$
|a_n|\leq C_0e^{2\pi ny}y^{-k/2}.
$$

Choosing $y=1/n$ yields

$$
|a_n|\leq C_0e^{2\pi}n^{k/2}.
$$

This proves the [Fourier coefficient bound for a cusp form](../../../modular-function.md#fourier-coefficient-bound-for-a-cusp-form).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Suppose for a contradiction that $b_0\ne0$. The [Eisenstein series](../../../modular-function.md#eisenstein-series) in the question has constant term $2\zeta(k)$, so

$$
h=g-\frac{b_0}{2\zeta(k)}G_k
$$

has zero constant term and is therefore a level-one [cusp form](../../../modular-function.md#cusp-form) of weight $k$. Part (b) gives the coefficient bound $[q^n]h=O(n^{k/2})$. Since $b_n=O(n^{k/2})$ as well, the displayed Fourier expansion of $G_k$ would imply

$$
\sigma_{k-1}(n)=O(n^{k/2}).
$$

Take $n=\ell$ through the [primes](../../../number-theory.md#prime-number). Then

$$
\sigma_{k-1}(\ell)=1+\ell^{k-1},
$$

which cannot be $O(\ell^{k/2})$ because $k-1>k/2$ for $k\geq4$. Therefore $b_0=0$, so $g$ vanishes at the only cusp of $\Gamma(1)$ and belongs to $S_k(\Gamma(1))$. This is the [Fourier coefficient growth criterion for a level-one cusp form](../../../modular-function.md#fourier-coefficient-growth-criterion-for-a-level-one-cusp-form).

## 2

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [modular function](../../../modular-function.md) of weight $k$ and level $\Gamma(1)$ is a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) $f:\mathfrak h\to\mathbb C$ satisfying

$$
f(\gamma\tau)=(c\tau+d)^k f(\tau)
$$

for every $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma(1)$, and having a meromorphic Fourier expansion at the cusp infinity. Equivalently, $f|_k\gamma=f$ for the [slash operator for modular forms](../../../modular-function.md#slash-operator-for-modular-forms).

A [modular form](../../../modular-function.md#modular-form) is a modular function that is [holomorphic](../../../complex-analysis.md#holomorphic-function) on $\mathfrak h$ and [holomorphic at infinity](../../../modular-function.md#holomorphic-at-a-cusp). Its Fourier expansion therefore has the form

$$
f(\tau)=\sum_{n\geq0}a_nq^n,
\qquad q=e^{2\pi i\tau}.
$$

Since $-I\in\Gamma(1)$, a nonzero level-one form must have even weight.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Extend the [slash operator for modular forms](../../../modular-function.md#slash-operator-for-modular-forms) to positive-determinant matrices by

$$
(f|_k\alpha)(\tau)
=\det(\alpha)^{k/2}(c\tau+d)^{-k}f(\alpha\tau).
$$

The [double coset](../../../group-theory.md#double-coset)

$$
\Gamma(1)\begin{pmatrix}p&0\\0&1\end{pmatrix}\Gamma(1)
$$

has left-coset representatives

$$
\begin{pmatrix}p&0\\0&1\end{pmatrix},
\qquad
\begin{pmatrix}1&b\\0&p\end{pmatrix}
\quad(0\leq b<p).
$$

Therefore the sum of the corresponding slashes, multiplied by $p^{k/2-1}$, is exactly

$$
T_p(f)(\tau)
=p^{k-1}f(p\tau)
+\frac1p\sum_{b=0}^{p-1}f\left(\frac{\tau+b}{p}\right).
$$

Right multiplication by an element of $\Gamma(1)$ permutes these left cosets. The cocycle law for the slash operator consequently gives

$$
T_p(f)|_k\gamma=T_p(f)
\qquad(\gamma\in\Gamma(1)),
$$

so $T_p(f)$ is a weight-$k$ level-one modular function. Each displayed summand is holomorphic on $\mathfrak h$, hence so is their finite sum. This is the [Hecke operator on modular forms](../../../modular-function.md#hecke-operator).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Because $f$ is a modular function that is holomorphic on $\mathfrak h$, it has a Laurent expansion

$$
f(\tau)=\sum_{n\geq-N}a_nq^n
$$

with a finite principal part at infinity. The [Hecke operator on modular forms](../../../modular-function.md#hecke-operator) acts on this expansion by

$$
T_pf=\sum_n\left(a_{pn}+p^{k-1}a_{n/p}\right)q^n.
$$

If $N>0$ and $a_{-N}\ne0$, the term $p^{k-1}f(p\tau)$ shows that $T_pf$ has pole order $pN$. Inductively, $T_p^rf$ has pole order $p^rN$ with nonzero leading coefficient. Functions with distinct pole orders are [linearly independent](../../../vector-space.md#linear-independence), so

$$
f,T_pf,T_p^2f,\ldots
$$

would span an infinite-dimensional vector space. This contradicts the hypothesis. Hence $N=0$, and $f$ is holomorphic at infinity. Together with its assumed holomorphy on $\mathfrak h$, this proves that $f$ is a modular form, as asserted by the [finite Hecke orbit criterion for holomorphy at a cusp](../../../modular-function.md#finite-hecke-orbit-criterion-for-holomorphy-at-a-cusp).

## 3

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The cusps are the $\Gamma_1(p)$-orbits of primitive columns $(a,c)^T$, with simultaneous negation representing the same point of $\mathbb P^1(\mathbb Q)$. For the [Gamma 1 congruence subgroup](../../../group-theory.md#gamma-1-congruence-subgroup), the standard primitive-vector classification separates the orbits according to $d=\gcd(c,p)$. For each divisor $d\mid p$, the two surviving unit coordinates give

$$
\frac12\varphi(d)\varphi(p/d)
$$

orbits when $p>2$. Hence an odd prime gives

$$
\#\bigl(\Gamma_1(p)\backslash\mathbb P^1(\mathbb Q)\bigr)
=\frac12\sum_{d\mid p}\varphi(d)\varphi(p/d)
=p-1.
$$

For $p=2$, simultaneous negation is already trivial modulo $2$, so the division by two does not apply. In that case $\Gamma_1(2)=\Gamma_0(2)$ has two cusps, represented by infinity and zero. Thus the [Number of cusps of Gamma 1 of prime level](../../../group-theory.md#number-of-cusps-of-gamma-1-of-prime-level) is

$$
\begin{cases}
2,&p=2,\\
p-1,&p\text{ odd}.
\end{cases}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Klein j-invariant](../../../modular-function.md#klein-j-invariant)

$$
j(\tau)=\frac{E_4(\tau)^3}{\Delta(\tau)}
$$

is a weight-zero modular function for $\Gamma(1)$, holomorphic on $\mathfrak h$ and meromorphic at infinity. Let

$$
\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_1(2).
$$

Since $c$ is even,

$$
\gamma'=\begin{pmatrix}a&2b\\c/2&d\end{pmatrix}\in\Gamma(1),
\qquad
2\gamma\tau=\gamma'(2\tau).
$$

The modular invariance of $j$ therefore gives

$$
\frac{j(\gamma\tau)}{j(2\gamma\tau)}
=\frac{j(\tau)}{j(2\tau)}.
$$

The quotient is meromorphic on $\mathfrak h$ and at the cusps, so it is a weight-zero modular function of level $\Gamma_1(2)$. This is the [Level-two modular ratio of Klein j-invariants](../../../modular-function.md#level-two-modular-ratio-of-klein-j-invariants).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The two cusps of $\Gamma_1(2)$ are infinity and zero. At infinity,

$$
j(\tau)=q^{-1}+744+O(q),
\qquad
j(2\tau)=q^{-2}+744+O(q^2),
$$

so

$$
f(\tau)=\frac{j(\tau)}{j(2\tau)}=q+O(q^2).
$$

Thus $f$ is holomorphic at infinity and has a simple zero there.

Use the scaling matrix

$$
S=\begin{pmatrix}0&-1\\1&0\end{pmatrix}
$$

at the cusp zero. Since $j(-1/\tau)=j(\tau)$,

$$
(f|_0S)(\tau)
=\frac{j(-1/\tau)}{j(-2/\tau)}
=\frac{j(\tau)}{j(\tau/2)}.
$$

The width of zero is two, so its local parameter is $q_0=e^{\pi i\tau}$. As $\operatorname{Im}\tau\to\infty$,

$$
j(\tau)=q_0^{-2}+O(1),
\qquad
j(\tau/2)=q_0^{-1}+O(1),
$$

and therefore

$$
(f|_0S)(\tau)=q_0^{-1}+O(1).
$$

It has a simple pole at zero and is not holomorphic there. This uses the [width of a cusp](../../../modular-function.md#width-of-a-cusp) to express the two expansions in their correct local parameters.

## 4

↑ **Parent:** [Paper 137](paper-137.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The left cosets $\Gamma_\infty\backslash\Gamma(1)$ correspond to primitive bottom rows $(c,d)\in\mathbb Z^2$, up to simultaneous sign. Put

$$
r=2\operatorname{Re}s+k.
$$

For $\tau=x+iy$, the identities

$$
\operatorname{Im}(\gamma\tau)=\frac{y}{|c\tau+d|^2},
\qquad
j(\gamma,\tau)=c\tau+d
$$

show that the absolute value of a summand is

$$
y^{\operatorname{Re}s}|c\tau+d|^{-r}.
$$

The hypothesis $\operatorname{Re}s>(2-k)/2$ says precisely that $r>2$.

If $\tau$ ranges over a compact subset $K\subset\mathfrak h$, the positive-definite quadratic form $|c\tau+d|^2$ has a uniform lower bound

$$
|c\tau+d|^2\geq C_K(c^2+d^2)
$$

for some $C_K>0$. The summands are therefore bounded uniformly on $K$ by a constant times

$$
(c^2+d^2)^{-r/2}.
$$

The corresponding two-dimensional [lattice sum](../../../real-analysis.md#lattice-sum) converges for $r>2$. The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) proves absolute and locally uniform convergence. This is the [absolute convergence of a weight-k real-analytic Eisenstein series](../../../modular-function.md#absolute-convergence-of-a-weight-k-real-analytic-eisenstein-series).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $\delta\in\Gamma(1)$, right multiplication by $\delta$ permutes $\Gamma_\infty\backslash\Gamma(1)$. The [automorphy factor](../../../modular-function.md#automorphy-factor) identity

$$
j(\gamma\delta,\tau)
=j(\gamma,\delta\tau)j(\delta,\tau)
$$

therefore gives

$$
E_{k,s}(\delta\tau)
=j(\delta,\tau)^kE_{k,s}(\tau).
$$

The [modular form](../../../modular-function.md#modular-form) $f$ obeys the same weight-$k$ transformation law, while

$$
\operatorname{Im}(\delta\tau)^k
=\frac{\operatorname{Im}(\tau)^k}{|j(\delta,\tau)|^{2k}}.
$$

Consequently

$$
\begin{aligned}
&f(\delta\tau)\overline{E_{k,s}(\delta\tau)}
\operatorname{Im}(\delta\tau)^k\\
&\quad=
j(\delta,\tau)^k\overline{j(\delta,\tau)}^k
|j(\delta,\tau)|^{-2k}
f(\tau)\overline{E_{k,s}(\tau)}\operatorname{Im}(\tau)^k\\
&\quad=
f(\tau)\overline{E_{k,s}(\tau)}\operatorname{Im}(\tau)^k.
\end{aligned}
$$

**Thus the product is invariant under the weight-zero action of $\Gamma(1)$, as described by the [invariant product with a weight-k real-analytic Eisenstein series](../../../modular-function.md#invariant-product-with-a-weight-k-real-analytic-eisenstein-series).**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
