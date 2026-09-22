# Paper 62

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper62.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper62.pdf)

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
- [5](#5)
  - [1](#5/1)
    - [Solution](#5/1/solution)
  - [2](#5/2)
    - [Solution](#5/2/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Bernstein polynomial](../../../functional-analysis.md#bernstein-polynomial) is

$$
B_n(f,x)=\sum_{j=0}^n f(j/n)\binom nj x^j(1-x)^{n-j}.
$$

It has degree at most $n$, since cancellation can lower the degree. For $0\le x\le1$, the [Bernstein basis](../../../functional-analysis.md#bernstein-basis) weights are nonnegative and their sum is $(x+(1-x))^n=1$ by the [binomial theorem](../../../combinatorics.md#binomial-theorem). Consequently

$$
|B_n(f,x)|\le\sum_{j=0}^n |f(j/n)|\binom nj x^j(1-x)^{n-j}\le\|f\|_\infty.
$$

Thus the [Bernstein polynomial](../../../functional-analysis.md#bernstein-polynomial) defines a [positive linear operator on continuous functions](../../../topological-vector-space.md#positive-linear-operator-on-continuous-functions) satisfying **$\|B_n f\|_\infty\le\|f\|_\infty$**. Since $B_n1=1$, its [operator norm](../../../continuous-dual-space.md#operator-norm) in the [supremum norm](../../../functional-analysis.md#supremum-norm) is exactly one.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $j^{\underline m}=j(j-1)\cdots(j-m+1)$ for the [falling factorial](../../../combinatorics.md#falling-factorial). At the sampling points, $f_{nm}(j/n)=n^{-m}j^{\underline m}$, which vanishes for $j<m$. For $j\ge m$, cancellation of the factorials gives

$$
j^{\underline m}\binom nj=\frac{n!}{(n-m)!}\binom{n-m}{j-m}=n^{\underline m}\binom{n-m}{j-m}.
$$

Insert this into the [Bernstein polynomial](../../../functional-analysis.md#bernstein-polynomial) and set $\ell=j-m$:

$$
\begin{aligned}
B_n(f_{nm},x)&=\frac{n^{\underline m}}{n^m}x^m\sum_{\ell=0}^{n-m}\binom{n-m}{\ell}x^\ell(1-x)^{n-m-\ell}\\
&=\frac{n^{\underline m}}{n^m}x^m=f_{nm}(1)x^m.
\end{aligned}
$$

The [binomial theorem](../../../combinatorics.md#binomial-theorem) evaluates the remaining sum. For $m=0$, both sides equal one. This proves the **[Bernstein falling-factorial identity](../../../functional-analysis.md#bernstein-falling-factorial-identity) $B_n(f_{nm},x)=f_{nm}(1)x^m$**.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix $m$ and take $n\ge m$. On $[0,1]$, every factor $x-r/n$ and every factor $x$ has absolute value at most one. Replacing the factors successively and applying the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\|f_{nm}-x^m\|_\infty\le\sum_{r=0}^{m-1}\frac rn=\frac{m(m-1)}{2n},\qquad |f_{nm}(1)-1|\le\frac{m(m-1)}{2n}.
$$

Using the [supremum norm](../../../functional-analysis.md#supremum-norm) contraction in (a) and the [Bernstein falling-factorial identity](../../../functional-analysis.md#bernstein-falling-factorial-identity) in (b),

$$
\begin{aligned}
\|B_n(x^m)-x^m\|_\infty
&\le\|B_n(x^m-f_{nm})\|_\infty+\|B_n(f_{nm})-x^m\|_\infty\\
&\le\|x^m-f_{nm}\|_\infty+|f_{nm}(1)-1|\le\frac{m(m-1)}n.
\end{aligned}
$$

For $m=0,1$, the [monomials](../../../polynomial.md#monomial) are reproduced exactly. For every fixed $m$, **$B_n(x^m)\to x^m$ uniformly on $[0,1]$**.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem) states that the [polynomials](../../../polynomial.md) are a [dense subspace](../../../topological-vector-space.md#dense-subspace) of $C[0,1]$ in the [supremum norm](../../../functional-analysis.md#supremum-norm). By [linearity](../../../vector-space.md#linearity) and (c), $B_np\to p$ uniformly for every [polynomial](../../../polynomial.md) $p$. Given $f\in C[0,1]$ and $\varepsilon>0$, choose a [polynomial](../../../polynomial.md) $p$ with $\|f-p\|_\infty<\varepsilon$. The [operator norm](../../../continuous-dual-space.md#operator-norm) estimate in (a) gives

$$
\|B_nf-f\|_\infty\le\|B_n(f-p)\|_\infty+\|B_np-p\|_\infty+\|p-f\|_\infty\le2\varepsilon+\|B_np-p\|_\infty.
$$

First let $n\to\infty$, then $\varepsilon\downarrow0$. Hence **$\|B_nf-f\|_\infty\to0$ for every continuous $f$**. This is an instance of [extension of approximation operators from a dense subspace](../../../uniform-approximation.md#extension-of-approximation-operators-from-a-dense-subspace).

## 2

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the centered [second modulus of smoothness](../../../uniform-approximation.md#second-modulus-of-smoothness)

$$
\omega_2(f,\delta)=\sup_{|h|\le\delta}\|f(\cdot+h)-2f+f(\cdot-h)\|_\infty.
$$

The relevant modulus properties are $\omega_2(f,t)\le(1+t/\delta)^2\omega_2(f,\delta)$ for $t\ge0$, $\delta>0$, and $\omega_2(f,\delta)\le\delta^2\|f''\|_\infty$ when $f''$ is continuous. The latter follows from the [second-difference integral formula](../../../uniform-approximation.md#second-difference-integral-formula)

$$
f(x+h)-2f(x)+f(x-h)=\int_{-|h|}^{|h|}(|h|-|u|)f''(x+u)\,du.
$$

The [Fejér kernel](../../../fourier-series.md#fejer-kernel) is even, nonnegative and has integral one. Averaging the convolution at $t$ and $-t$ therefore gives

$$
\sigma_nf(x)-f(x)=\frac12\int_{-\pi}^{\pi}F_n(t)\bigl(f(x+t)-2f(x)+f(x-t)\bigr)\,dt.
$$

Apply the [second modulus of smoothness](../../../uniform-approximation.md#second-modulus-of-smoothness) bound and $(1+s)^2\le2(1+s^2)$:

$$
\|\sigma_nf-f\|_\infty\le\omega_2(f,\delta)\left(1+\delta^{-2}\int_{-\pi}^{\pi}t^2F_n(t)\,dt\right).
$$

For $|t|\le\pi$, $\sin(|t|/2)\ge|t|/\pi$, while $\sin^2(nt/2)\le1$. Thus

$$
t^2F_n(t)\le\frac{\pi}{2n},\qquad \int_{-\pi}^{\pi}t^2F_n(t)\,dt\le\frac{\pi^2}{n}.
$$

The removable value at $t=0$ causes no problem. With $\delta=n^{-1/2}$, the [Fejér second-modulus approximation bound](../../../fourier-series.md#fejer-second-modulus-approximation-bound) is

$$
\boxed{\|\sigma_nf-f\|_\infty\le(1+\pi^2)\omega_2(f,n^{-1/2}).}
$$

If $f''$ is continuous, this also yields **$\|\sigma_nf-f\|_\infty\le(1+\pi^2)\|f''\|_\infty/n=O(n^{-1})$**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Squaring the finite geometric sum in the [Fejér kernel](../../../fourier-series.md#fejer-kernel) gives its [Fourier series](../../../fourier-series.md)

$$
F_n(t)=\frac1{2\pi n}\left|\sum_{j=0}^{n-1}e^{ijt}\right|^2=\frac1{2\pi}\sum_{|r|<n}\left(1-\frac{|r|}{n}\right)e^{irt}.
$$

For a fixed positive integer $k$ and $n>k$, convolution therefore gives $\sigma_n(e^{ikx})=(1-k/n)e^{ikx}$. Taking the real part,

$$
\boxed{\|\sigma_n(\cos kx)-\cos kx\|_\infty=\frac{k}{n}.}
$$

The ratio to $1/n$ is the nonzero constant $k$, even though the function is infinitely differentiable. This [Fejér saturation on a Fourier mode](../../../fourier-series.md#fejer-saturation-on-a-fourier-mode) disproves an $o(n^{-1})$ estimate for all $C^2$ periodic functions.

## 3

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $x=\cos\theta$ with $0<\theta<\pi$, differentiation of the [Chebyshev polynomial](../../../numerical-analysis.md#chebyshev-polynomial) gives

$$
T_n'(\cos\theta)=n\frac{\sin(n\theta)}{\sin\theta},\qquad \frac{1-x^2}{n^2}T_n'(x)^2=\sin^2(n\theta)=1-T_n(x)^2.
$$

Both sides are [polynomials](../../../polynomial.md) in $x$, so the identity holds at the endpoints and, in fact, for every real $x$.

Order the [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) here as $x_j=\cos\theta_j$, $\theta_j=(2j-1)\pi/(2n)$, so $x_1>\cdots>x_n$. At these simple roots,

$$
T_n'(x_j)=\frac{n(-1)^{j-1}}{\sin\theta_j},\qquad |T_n'(x_j)|=\frac{n}{\sqrt{1-x_j^2}}.
$$

For a [polynomial](../../../polynomial.md) $q$ of degree at most $n-1$, the [Lagrange interpolation polynomial](../../../numerical-analysis.md#lagrange-polynomial) is

$$
q(x)=\sum_{j=1}^n q(x_j)\ell_j(x),\qquad \ell_j(x)=\frac{T_n(x)}{(x-x_j)T_n'(x_j)}.
$$

For $x>x_1$, the [Chebyshev polynomial](../../../numerical-analysis.md#chebyshev-polynomial) is positive: all its roots are at most $x_1$ and its leading coefficient is positive. Hence $\ell_j(x)T_n'(x_j)=T_n(x)/(x-x_j)>0$. The assumed nodal bounds and interpolation of the degree-$n-1$ [polynomial](../../../polynomial.md) $T_n'$ now give

$$
|q(x)|\le\sum_j|\ell_j(x)|\,|T_n'(x_j)|=\sum_j\ell_j(x)T_n'(x_j)=T_n'(x).
$$

Continuity includes $x=x_1$. Apply this argument to $q(-x)$ and use the parity of the [Chebyshev polynomial](../../../numerical-analysis.md#chebyshev-polynomial) to obtain the negative side. Thus the [Chebyshev nodal derivative comparison](../../../numerical-analysis.md#chebyshev-nodal-derivative-comparison) proves

$$
\boxed{|q(x)|\le|T_n'(x)|\quad\text{when }|x|\ge\cos(\pi/(2n)).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assume $n\ge1$ and $\|p\|_{[-1,1]}\le1$. The given [Bernstein inequality for algebraic polynomials](../../../uniform-approximation.md#bernstein-inequality-for-algebraic-polynomials) shows that $q=p'$ satisfies the nodal hypotheses of (a). Consequently, in the two endpoint regions $\cos(\pi/(2n))\le|x|\le1$, $|p'(x)|\le|T_n'(x)|$.

For $0<\theta<\pi$, the finite geometric identity

$$
\frac{\sin(n\theta)}{\sin\theta}=\sum_{r=0}^{n-1}e^{i(n-1-2r)\theta}
$$

bounds its absolute value by $n$. It follows that $|T_n'(\cos\theta)|\le n^2$, and the endpoint limit gives $T_n'(1)=n^2$. In the central interval, the [Bernstein inequality for algebraic polynomials](../../../uniform-approximation.md#bernstein-inequality-for-algebraic-polynomials) gives

$$
|p'(x)|\le\frac{n}{\sqrt{1-x^2}}\le\frac{n}{\sin(\pi/(2n))}\le n^2,
$$

since $\sin t\ge2t/\pi$ on $[0,\pi/2]$. Combining the regions and rescaling proves the [Markov inequality for polynomial derivatives](../../../uniform-approximation.md#markov-inequality-for-polynomial-derivatives):

$$
\boxed{\|p'\|_{[-1,1]}\le n^2\|p\|_{[-1,1]},\qquad T_n'(1)=n^2.}
$$

The [Chebyshev polynomial](../../../numerical-analysis.md#chebyshev-polynomial) itself attains equality, so this constant is sharp. Constant [polynomials](../../../polynomial.md) have zero [derivative](../../../calculus.md#derivative).

## 4

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put $s_j=t_{i+j}$ for $0\le j\le k$, with the knots in increasing order. The explicit formula for a [divided difference](../../../numerical-analysis.md#divided-difference) at distinct nodes gives

$$
M_i(t)=k\sum_{j=0}^k\frac{(s_j-t)_+^{k-1}}{\prod_{\ell\ne j}(s_j-s_\ell)}.
$$

Each [truncated power function](../../../polynomial.md#truncated-power-function) is a [piecewise polynomial function](../../../polynomial.md#piecewise-polynomial-function) of degree $k-1$ and is $C^{k-2}$ for $k\ge2$. Therefore their sum has the same global smoothness. The jump in the $(k-1)$st [derivative](../../../calculus.md#derivative) at $s_j$ equals

$$
\frac{k(-1)^k(k-1)!}{\prod_{\ell\ne j}(s_j-s_\ell)},
$$

which is nonzero. Thus each $s_j$ really is a knot, and generally there is no additional smoothness.

If $t<s_0$, the values being differenced are the values of the degree-$k-1$ [polynomial](../../../polynomial.md) $(s-t)^{k-1}$, so their $k$th [divided difference](../../../numerical-analysis.md#divided-difference) vanishes. If $t>s_k$, every sampled [truncated power function](../../../polynomial.md#truncated-power-function) is zero. To check that both support endpoints occur, for $s_0<t<s_1$ subtract the vanished full [polynomial](../../../polynomial.md) divided difference to obtain

$$
M_i(t)=\frac{k(t-s_0)^{k-1}}{\prod_{\ell=1}^k(s_\ell-s_0)}>0.
$$

For $s_{k-1}<t<s_k$, only the last term survives and is positive. The nonnegativity from the recurrence in (b) actually gives positivity throughout the interior: for each $s_0<t<s_k$, at least one lower-order [B-spline](../../../uniform-approximation.md#b-spline) covering $t$ has a positive recurrence coefficient, and induction starts with positive order-one indicators. Hence **$\operatorname{supp}M_i=[t_i,t_{i+k}]$ and $M_i\in C^{k-2}$ for $k\ge2$**, with degree $k-1$ on its knot intervals. For $k=1$, the [B-spline](../../../uniform-approximation.md#b-spline) is the step function $1_{[s_0,s_1)}(t)/(s_1-s_0)$, so no continuity is asserted.

The [unit-integral normalization of a B-spline](../../../uniform-approximation.md#unit-integral-normalization-of-a-b-spline) also follows directly: integrating $k(s_j-t)_+^{k-1}$ over $s_0\le t\le s_k$ gives $(s_j-s_0)^k$. The $k$th [divided difference](../../../numerical-analysis.md#divided-difference) of this monic degree-$k$ [polynomial](../../../polynomial.md) is one. Thus $\int M_i(t)\,dt=1$, explaining its normalization.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use $s_j=t_{i+j}$ again and take $k\ge2$. Set $g(s)=(s-t)_+^{k-2}$, so $(s-t)g(s)=(s-t)_+^{k-1}$. Let

$$
H=[s_0,\ldots,s_{k-1}]g,\qquad K=[s_1,\ldots,s_k]g,\qquad G=[s_0,\ldots,s_k]g=\frac{K-H}{s_k-s_0}.
$$

The [Leibniz rule for divided differences](../../../numerical-analysis.md#leibniz-rule-for-divided-differences), applied to the linear factor $s-t$, reads

$$
[s_0,\ldots,s_k]\bigl((s-t)g(s)\bigr)=(s_0-t)G+K.
$$

Multiply by $s_k-s_0$ and substitute $G$ to get $(t-s_0)H+(s_k-t)K$. Converting $H$ and $K$ to the lower-order normalized [B-splines](../../../uniform-approximation.md#b-spline) proves the [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula):

$$
\boxed{N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t).}
$$

It starts with $N_{i,1}=1_{[t_i,t_{i+1})}$. The coefficients are nonnegative wherever the corresponding lower-order [B-spline](../../../uniform-approximation.md#b-spline) is nonzero, so induction proves nonnegativity.

For later use, extend the finite knot sequence to a strictly increasing sequence in both directions. The full order-one sum is one. When the [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula) is summed, the two coefficients of each fixed lower-order [B-spline](../../../uniform-approximation.md#b-spline) add to one. Induction therefore gives a full partition of unity. Removing terms proves the [subpartition of unity for B-splines](../../../uniform-approximation.md#subpartition-of-unity-for-b-splines), $\sum_{i=1}^nN_{i,k}(t)\le1$. For repeated knots, the same statement follows by a limit of strictly increasing knot sequences, with the usual convention that a recurrence term with zero denominator is zero; the bound holds on each open knot interval and for the standard one-sided endpoint values. The terminology “$L_\infty$-normalized” refers to this standard basis normalization; it does not claim that each individual [B-spline](../../../uniform-approximation.md#b-spline) has [supremum norm](../../../functional-analysis.md#supremum-norm) exactly one.

## 5

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="5/1">1</h3>

↑ **Parent:** [5](#5)

<h4 id="5/1/solution">Solution</h4>

↑ **Parent:** [1](#5/1)

For the usual [spline interpolation](../../../uniform-approximation.md#spline-interpolation) problem the sites are distinct and ordered; the [Schoenberg–Whitney theorem](../../../uniform-approximation.md#schoenberg-whitney-theorem) then makes $A_x$ invertible under the stated support positivity. More generally, the following argument applies whenever the interpolation map in the question is well defined and $A_x$ is invertible.

Factor the [spline interpolation operator](../../../uniform-approximation.md#spline-interpolation-operator) as $P_x=BA_x^{-1}R$, where

$$
Rf=(f(x_1),\ldots,f(x_n)),\qquad Bc=\sum_{j=1}^nc_jN_j.
$$

Sampling has [operator norm](../../../continuous-dual-space.md#operator-norm) at most one from the [supremum norm](../../../functional-analysis.md#supremum-norm) to $\ell_\infty$. Nonnegativity and the [subpartition of unity for B-splines](../../../uniform-approximation.md#subpartition-of-unity-for-b-splines) give

$$
|Bc(t)|\le\|c\|_{\ell_\infty}\sum_jN_j(t)\le\|c\|_{\ell_\infty}.
$$

Consequently $\|P_x\|\le\|A_x^{-1}\|_{\ell_\infty}$.

For the reverse bound, select a row $r$ of $A_x^{-1}$ with maximal absolute row sum, and choose $y_j=\operatorname{sgn}((A_x^{-1})_{rj})$, assigning any value of modulus at most one when the entry is zero. Then $\|y\|_{\ell_\infty}=1$ and

$$
\|A_x^{-1}y\|_{\ell_\infty}=\sum_j|(A_x^{-1})_{rj}|=\|A_x^{-1}\|_{\ell_\infty}.
$$

At distinct sites there is a continuous [piecewise linear function](../../../function.md#piecewise-linear-function) $f$ with $f(x_j)=y_j$ and $\|f\|_\infty=1$: interpolate linearly between the ordered sites and extend constantly to the endpoints. The given [uniform-norm stability of a B-spline basis](../../../uniform-approximation.md#uniform-norm-stability-of-a-b-spline-basis) therefore implies

$$
\|P_xf\|_\infty=\|BA_x^{-1}y\|_\infty\ge\frac1{d_k}\|A_x^{-1}y\|_{\ell_\infty}.
$$

Thus the [B-spline interpolation operator norm](../../../uniform-approximation.md#b-spline-interpolation-operator-norm) satisfies

$$
\boxed{\frac1{d_k}\|A_x^{-1}\|_{\ell_\infty}\le\|P_x\|\le\|A_x^{-1}\|_{\ell_\infty}.}
$$

Positivity $N_i(x_i)>0$ alone, without the usual distinct-site convention, is insufficient to define an interpolation operator. For example, take order-two [B-splines](../../../uniform-approximation.md#b-spline) with knots $0,1,2,3$ and $x_1=x_2=3/2$. Both diagonal values are $1/2$, but the [B-spline collocation matrix](../../../uniform-approximation.md#b-spline-collocation-matrix) has identical rows $(1/2,1/2)$ and is singular. The displayed proof uses the well-defined interpolation map posited in the question; ordered distinct sites supply its standard existence guarantee.

<h3 id="5/2">2</h3>

↑ **Parent:** [5](#5)

<h4 id="5/2/solution">Solution</h4>

↑ **Parent:** [2](#5/2)

For unit-spaced knots, the [quadratic cardinal B-spline](../../../uniform-approximation.md#quadratic-cardinal-b-spline) with support $[i,i+3]$ is $N_i(t)=B(t-i)$, where the [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula) gives

$$
B(u)=\begin{cases}u^2/2,&0\le u\le1,\\-u^2+3u-3/2,&1\le u\le2,\\(3-u)^2/2,&2\le u\le3,\\0,&\text{otherwise}.\end{cases}
$$

In particular $B(1)=B(2)=1/2$ and $B(0)=B(3)=0$. At $x_i=i+2$, the only nonzero entries in row $i$ are $A_{ii}=1/2$ and, if $i<n$, $A_{i,i+1}=1/2$. Write $U$ for the upper shift matrix, with ones immediately above its diagonal. Then

$$
A_x=\tfrac12(I+U),\qquad A_x^{-1}=2\sum_{r=0}^{n-1}(-U)^r,
$$

since $U^n=0$. Thus $(A_x^{-1})_{ij}=2(-1)^{j-i}$ for $j\ge i$, and zero otherwise. The largest absolute row sum is the first, giving $\|A_x^{-1}\|_{\ell_\infty}=2n$.

Using (1) and the permitted $d_3=3$ proves the stronger [linear growth of shifted quadratic spline interpolation](../../../uniform-approximation.md#linear-growth-of-shifted-quadratic-spline-interpolation) estimate

$$
\boxed{\frac{2n}{3}\le\|P_x\|\le2n.}
$$

Therefore **$\|P_x\|=\Theta(n)$ and is not uniformly bounded**. An $O(n)$ upper bound alone would not imply unboundedness; the lower bound is essential.

## 6

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

An orthonormal [multiresolution analysis](../../../fourier-analysis.md#multiresolution-analysis) consists of closed subspaces $V_j\subset L_2(\mathbb R)$, $j\in\mathbb Z$, with $V_j\subset V_{j+1}$, $\overline{\bigcup_jV_j}=L_2(\mathbb R)$, $\bigcap_jV_j=\{0\}$, and the dilation equivalence $h\in V_j\iff h(2\cdot)\in V_{j+1}$. A [scaling function](../../../fourier-analysis.md#scaling-function) $\phi$ has integer translates forming an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_0$. Hence

$$
\phi_{j,k}(x)=2^{j/2}\phi(2^jx-k),\qquad k\in\mathbb Z,
$$

is an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_j$. Set $W_j=V_{j+1}\ominus V_j$, the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of $V_j$ inside $V_{j+1}$. A function $\psi$ whose integer translates form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $W_0$ produces a complete [orthonormal wavelet](../../../fourier-analysis.md#orthonormal-wavelet) system $\{2^{j/2}\psi(2^j\cdot-k):j,k\in\mathbb Z\}$: different $W_j$ are orthogonal, their sum contains every difference $V_b\ominus V_a$, and density together with the zero intersection exhausts $L_2(\mathbb R)$.

Here is the filter construction that guarantees such a [wavelet](../../../fourier-analysis.md#wavelet). Nesting puts $\phi$ in $V_1$, so expansion in its [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) gives the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation) $\phi=\sum_na_n\phi(2\cdot-n)$, with $a\in\ell_2$. Define the [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) and its complementary [quadrature mirror filter](../../../fourier-analysis.md#quadrature-mirror-filter) by

$$
m(t)=\tfrac12\sum_na_ne^{-int},\qquad q(t)=-e^{-it}\overline{m(t+\pi)}.
$$

Splitting the [orthonormal translates and Fourier periodization](../../../fourier-analysis.md#orthonormal-translates-and-fourier-periodization) identity at $2t$, as in part (b), gives $|m(t)|^2+|m(t+\pi)|^2=1$ almost everywhere. Consequently the rows of

$$
\begin{pmatrix}m(t)&m(t+\pi)\\-e^{-it}\overline{m(t+\pi)}&e^{-it}\overline{m(t)}\end{pmatrix}
$$

have length one and are orthogonal; the matrix is unitary. Put $b_n=(-1)^n\overline{a_{1-n}}$ and $\psi=\sum_nb_n\phi(2\cdot-n)$, so $q(t)=\tfrac12\sum_nb_ne^{-int}$.

To see completeness as well as orthogonality, identify $V_1$ with its fine-scale coefficient sequences and take their [Fourier series](../../../fourier-series.md). Group the frequencies $t$ and $t+\pi$ over a half-period. The two rows of the displayed matrix are the normalized coarse and complementary channels; their unitarity is exactly an onto isometry from these two channels to the fine-scale coefficient space. Translates of $\phi$ and $\psi$ correspond to the [Fourier basis](../../../fourier-series.md#fourier-basis) in the respective channels. They therefore jointly form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_1$. The [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) channel gives the [wavelet completion of a multiresolution filter](../../../fourier-analysis.md#wavelet-completion-of-a-multiresolution-filter), namely the integer translates of $\psi$ span $W_0$. This proves the asserted relation with an [orthonormal wavelet](../../../fourier-analysis.md#orthonormal-wavelet).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Use the [Fourier transform](../../../analysis.md#fourier-transform) convention $f(t)=\widehat\phi(t)=\int\phi(x)e^{-ixt}\,dx$ and the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) normalization $\|\phi\|_2^2=(2\pi)^{-1}\|f\|_2^2$. For a general $L_2$ [scaling function](../../../fourier-analysis.md#scaling-function), the transform means its $L_2$ extension; an ordinary absolutely convergent integral is not required.

A change of variables gives $\widehat{\phi(2\cdot-n)}(t)=\tfrac12e^{-int/2}f(t/2)$. Thus the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation) transforms to $f(t)=m(t/2)f(t/2)$, or **$f(2t)=m(t)f(t)$**, with the $2\pi$-periodic [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) $m(t)=\tfrac12\sum_na_ne^{-int}$. The periodicity is necessary; allowing an arbitrary quotient $f(2t)/f(t)$ would not express refinement by integer translates.

For orthonormality, let $P(t)=\sum_{k\in\mathbb Z}|f(t+2\pi k)|^2$. This is a $2\pi$-periodic $L_1$ function, since $f\in L_2$. The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) gives

$$
\langle\phi(\cdot-j),\phi(\cdot-\ell)\rangle=\frac1{2\pi}\int_{\mathbb R}|f(t)|^2e^{i(\ell-j)t}\,dt=\frac1{2\pi}\int_0^{2\pi}P(t)e^{i(\ell-j)t}\,dt.
$$

These inner products equal $\delta_{j\ell}$ precisely when the [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) of $P$ agree with those of one. The [uniqueness of Fourier coefficients in L1](../../../fourier-series.md#uniqueness-of-fourier-coefficients-in-l1) proves the equivalence

$$
\boxed{\{\phi(\cdot-n)\}\text{ orthonormal}\quad\Longleftrightarrow\quad\sum_k|f(t+2\pi k)|^2=1\ \text{a.e.}}
$$

For completeness, the converse refinement implication is also valid with the natural $L_2$ series interpretation. Suppose this periodization identity and $f(2t)=m(t)f(t)$ hold for a measurable $2\pi$-periodic $m$. Splitting the periodization at $2t$ into even and odd translates gives

$$
\begin{aligned}
1&=\sum_k|f(2t+2\pi k)|^2\\
&=|m(t)|^2\sum_r|f(t+2\pi r)|^2+|m(t+\pi)|^2\sum_r|f(t+\pi+2\pi r)|^2\\
&=|m(t)|^2+|m(t+\pi)|^2.
\end{aligned}
$$

Hence $m$ is bounded and belongs to $L_2$ of a period. Write $m=\tfrac12\sum_na_ne^{-int}$ in $L_2$ and let $m_N$ denote the symmetric partial sums. Since $P=1$,

$$
\int_{\mathbb R}|(m_N(t)-m(t))f(t)|^2\,dt=\int_0^{2\pi}|m_N(t)-m(t)|^2P(t)\,dt\longrightarrow0.
$$

After substituting $t/2$, this proves convergence of the transformed refinement sums to $f$ in $L_2$. Inverting the [Fourier transform](../../../analysis.md#fourier-transform) proves $\phi=\sum_na_n\phi(2\cdot-n)$ in $L_2$. Thus **the two spatial conditions and the two Fourier conditions are equivalent**, with the periodic mask and convergence conventions made explicit.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

First use the usual real-valued, measurable interpretation of the transition data. The complementary squares then imply $|f|\le1$, and the compact support gives $f\in L_2$. Consider the periodization on $[-\pi,\pi]$. For $|t|<2\pi/3$, only $f(t)=1$ contributes. For $2\pi/3\le t\le\pi$, only $f(t)$ and $f(t-2\pi)$ can contribute, and their squares sum to one. For $-\pi\le t\le-2\pi/3$, apply the complementary identity at $t+2\pi$ to obtain $f(t)^2+f(t+2\pi)^2=1$. Therefore the [orthonormal translates and Fourier periodization](../../../fourier-analysis.md#orthonormal-translates-and-fourier-periodization) identity holds almost everywhere.

Define a periodic [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) by prescribing it on $[-\pi,\pi]$:

$$
m(t)=\begin{cases}f(2t),&|t|<2\pi/3,\\0,&2\pi/3\le|t|\le\pi,\end{cases}\qquad m(t+2\pi)=m(t).
$$

In the central band, $f(t)=1$, so $f(2t)=m(t)f(t)$. In the rest of this fundamental interval, both $m(t)$ and $f(2t)$ vanish. If $\pi<|t|<4\pi/3$, reducing $t$ modulo $2\pi$ puts it in an outer band where $m=0$, and again $f(2t)=0$. For $|t|\ge4\pi/3$, both $f(t)$ and $f(2t)$ vanish. Endpoint choices affect only a null set. Thus the [complementary transition bands for a scaling function](../../../fourier-analysis.md#complementary-transition-bands-for-a-scaling-function) give **both Fourier conditions**, with this explicitly constructed periodic mask.

A concrete real-valued choice, illustrating that the transition constraints are consistent, is

$$
f(t)=\begin{cases}1,&|t|\le2\pi/3,\\\cos\!\left(\dfrac\pi2\left(\dfrac{3|t|}{2\pi}-1\right)\right),&2\pi/3<|t|<4\pi/3,\\0,&|t|\ge4\pi/3.\end{cases}
$$

On the positive transition band put $u=3t/(2\pi)-1\in[0,1]$. The other translate has parameter $1-u$, so the sum is $\cos^2(\pi u/2)+\sin^2(\pi u/2)=1$.

There is a genuine qualification in the printed formulation: it uses ordinary squares without explicitly declaring $f$ real-valued. If arbitrary complex values are allowed, the claimed verification is false. Take $f=1$ for $|t|\le2\pi/3$, $f=0$ for $|t|\ge4\pi/3$, and set

$$
f(t)=i\quad(2\pi/3<t<4\pi/3),\qquad f(t)=\sqrt2\quad(-4\pi/3<t<-2\pi/3).
$$

The printed complementary-square rule holds, including its endpoints: in the interior $i^2+(\sqrt2)^2=1$, while the endpoints pair one with zero. Nevertheless, for $2\pi/3<t<\pi$,

$$
\sum_k|f(t+2\pi k)|^2=|i|^2+|\sqrt2|^2=3.
$$

This compactly supported $L_2$ function is the [Fourier transform](../../../analysis.md#fourier-transform) of an $L_2$ function, so it is a counterexample within the natural complex [Hilbert space](../../../hilbert-space.md). **The verification is valid for real-valued $f$, or with absolute squares in the transition rule; it is not valid for unrestricted complex $f$ with ordinary squares.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
