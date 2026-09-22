# Paper 69

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_69.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_69.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [A](#2/a)
    - [Solution](#2/a/solution)
  - [B](#2/b)
    - [Solution](#2/b/solution)
  - [C](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
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
- [6](#6)
  - [1](#6/1)
    - [a](#6/1/a)
      - [Solution](#6/1/a/solution)
    - [b](#6/1/b)
      - [Solution](#6/1/b/solution)
  - [2](#6/2)
    - [Solution](#6/2/solution)
  - [3](#6/3)
    - [Solution](#6/3/solution)

## 1

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For [positive linear operators on continuous functions](../../../topological-vector-space.md#positive-linear-operator-on-continuous-functions), a general [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem), in its [compact Korovkin test space](../../../uniform-approximation.md#compact-korovkin-test-space) form, can be stated using a test space $H\subset C(K,\mathbb R)$, where $K$ is a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space). Assume $H$ contains a strictly positive function $h_0$. Require that, for every $x\in K$, the only [positive linear functional](../../../continuous-dual-space.md#positive-linear-functional) $L$ on $C(K)$ with $L(h)=h(x)$ for all $h\in H$ is evaluation at $x$. Then **convergence on the test space implies convergence on every continuous function**:

$$
\boxed{\|U_nh-h\|_\infty\longrightarrow0\ (h\in H)
\quad\Longrightarrow\quad\|U_nf-f\|_\infty\longrightarrow0\ (f\in C(K)).}
$$

By the [Riesz-Markov-Kakutani representation theorem](../../../functional-analysis.md#riesz-markov-kakutani-representation-theorem), the functional condition equivalently says that a positive measure with these test moments must be $\delta_x$. This permits arbitrary test families, not just the interval tests $1,x,x^2$.

For completeness, let $c=\min_Kh_0>0$. Positivity gives $U_n1\leq c^{-1}U_nh_0$, so the [operator norms](../../../continuous-dual-space.md#operator-norm) are uniformly bounded. If the conclusion failed for some $f$, choose $x_n$ where its error is bounded away from zero. The evaluation functionals $L_n(g)=U_ng(x_n)$ have uniformly bounded norm. Compactness of $K$ and the [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) give a subnet on which $x_n\to x$ and $L_n$ converges in the [weak-star topology](../../../weak-topology.md#weak-star-topology) to a positive $L$. For every $h\in H$, uniform test convergence gives $L(h)=h(x)$. The hypothesis forces $L(f)=f(x)$, contradicting the chosen errors. Complex-valued functions follow by applying the real result to their real and imaginary parts.

A useful concrete sufficient condition is that $1\in H$ and for each $x$ there is $g_x\in H$ with $g_x\geq0$ and zero set exactly $\{x\}$. Its zero moment forces the representing measure to be supported at $x$, while the constant moment fixes its mass.

For the circle, take $H=\operatorname{span}\{1,\sin t,\cos t\}$. The nonnegative function $g_x(t)=1-\cos(t-x)$ belongs to $H$ and vanishes only at $x$ on the circle. Thus **the periodic Korovkin test set is**

$$
\boxed{1,\ \sin x,\ \cos x.}
$$

[Uniform convergence](../../../real-analysis.md#uniform-convergence) on these three functions is sufficient for [uniform convergence](../../../real-analysis.md#uniform-convergence) on $C(\mathbb T)$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Averaging the given [Dirichlet kernels](../../../fourier-series.md#dirichlet-kernel) gives the normalized [Fejér kernel](../../../fourier-series.md#fejer-kernel)

$$
K_n(t)=\frac1{\pi n}\sum_{j=0}^{n-1}D_j(t)
=\frac1{2\pi n}\left(\frac{\sin(nt/2)}{\sin(t/2)}\right)^2.
$$

The geometric-series identity, or summing the sine terms, proves the second equality. At multiples of $2\pi$ use its removable value $n/(2\pi)$. Therefore $K_n\geq0$, and

$$
\sigma_n(f,x)=\int_{-\pi}^{\pi}K_n(t)f(x-t)\,dt
$$

is a [positive linear operator on continuous functions](../../../topological-vector-space.md#positive-linear-operator-on-continuous-functions). The [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum), viewed as [orthogonal projections](../../../hilbert-space.md#orthogonal-projection), fix $1$, so $\sigma_n1=1$ and $\int K_n=1$. They also fix $\sin x$ and $\cos x$ for degrees at least one, whereas $s_0$ annihilates them. Consequently

$$
\sigma_n(\sin x)=(1-1/n)\sin x,\qquad
\sigma_n(\cos x)=(1-1/n)\cos x.
$$

All three periodic [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem) tests converge uniformly. Hence **[Fejér sums](../../../fourier-series.md#fejer-sum) converge uniformly for every continuous periodic function**:

$$
\boxed{\|\sigma_n(f)-f\|_\infty\longrightarrow0.}
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Apply the periodic [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem) to the constant sequence $U_n=U$. Since it fixes the three test functions, the theorem gives $Uf=f$ for every $f$.

One can also see the rigidity directly. For fixed $x$, the [positive linear functional](../../../continuous-dual-space.md#positive-linear-functional) $L_x(f)=(Uf)(x)$ has $L_x(1)=1$ and is represented by a [probability measure](../../../probability-theory.md#probability-measure). The fixed sine and cosine imply $L_x(1-\cos(t-x))=0$. The integrand is nonnegative with unique zero $x$ on the circle, so the measure is $\delta_x$. Thus $(Uf)(x)=f(x)$ at every point. **The operator is uniquely the identity**: $\boxed{U=I}$.

## 2

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="2/a">A</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

An orthonormal [multiresolution analysis](../../../fourier-analysis.md#multiresolution-analysis) consists of closed subspaces $(V_j)_{j\in\mathbb Z}$ of the [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) $L^2(\mathbb R)$ with $V_j\subset V_{j+1}$, dense union, intersection $\{0\}$, and the dilation rule $f\in V_j\iff f(2\cdot)\in V_{j+1}$. A [scaling function](../../../fourier-analysis.md#scaling-function) $\phi$ has integer translates forming an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_0$. Equivalently,

$$
\phi_{j,n}(x)=2^{j/2}\phi(2^jx-n),\qquad n\in\mathbb Z,
$$

form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_j$. Let $W_j=V_{j+1}\ominus V_j$. Density and the trivial intersection imply $L^2(\mathbb R)=\bigoplus_{j\in\mathbb Z}W_j$.

Nesting gives the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation) $\phi(x)=\sum_na_n\phi(2x-n)$, with $h_n=a_n/\sqrt2$ the coefficients in the normalized finer-scale basis. [Orthogonality](../../../linear-algebra.md#orthogonal-vectors) of the translates gives $\sum_na_n\overline{a_{n-2r}}=2\delta_{r0}$. Its Fourier form is the [quadrature mirror filter](../../../fourier-analysis.md#quadrature-mirror-filter) identity $|m(t)|^2+|m(t+\pi)|^2=1$, where $m(t)=\tfrac12\sum_na_ne^{-int}$.

Set $b_n=(-1)^n\overline{a_{1-n}}$ and define $\psi(x)=\sum_nb_n\phi(2x-n)$ in $L^2$. Its high-pass symbol is $q(t)=-e^{-it}\overline{m(t+\pi)}$. The matrix

$$
\begin{pmatrix}m(t)&m(t+\pi)\\q(t)&q(t+\pi)\end{pmatrix}
$$

is unitary almost everywhere. Under the identification of $V_1$ with its finer-scale coefficient space, this two-channel unitary transform splits that space into the translates of $\phi$ and the translates of $\psi$. The latter are therefore an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $W_0$. Dilating gives **an [orthonormal wavelet](../../../fourier-analysis.md#orthonormal-wavelet) basis**

$$
\boxed{\{2^{j/2}\psi(2^jx-n):j,n\in\mathbb Z\}\text{ of }L^2(\mathbb R).}
$$

This [wavelet completion of a multiresolution filter](../../../fourier-analysis.md#wavelet-completion-of-a-multiresolution-filter) explains how the [multiresolution analysis](../../../fourier-analysis.md#multiresolution-analysis) supplies a single [orthonormal wavelet](../../../fourier-analysis.md#orthonormal-wavelet). The argument uses coefficient-space completeness, not just pairwise [orthogonality](../../../linear-algebra.md#orthogonal-vectors).

<h3 id="2/b">B</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the unnormalized [Fourier transform](../../../analysis.md#fourier-transform) in the question and the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem), with inverse factor $1/(2\pi)$. For a general $L^2$ [scaling function](../../../fourier-analysis.md#scaling-function), the transform is interpreted in the $L^2$ sense; the printed integral need not be absolutely convergent. All frequency identities are almost-everywhere statements.

Changing variables in the [Fourier transform](../../../analysis.md#fourier-transform) gives

$$
\widehat{\phi(2\cdot-n)}(\xi)=\frac12e^{-in\xi/2}f(\xi/2).
$$

Thus taking the transform of the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation) gives $f(\xi)=m(\xi/2)f(\xi/2)$, or

$$
\boxed{f(2t)=m(t)f(t),\qquad m(t)=\frac12\sum_na_ne^{-int}.}
$$

Conversely the same calculation and injectivity of the [Fourier transform](../../../analysis.md#fourier-transform) recover refinement, with convergence understood in $L^2$.

To justify both the [orthogonality](../../../linear-algebra.md#orthogonal-vectors) assertion and this convergence precisely, put $P(t)=\sum_{k\in\mathbb Z}|f(t+2\pi k)|^2$. It belongs to $L^1[-\pi,\pi]$ by monotone integration. The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) gives

$$
\langle\phi,\phi(\cdot-j)\rangle
=\frac1{2\pi}\int_{-\pi}^{\pi}P(t)e^{-ijt}\,dt.
$$

Hence orthonormality of all integer translates is equivalent, by [uniqueness of Fourier coefficients in L1](../../../fourier-series.md#uniqueness-of-fourier-coefficients-in-l1), to **the periodized-energy condition**

$$
\boxed{P(t)=1\quad\text{almost everywhere}.}
$$

When this holds, the squared norm of $\sum_na_n\phi(2\cdot-n)$ is $\tfrac12\sum_n|a_n|^2$, so square-summable coefficient series converge in $L^2$. In the converse direction the refinement identity and $P=1$ give, by splitting the periodization of $|f(2t)|^2$ into even and odd translates,

$$
1=|m(t)|^2+|m(t+\pi)|^2.
$$

Thus $m$ is bounded and its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) $a_n/2$ are square summable. If $m_N$ are its [Fourier partial sum](../../../fourier-series.md#fourier-partial-sum), then

$$
\int_{\mathbb R}|m_N(\xi/2)-m(\xi/2)|^2|f(\xi/2)|^2\,d\xi
=2\int_{-\pi}^{\pi}|m_N(t)-m(t)|^2P(t)\,dt\longrightarrow0.
$$

This verifies the transformed refinement series converges to $f$, completing the equivalence of the two pairs of conditions without imposing an unnecessary $L^1$ assumption on $\phi$.

<h3 id="2/c">C</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The half-open intervals $[-\pi+2\pi k,\pi+2\pi k)$ tile the line, so exactly one term contributes to $\sum_k|f(t+2\pi k)|^2$. It equals one almost everywhere.

Choose the [Shannon scaling mask](../../../fourier-analysis.md#shannon-scaling-mask), a $2\pi$-periodic [low-pass filter of a multiresolution analysis](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) which equals one on $[-\pi/2,\pi/2)$ and zero on the rest of $[-\pi,\pi)$. On the support of $f$ its product with $f(t)$ equals $f(2t)$; outside that support both sides vanish. Its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) give

$$
a_0=1,\qquad a_n=\frac{2\sin(n\pi/2)}{\pi n}\quad(n\ne0),
$$

so it also has the required symbol representation. The inverse [Fourier transform](../../../analysis.md#fourier-transform) gives **the [Shannon scaling function](../../../fourier-analysis.md#shannon-scaling-function)**

$$
\boxed{\phi(x)=\frac1{2\pi}\int_{-\pi}^{\pi}e^{ixt}\,dt
=\frac{\sin(\pi x)}{\pi x},\qquad\phi(0)=1.}
$$

This [sinc function](../../../analysis.md#sinc-function) has $L^2$ norm one. It illustrates why the [Fourier transform](../../../analysis.md#fourier-transform) convention in part B must allow $L^2$ transforms: the [Shannon scaling function](../../../fourier-analysis.md#shannon-scaling-function) is not absolutely integrable on the line.

## 3

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Define the [second modulus of smoothness](../../../uniform-approximation.md#second-modulus-of-smoothness) by $\omega_2(f,h)=\sup_{|u|\leq h}\|f(\cdot+u)-2f+f(\cdot-u)\|_\infty$. The [Jackson kernel](../../../uniform-approximation.md#jackson-kernel) is even, nonnegative and has integral one. Symmetrizing its [convolution](../../../fourier-analysis.md#convolution) therefore gives

$$
j_n(f,x)-f(x)=\frac12\int_{-\pi}^{\pi}[f(x+t)-2f(x)+f(x-t)]J_n(t)\,dt.
$$

We first establish the needed scaling rule. For the translation operator $T_u$, $(T_u^m-I)=(I+T_u+\cdots+T_u^{m-1})(T_u-I)$. Squaring gives $\|(T_u^m-I)^2f\|\leq m^2\|(T_u-I)^2f\|$. Central and forward second differences have the same norm. For every $|v|\leq|t|$, take $m=\lceil |v|/h\rceil$ and $u=v/m$. Taking the supremum over these $v$ proves

$$
\omega_2(f,|t|)\leq(1+|t|/h)^2\omega_2(f,h).
$$

The zero-step case is immediate.

For $|t|\leq\pi$, the inequalities $|\sin(nt/2)|\leq n|\sin(t/2)|$, $|\sin(nt/2)|\leq1$, and $|\sin(t/2)|\geq |t|/\pi$ imply

$$
0\leq J_n(t)\leq C\min\left(n,\frac1{n^3t^4}\right).
$$

Use the first estimate on $|t|\leq1/n$ and the second outside it. Then

$$
\int_{-\pi}^{\pi}(1+n|t|)^2J_n(t)\,dt
\leq C\left[n\int_0^{1/n}1\,dt+\frac1n\int_{1/n}^{\pi}\frac{dt}{t^2}\right]\leq C'.
$$

All constants are independent of $n$ and $f$. Combining these estimates proves **the [Jackson operator estimate](../../../uniform-approximation.md#jackson-operator-estimate)**

$$
\boxed{\|j_n(f)-f\|_\infty\leq C\,\omega_2(f,1/n).}
$$

For $f\in C^2(\mathbb T)$, two applications of the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) give the [second-difference integral formula](../../../uniform-approximation.md#second-difference-integral-formula)

$$
f(x+h)-2f(x)+f(x-h)=\int_{-h}^{h}(h-|u|)f''(x+u)\,du
$$

for $h\geq0$. Its absolute value is at most $h^2\|f''\|_\infty$, so $\omega_2(f,h)\leq h^2\|f''\|_\infty$.

Finally, $J_m$ is a [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) of degree $2(m-1)$: its sine ratio squared is a Fejér [polynomial](../../../polynomial.md) of degree $m-1$, and squaring doubles that degree. Thus $j_m(f)$ has degree at most $2(m-1)$. To bound degree-$n$ best approximation, choose $m=\lfloor n/2\rfloor+1$, rather than using $j_n$ directly. Since $m\geq n/2$ for $n\geq1$, **the smooth-function approximation rate is**

$$
\boxed{E_n(f)\leq\|j_m(f)-f\|_\infty\leq\frac{C_1}{n^2}\|f''\|_\infty.}
$$

## 4

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $u^*\in\mathcal U$, $e=f-u^*$, $d=\|e\|_\infty$, and $E=\{x:|e(x)|=d\}$. The real [Kolmogorov criterion for uniform approximation](../../../uniform-approximation.md#kolmogorov-criterion-for-uniform-approximation) says **$u^*$ is best if and only if**

$$
\boxed{\text{for every }v\in\mathcal U,\quad\min_{x\in E}e(x)v(x)\leq0.}
$$

Equivalently, no direction $v$ has the error's sign strictly at every extremal point. If $d=0$, the criterion is automatic.

For sufficiency, a point with $e(x)v(x)\leq0$ gives $|e(x)-v(x)|\geq d$, so $u^*+v$ cannot improve the norm. For necessity, suppose $e(x)v(x)>0$ on $E$. Compactness gives a positive lower bound there and on a neighbourhood of $E$. On that neighbourhood, $(e-\tau v)^2=e^2-2\tau ev+\tau^2v^2<d^2$ for sufficiently small positive $\tau$. Off the neighbourhood, $|e|$ has a strict gap below $d$, and small $\tau$ preserves that gap. Thus $u^*+\tau v$ has smaller error, a contradiction. This also explains why the criterion involves all active extrema.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $p\in\mathcal P_n$ and $e=f-p$, with $d=\|e\|_\infty>0$. **The [Chebyshev alternation theorem](../../../uniform-approximation.md#equioscillation-theorem) is**

$$
\boxed{p\text{ is best}\iff\exists x_0<\cdots<x_{n+1},\quad e(x_i)=\varepsilon(-1)^id,\quad\varepsilon\in\{1,-1\}.}
$$

If such points exist and a [polynomial](../../../polynomial.md) $v\in\mathcal P_n$ had $e(x)v(x)>0$ at every extremum, its signs at those $n+2$ points would alternate. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) would give at least $n+1$ distinct zeros, impossible for a nonzero degree-at-most-$n$ [polynomial](../../../polynomial.md). The [Kolmogorov criterion for uniform approximation](../../../uniform-approximation.md#kolmogorov-criterion-for-uniform-approximation) therefore proves sufficiency.

For necessity, let $E_+=\{e=d\}$ and $E_-=\{e=-d\}$. They are disjoint compact sets. If one set is empty there is just one sign block. Otherwise their positive separation implies that, reading the extremal set from left to right, its signs form finitely many alternating blocks. If there are fewer than $n+2$ alternating extrema, there are at most $n+1$ blocks. Place one point $\xi_j$ in each extremum-free gap between consecutive blocks. A scalar multiple of $v(x)=\prod_j(x-\xi_j)$ can be chosen to have exactly the sign of $e$ on every block. Its degree is at most $n$, and $ev>0$ throughout $E$, contradicting the [Kolmogorov criterion for uniform approximation](../../../uniform-approximation.md#kolmogorov-criterion-for-uniform-approximation). Thus there must be at least $n+2$ alternating extrema. If $d=0$, the exact [polynomial](../../../polynomial.md) is already best and the equalities with zero error are automatic.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Fix the degree bound $n$. Existence can be proved without a general uniqueness theorem: a minimizing sequence in $\mathcal P_n$ is uniformly bounded because its distances from $f$ are bounded. Values at any fixed $n+1$ distinct points determine its coefficients through an invertible [Vandermonde matrix](../../../galois-theory.md#vandermonde-matrix), so those coefficients are bounded. A convergent subsequence supplies a [polynomial](../../../polynomial.md) attaining the minimum.

For [uniqueness of best uniform polynomial approximation](../../../uniform-approximation.md#uniqueness-of-best-uniform-polynomial-approximation), suppose $p$ and $q$ attain the same minimum $d$, and let $r=(p+q)/2$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) makes $r$ another minimizer. If $d=0$, both [polynomials](../../../polynomial.md) equal $f$, so assume $d>0$. Put $e=f-r$ and $E=\{|e|=d\}$. At each $x\in E$, the two real errors $f-p$ and $f-q$ lie in $[-d,d]$ and their average equals an endpoint. Hence they are equal there, and $p(x)=q(x)$.

The set $E$ must contain at least $n+2$ points. Otherwise interpolate the values $\operatorname{sign}e(x)$ on its at most $n+1$ points by a [polynomial](../../../polynomial.md) $v\in\mathcal P_n$. Then $ev>0$ on $E$. Continuity gives this positivity on a neighbourhood of $E$, while the error has a strict gap below $d$ on the compact complement. A sufficiently small positive multiple of $v$ decreases the maximum error, contradicting optimality of $r$. This is an elementary perturbation argument, not an appeal to Haar's theorem.

Thus $p-q$ has at least $n+2$ distinct zeros. A [polynomial](../../../polynomial.md) of degree at most $n$ with that many zeros is identically zero. **The best uniform [polynomial](../../../polynomial.md) is unique for every fixed degree bound**: $\boxed{p=q}$.

## 5

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Write $g_t(y)=(y-t)_+^{k-1}$. Begin with distinct increasing knots so ordinary [polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation) is unambiguous. The two interpolants agree at the $k-1$ common knots $t_{i+1},\ldots,t_{i+k-1}$. Their difference is consequently a scalar multiple of the monic [polynomial](../../../polynomial.md) $\omega_i$ of degree $k-1$.

The leading coefficient of an interpolant is its highest [divided difference](../../../numerical-analysis.md#divided-difference). Thus this scalar is

$$
[t_{i+1},\ldots,t_{i+k}]g_t-[t_i,\ldots,t_{i+k-1}]g_t
=(t_{i+k}-t_i)[t_i,\ldots,t_{i+k}]g_t=N_i(t).
$$

The equality is precisely the divided-difference recurrence. This proves **the [Lee interpolation identity](../../../uniform-approximation.md#lee-interpolation-identity)**:

$$
\boxed{\ell_{i+1}(x,t)-\ell_i(x,t)=\omega_i(x)N_i(t).}
$$

For $k=1$ the common-knot product is empty; the same argument is a difference of constants. Interpret $(y-t)_+^0$ as $1_{y>t}$ to obtain the usual half-open order-one [B-splines](../../../uniform-approximation.md#b-spline). Repeated knots use the standard confluent or limiting interpretation, where the interpolation data are defined.

Sum over $i=1,\ldots,n$. The right side telescopes to $\ell_{n+1}(x,t)-\ell_1(x,t)$. When $t_k<t<t_{n+1}$, the first interpolation nodes all lie below $t$, so $\ell_1=0$. The last interpolation nodes all lie above $t$, so $\ell_{n+1}$ interpolates the [polynomial](../../../polynomial.md) $(x-t)^{k-1}$ of degree $k-1$ and equals it identically. Hence **the [Marsden identity](../../../uniform-approximation.md#marsden-identity) follows**:

$$
\boxed{(x-t)^{k-1}=\sum_{i=1}^n\omega_i(x)N_i(t),\qquad t_k<t<t_{n+1}.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Set $d=k-1$ and let $e_m(t_{i+1},\ldots,t_{i+d})$ be the [elementary symmetric polynomial](../../../polynomial.md#elementary-symmetric-polynomial) of degree $m$ in the interior knots, with $e_0=1$. Expand the [Marsden identity](../../../uniform-approximation.md#marsden-identity) in powers of $x$. The coefficient of $x^{d-m}$ on the left is $(-1)^m\binom dm t^m$; that coefficient in $\omega_i(x)$ is $(-1)^me_m(t_{i+1},\ldots,t_{i+d})$. Comparing and cancelling the sign proves **the [monomial B-spline coefficients](../../../uniform-approximation.md#monomial-b-spline-coefficients)**:

$$
\boxed{a_i^{(m)}=\frac{e_m(t_{i+1},\ldots,t_{i+k-1})}{\binom{k-1}{m}},\qquad0\leq m\leq k-1.}
$$

For $m=0$ this gives [partition of unity](../../../differential-geometry.md#partition-of-unity) on the basic interval. For $m=1$ it gives the [Greville abscissae](../../../uniform-approximation.md#greville-abscissa), the arithmetic means of the $k-1$ interior knots. For the top degree it gives their product. When $k=1$, only $m=0$ occurs and the empty symmetric [polynomial](../../../polynomial.md) is one.

## 6

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="6/1">1</h3>

↑ **Parent:** [6](#6)

<h4 id="6/1/a">a</h4>

↑ **Parent:** [1](#6/1)

<h5 id="6/1/a/solution">Solution</h5>

↑ **Parent:** [A](#6/1/a)

Put $e=x-u^*$. If $u^*$ minimizes distance, then for every $v\in\mathcal U_n$ and every real $t$,

$$
\|e-tv\|^2=\|e\|^2-2t\operatorname{Re}(e,v)+t^2\|v\|^2\geq\|e\|^2.
$$

Both signs of arbitrarily small $t$ force $\operatorname{Re}(e,v)=0$. In a complex [inner product space](../../../linear-algebra.md#inner-product-space), apply the same argument to $iv$ to obtain the imaginary part too. Conversely, if $e$ is orthogonal to the subspace, the [Pythagorean theorem for inner product spaces](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives

$$
\|x-u\|^2=\|x-u^*\|^2+\|u-u^*\|^2\qquad(u\in\mathcal U_n).
$$

Thus **[orthogonality](../../../linear-algebra.md#orthogonal-vectors) characterizes the unique best approximation**:

$$
\boxed{u^*\text{ is best}\iff(x-u^*,v)=0\quad(v\in\mathcal U_n).}
$$

Finite dimension also guarantees existence by solving the invertible [Gram matrix](../../../linear-algebra.md#gram-matrix) normal equations; completeness of the ambient [inner product space](../../../linear-algebra.md#inner-product-space) is unnecessary.

<h4 id="6/1/b">b</h4>

↑ **Parent:** [1](#6/1)

<h5 id="6/1/b/solution">Solution</h5>

↑ **Parent:** [B](#6/1/b)

Use the convention that the [inner product](../../../linear-algebra.md#inner-product) is conjugate-linear in its first argument; the real case is the same without conjugates. [Linear independence](../../../vector-space.md#linear-independence) makes the [Gram matrix](../../../linear-algebra.md#gram-matrix) $G$ positive definite, so $B=G^{-1}$ exists and is Hermitian. Define the [Riesz dual basis in an inner product space](../../../linear-algebra.md#riesz-dual-basis-in-an-inner-product-space) within $\mathcal U_n$ by

$$
\widehat u_k=\sum_{l=1}^n b_{lk}u_l.
$$

Then $(u_i,\widehat u_k)=\sum_lG_{il}b_{lk}=\delta_{ik}$. Its own Gram entries are

$$
(\widehat u_j,\widehat u_k)=\sum_{l,m}\overline{b_{lj}}G_{lm}b_{mk}
=(B^*GB)_{jk}=B_{jk}.
$$

Hence **the inverse [Gram matrix](../../../linear-algebra.md#gram-matrix) is the [Gram matrix](../../../linear-algebra.md#gram-matrix) of the dual vectors**:

$$
\boxed{b_{jk}=(\widehat u_j,\widehat u_k).}
$$

The dual vectors are required to lie in $\mathcal U_n$; adding arbitrary vectors orthogonal to that subspace would preserve the displayed biorthogonality but would destroy this conclusion.

<h3 id="6/2">2</h3>

↑ **Parent:** [6](#6)

<h4 id="6/2/solution">Solution</h4>

↑ **Parent:** [2](#6/2)

Use the standard partition normalization of [B-splines](../../../uniform-approximation.md#b-spline), not rescaling each spline to have supremum exactly one. Let $h_i=t_{i+k}-t_i>0$. Then $M_i=kN_i/h_i$. In the ordinary real [inner product](../../../linear-algebra.md#inner-product), the [mixed-normalization spline Gram matrix](../../../uniform-approximation.md#mixed-normalization-spline-gram-matrix) is $G=D^{-1}H$, where $D=\operatorname{diag}(h_i/k)$ and $H_{ij}=(N_i,N_j)$. Since the $N_i$ form a basis, $H$ is positive definite; $D$ is invertible, so $G$ is invertible. The undeclared upper index $h$ in the printed matrix should be $n$.

We need the standard positivity and normalization properties with their justification. The [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula) is

$$
N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t),
$$

with zero-width terms interpreted as zero. It starts from nonnegative interval indicators. On each lower-order spline's support, its recurrence coefficients are nonnegative, so induction gives $N_i\geq0$. Extend the finite knots outside their endpoints to a full knot sequence. In the full sum, coefficients of each lower-order spline add to one, so the recurrence preserves [partition of unity](../../../differential-geometry.md#partition-of-unity). Our finite collection is a subset of nonnegative [B-splines](../../../uniform-approximation.md#b-spline); therefore $\sum_{i=1}^nN_i(t)\leq1$ everywhere. The [Marsden identity](../../../uniform-approximation.md#marsden-identity) gives equality on the basic knot interval.

The divided-difference definition also gives support in $[t_i,t_{i+k}]$: below the left endpoint the knot-data function is a [polynomial](../../../polynomial.md) of degree $k-1$, whose order-$k$ [divided difference](../../../numerical-analysis.md#divided-difference) vanishes; above the right endpoint the knot data vanish. Choose $a<t_i$ and $b>t_{i+k}$. Integrating in $t$ and then taking the [divided difference](../../../numerical-analysis.md#divided-difference) in its knot variable gives

$$
\int M_i(t)\,dt
=k[t_i,\ldots,t_{i+k}]\left(\frac{(\cdot-a)^k}{k}\right)=1,
$$

because an order-$k$ [divided difference](../../../numerical-analysis.md#divided-difference) of a monic degree-$k$ [polynomial](../../../polynomial.md) is one. The support lies inside $[0,1]$, so $\int_0^1M_i=1$.

[Orthogonality](../../../linear-algebra.md#orthogonal-vectors) of $f-s^*$ to the spline space gives $Ga=r$, with $r_i=(M_i,f)$. Since $M_i\geq0$ and has unit integral, $|r_i|\leq\|f\|_\infty$. The induced matrix maximum norm is the absolute row-sum norm, so

$$
\|a\|_{\ell^\infty}\leq\|G^{-1}\|_{\ell^\infty}\|f\|_\infty,
\qquad
|s^*(t)|\leq\|a\|_{\ell^\infty}\sum_iN_i(t)\leq\|a\|_{\ell^\infty}.
$$

Taking the supremum over nonzero $f$ proves **the [maximum-norm bound for spline projection](../../../uniform-approximation.md#maximum-norm-bound-for-spline-projection)**:

$$
\boxed{\|P_{\mathcal S}\|_\infty\leq\|G^{-1}\|_{\ell^\infty}.}
$$

The range is $\mathcal S$, so the printed phrase “onto $C[0,1]$” must mean into $C[0,1]$, and onto $\mathcal S$. Continuity of the range requires continuous [B-splines](../../../uniform-approximation.md#b-spline), for example $k\geq2$ and internal multiplicities at most $k-1$. For order-one or discontinuous [B-splines](../../../uniform-approximation.md#b-spline), the same bound is valid with codomain $L^\infty[0,1]$ rather than $C[0,1]$.

<h3 id="6/3">3</h3>

↑ **Parent:** [6](#6)

<h4 id="6/3/solution">Solution</h4>

↑ **Parent:** [3](#6/3)

Fix $i$. If $t<t_i$, all knot values of the function $x\mapsto(x-t)_+^{k-1}$ agree with a [polynomial](../../../polynomial.md) of degree $k-1$. Its order-$k$ [divided difference](../../../numerical-analysis.md#divided-difference) vanishes. If $t>t_{i+k}$, all the knot values are zero, so the same [divided difference](../../../numerical-analysis.md#divided-difference) again vanishes. Thus **the support is finite**:

$$
\boxed{\operatorname{supp}M_i\subseteq[t_i,t_{i+k}],\qquad\operatorname{supp}N_i\subseteq[t_i,t_{i+k}].}
$$

The [support and Gram bandwidth of B-splines](../../../uniform-approximation.md#support-and-gram-bandwidth-of-b-splines) also holds at repeated knots: the same conclusion follows with the standard limiting convention. If $j\geq i+k$, then $t_j\geq t_{i+k}$, so the two supports have no positive-length overlap. An endpoint intersection contributes zero to the integral defining $G_{ij}$. The case $i\geq j+k$ is identical. Hence

$$
\boxed{G_{ij}=0\quad\text{when }|i-j|\geq k,\qquad d=k.}
$$

For strictly increasing knots, [B-splines](../../../uniform-approximation.md#b-spline) whose indices differ by $k-1$ overlap on a positive-length interval and their product is positive there, so this universal bound is sharp. In standard matrix terminology the half-bandwidth is $k-1$ and the full bandwidth is $2k-1$; the paper's integer $d$ is $k$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
