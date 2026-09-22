# Paper 326

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_326.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_326.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
  - [vi](#2/vi)
    - [Solution](#2/vi/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)

## 1

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) $K:U\to V$ between [Hilbert spaces](../../../hilbert-space.md), the [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) assigns to each admissible datum its unique [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution). Its domain is

$$
\boxed{\mathcal D(K^\dagger)=\operatorname{ran}K\oplus(\operatorname{ran}K)^\perp.}
$$

Write $f=Ku+h$, where $u\in(\ker K)^\perp$ and $h\in(\operatorname{ran}K)^\perp=\ker K^*$. Then $K^\dagger f=u$. Restricting to $(\ker K)^\perp$ removes the ambiguity among solutions differing by an element of the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). The [orthogonal decomposition](../../../hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) also shows that $KK^\dagger f$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) of $f$ onto $\overline{\operatorname{ran}K}$, and $K^\dagger Ku$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) of $u$ onto $(\ker K)^\perp$. The inverse is defined on a dense domain and need not be a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) when the range is not closed.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The given map is the [unilateral shift operator](../../../linear-operator-theory.md#unilateral-shift-operator). Its [adjoint operator](../../../hilbert-space.md#adjoint-operator) is the [left shift operator](../../../linear-operator-theory.md#left-shift-operator), since

$$
\langle Ku,f\rangle=\sum_{j\geq1}u_j\overline{f_{j+1}},\qquad K^*f=(f_2,f_3,\ldots).
$$

The shift is an [isometry](../../../riemannian-geometry.md#isometry) with trivial [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and closed range $\{f:f_1=0\}$. Its range has [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) $\operatorname{span}\{e_1\}$, so **every square-summable datum is admissible**. Consequently,

$$
\boxed{\mathcal D(K^\dagger)=\ell^2,\qquad K^\dagger(f_1,f_2,\ldots)=(f_2,f_3,\ldots)=K^*f.}
$$

Indeed $K^\dagger K=I$, while $KK^\dagger f=f-f_1e_1$ is the required [orthogonal projection](../../../hilbert-space.md#orthogonal-projection). The discarded first component is the residual of the [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem), not an obstruction to the existence of the [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Choose a [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator) with $Kv_j=\sigma_j u_j$, $K^*u_j=\sigma_jv_j$ and $\sigma_j>0$. The [Picard criterion](../../../inverse-problem.md#picard-criterion), together with range orthogonality, gives

$$
\boxed{f\in\operatorname{ran}K\iff f\perp\ker K^*\ \text{and}\ \sum_j\frac{|\langle f,u_j\rangle|^2}{\sigma_j^2}<\infty.}
$$

For necessity, expand a solution's component in $(\ker K)^\perp$ in the [orthonormal](../../../linear-algebra.md#orthonormal-set) vectors $v_j$; its coefficients must be $\langle f,u_j\rangle/\sigma_j$. Their square sum is finite by [Bessel's inequality](../../../hilbert-space.md#bessel-s-inequality). Conversely, the displayed square sum defines a convergent [Hilbert space](../../../hilbert-space.md) series

$$
K^\dagger f=\sum_j\frac{\langle f,u_j\rangle}{\sigma_j}v_j.
$$

Applying the [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) $K$ to the partial sums yields the expansion of $f$ in $\overline{\operatorname{ran}K}=(\ker K^*)^\perp$. Thus its limit solves $Ku=f$. The perpendicularity condition is essential here: the [Picard criterion](../../../inverse-problem.md#picard-criterion) alone characterizes the domain of the generalized inverse, which also includes components in $\ker K^*$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

A [linear regularization](../../../inverse-problem.md#linear-regularization) is a family of [bounded linear operators](../../../topological-vector-space.md#continuous-linear-operator) $R_\alpha:V\to U$, $\alpha>0$, for which $R_\alpha f\to K^\dagger f$ for every $f\in\mathcal D(K^\dagger)$ as $\alpha\downarrow0$. To obtain a [convergent regularization of an inverse problem](../../../inverse-problem.md#convergent-regularization-of-an-inverse-problem) for noisy data, choose a [regularization parameter](../../../inverse-problem.md#regularization-parameter) so that the exact-data approximation error and the amplified noise both vanish.

An example is [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization):

$$
\boxed{R_\alpha=(K^*K+\alpha I)^{-1}K^*.}
$$

The positive quadratic term makes $K^*K+\alpha I$ invertible. The [Tikhonov filter norm bound](../../../inverse-problem.md#tikhonov-filter-norm-bound) follows from the filter $s/(s^2+\alpha)$, whose maximum for $s\geq0$ is $1/(2\sqrt\alpha)$. Therefore $\|R_\alpha\|\leq1/(2\sqrt\alpha)$. The spectral factors $s^2/(s^2+\alpha)$ tend to one on the positive spectrum; [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives consistency on $\mathcal D(K^\dagger)$. The [noise-bias decomposition for linear regularization](../../../inverse-problem.md#noise-bias-decomposition-for-linear-regularization) then proves convergence whenever $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$, for example $\alpha(\delta)=\delta$ for sufficiently small positive noise levels.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

The [Volterra integration operator](../../../functional-analysis.md#volterra-operator) is injective and has dense range. Its [range of the Volterra integration operator](../../../functional-analysis.md#range-of-the-volterra-integration-operator) is $\{f\in H^1(0,1):f(0)=0\}$, and its [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) is differentiation on this domain. Thus the error estimate for $K^\dagger f$ implicitly requires $f(0)=0$, in addition to the printed $H^2$ assumption. For an arbitrary $H^2$ function the same calculation bounds error against $f'$, but that function need not be in $\mathcal D(K^\dagger)$.

Put $a=(1-\alpha)/2$, $b=(1+\alpha)/2$ and $h=\alpha/2$. The three stencils are forward, [central finite differences](../../../finite-difference.md#central-finite-difference), and backward on $[0,a)$, $[a,b)$ and $[b,1]$, respectively. All shifted evaluation points lie in $[0,1]$. For $g\in L^2(0,1)$, apply $|A-B|^2\leq2(|A|^2+|B|^2)$ and change variables in each of the six evaluation terms. The resulting integration intervals are

$$
[\alpha,b],\quad[0,a],\quad[1/2,1/2+\alpha],\quad[1/2-\alpha,1/2],\quad[b,1],\quad[a,1-\alpha].
$$

Pair $[0,a]$ with $[a,1-\alpha]$, $[\alpha,b]$ with $[b,1]$, and the two middle intervals. Each pair has disjoint interiors, so almost every point is counted at most three times. This [overlap multiplicity bound for piecewise difference operators](../../../inverse-problem.md#overlap-multiplicity-bound-for-piecewise-difference-operators) proves

$$
\|R_\alpha g\|_2^2\leq\frac6{\alpha^2}\|g\|_2^2,\qquad \|R_\alpha\|\leq\frac{\sqrt6}{\alpha}.
$$

For the bias on the middle interval, write the [central finite difference](../../../finite-difference.md#central-finite-difference) as an average of $f'$. The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives

$$
R_\alpha f(x)-f'(x)=\int_{-h}^h k_\alpha(s)f''(x+s)\,ds,\qquad k_\alpha(s)=\frac{\operatorname{sgn}(s)(h-|s|)}{\alpha},
$$

where $\|k_\alpha\|_1=\alpha/4$. Extend $f''$ by zero to the [real line](../../../real-analysis.md#real-line). [Young's convolution inequality](../../../fourier-analysis.md#young-s-convolution-inequality) bounds the middle-interval $L^2$ error by $\alpha c/4$. Combining its squared error with the supplied outer-interval estimate gives the [central-difference noise-bias bound](../../../inverse-problem.md#central-difference-noise-bias-bound)

$$
\|R_\alpha f-f'\|_2\leq\sqrt{\alpha^2c^2+\alpha^2c^2/16}=\frac{\sqrt{17}}4\alpha c.
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) and the [operator norm](../../../continuous-dual-space.md#operator-norm) estimate now give

$$
\boxed{\|K^\dagger f-R_\alpha f^\delta\|_2\leq\frac{\sqrt6\,\delta}{\alpha}+\frac{\sqrt{17}}4\alpha c.}
$$

For $c>0$, [balancing noise and approximation bias](../../../inverse-problem.md#balancing-noise-and-approximation-bias) minimizes this upper bound at

$$
\boxed{\alpha(\delta)=2(6/17)^{1/4}\sqrt{\delta/c},\qquad \|K^\dagger f-R_{\alpha(\delta)}f^\delta\|_2\leq102^{1/4}\sqrt{\delta c},}
$$

for sufficiently small $\delta$ that $\alpha<1/2$. Capping the parameter at $1/4$ supplies an admissible rule for all positive noise levels. More generally, $\alpha\to0$ and $\delta/\alpha\to0$ suffice; $\alpha=\sqrt\delta$ avoids needing $c$ or dividing by $c=0$.

To prove convergence for every admissible datum, not just $H^2$ data, let $f=Ku$ with $u\in L^2(0,1)$ and extend $u$ by zero. Each stencil is a forward, centred or backward average of $u$. [Translation continuity in Lp](../../../measure-theory.md#translation-continuity-in-lp) makes each averaged difference from $u$ tend to zero in $L^2(\mathbb R)$. Restricting those three bounds to their respective intervals proves $R_\alpha Ku\to u$. The [noise-bias decomposition for linear regularization](../../../inverse-problem.md#noise-bias-decomposition-for-linear-regularization), with $\delta/\alpha\to0$, finishes the [convergent regularization of an inverse problem](../../../inverse-problem.md#convergent-regularization-of-an-inverse-problem).

## 2

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For a [proper convex function](../../../real-analysis.md#proper-convex-function) $E$ on a real [Hilbert space](../../../hilbert-space.md), its [subdifferential](../../../convex-optimization.md#subdifferential) at $y$ is

$$
\partial E(y)=\{p:E(x)\geq E(y)+\langle p,x-y\rangle\text{ for every }x\}.
$$

In a [Banach space](../../../banach-space.md), interpret the pairing with an element of the [dual space](../../../linear-algebra.md#dual-space). For a chosen [subgradient](../../../real-analysis.md#subgradient) $p\in\partial E(y)$, the [Bregman distance](../../../inverse-problem.md#bregman-divergence) is

$$
\boxed{D_E^p(x,y)=E(x)-E(y)-\langle p,x-y\rangle\geq0.}
$$

If also $q\in\partial E(x)$, its [symmetric Bregman distance](../../../inverse-problem.md#symmetric-bregman-distance) is

$$
\boxed{D_E^p(x,y)+D_E^q(y,x)=\langle q-p,x-y\rangle.}
$$

The [subgradient inequality](../../../real-analysis.md#subgradient-inequality) proves nonnegativity. These quantities depend on the chosen [subgradients](../../../real-analysis.md#subgradient) and generally are not [metrics](../../../topological-analysis.md#metric): they need not distinguish different points or obey the [triangle inequality](../../../topological-analysis.md#triangle-inequality).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For the [maximum-entropy regularization functional](../../../inverse-problem.md#maximum-entropy-regularization-functional), differentiation of the scalar integrand gives $(s\log s-s)'=\log s$. Thus the [Fréchet derivative](../../../calculus.md#frechet-derivative) at a positive reference function $y$ is $E'(y)=\log y$, and the stated differentiability result gives $\partial E(y)=\{\log y\}$. Consequently,

$$
\boxed{D_E(x,y)=\int_\Omega\left[x\log\frac{x}{y}-x+y\right]dt.}
$$

This is the [generalized Kullback–Leibler divergence](../../../probability-and-statistics.md#generalized-kullback-leibler-divergence). When both functions integrate to the same mass, the last two terms cancel after integration; for [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) it becomes the usual [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence). For two positive functions, adding the reverse distance gives

$$
\boxed{D_E^{\mathrm{sym}}(x,y)=\int_\Omega(x-y)(\log x-\log y)\,dt.}
$$

A sufficient setting for the differentiability argument is $L^\infty(\Omega)$ with $y$ bounded away from zero. For nonnegative $x$, use $0\log(0/y)=0$ wherever appropriate. Positivity alone in $L^2$ does not automatically provide an open domain on which the [Fréchet derivative](../../../calculus.md#frechet-derivative) exists.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

For $E(x)=|x|$, the [subdifferential](../../../convex-optimization.md#subdifferential) at zero is $[-1,1]$. Choose the allowed interior [subgradient](../../../real-analysis.md#subgradient) **$p=0$**. Its supporting line is horizontal, so the [Bregman distance](../../../inverse-problem.md#bregman-divergence) is the vertical gap from $y=0$ to $y=|x|$ at the selected input:

$$
\boxed{D_E^0(1,0)=|1|-|0|-0(1-0)=1.}
$$

More generally, an interior choice $-1<p<1$ gives $D_E^p(1,0)=1-p$. The sketch shows the particular choice $p=0$.

<a id="2/iii/image-bregman-distance-for-the-absolute-value-function-at-x-1-from-the-reference-point-zero-using-the-subgradient-p-0"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326-bregman-gap.png)

**[Figure 1](#2/iii/image-bregman-distance-for-the-absolute-value-function-at-x-1-from-the-reference-point-zero-using-the-subgradient-p-0). Bregman distance for the absolute-value function at x=1 from the reference point zero, using the subgradient p=0**.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Interpret the [normal-operator source condition](../../../inverse-problem.md#normal-operator-source-condition) as the displayed intersection condition: there is $v\in U$ with $w=K^*Kv\in\partial J(u^\dagger)$. Fix any $\alpha>0$ and put $\bar u=u^\dagger+\alpha v$. The [subgradient optimality condition](../../../real-analysis.md#subgradient-optimality-condition) for the artificial-data objective is

$$
0\in K^*(Ku^\dagger-K\bar u)+\alpha\partial J(u^\dagger).
$$

It holds because its first term equals $-\alpha K^*Kv=-\alpha w$. By [convexity](../../../real-analysis.md#convex-function), this is sufficient for global minimality, proving the forward implication. Conversely, if $u^\dagger$ minimizes that objective, the same optimality condition gives

$$
w=\frac1\alpha K^*K(\bar u-u^\dagger)\in\partial J(u^\dagger).
$$

Taking $v=(\bar u-u^\dagger)/\alpha$ proves the intersection condition. Thus **the two conditions are equivalent when the source vector is allowed to be zero**.

The printed additional requirement $v\ne0$ is not equivalent in general. For $K=I$ and $J\equiv0$, the displayed source condition holds, and choosing $\bar u=u^\dagger$ makes $u^\dagger$ the minimizer, but $\partial J(u^\dagger)=\{0\}$ forces $v=0$. A nonzero-source version needs an additional hypothesis, such as requiring $w\ne0$; it cannot be inferred from the printed intersection alone.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

Let $w=K^*Kv\in\partial J(u^\dagger)$ from the [normal-operator source condition](../../../inverse-problem.md#normal-operator-source-condition), and set $e=u-u^\dagger$. Since $u^\dagger$ is a [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem), the [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) gives $K^*(Ku^\dagger-f)=0$. Expand the objective difference and use the [Bregman distance](../../../inverse-problem.md#bregman-divergence) definition:

$$
\begin{aligned}
\mathcal F_\alpha(u)-\mathcal F_\alpha(u^\dagger)
&=\frac12\|Ke\|^2+\alpha[J(u)-J(u^\dagger)]\\
&=\frac12\|Ke\|^2+\alpha\langle Kv,Ke\rangle+\alpha D_J^w(u,u^\dagger)\\
&=\frac12\|K(e+\alpha v)\|^2+\alpha D_J^w(u,u^\dagger)-\frac{\alpha^2}2\|Kv\|^2.
\end{aligned}
$$

The cross term with the residual of the [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) vanishes by the normal equation; exact data are not required. Compare the minimizing $u_\alpha$ with $z=u^\dagger-\alpha v$. At $z$, the completed square is zero. Dividing the resulting inequality by $\alpha$ proves the stronger [shifted-comparator Bregman bound](../../../inverse-problem.md#shifted-comparator-bregman-bound)

$$
\boxed{D_J^w(u_\alpha,u^\dagger)+\frac1{2\alpha}\|K(u_\alpha-u^\dagger+\alpha v)\|^2\leq D_J^w(u^\dagger-\alpha v,u^\dagger),\qquad w=K^*Kv.}
$$

Dropping the nonnegative squared term gives the requested estimate. If the comparator lies outside the effective domain of $J$, its distance is infinite and the inequality is valid but gives no finite error bound.

<h3 id="2/vi">vi</h3>

↑ **Parent:** [2](#2)

<h4 id="2/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#2/vi)

The relevant nonlinear [generalized singular vector](../../../convex-optimization.md#generalized-singular-vector) relation, without imposing unit-data normalization, is

$$
p=\lambda K^*Ku^\dagger\in\partial J(u^\dagger),\qquad u^\dagger\ne0.
$$

This is a [generalized eigenfunction in the forward-operator metric](../../../convex-optimization.md#generalized-eigenfunction-in-the-forward-operator-metric), rather than a distributional generalized eigenfunction of a linear operator. It supplies the [normal-operator source condition](../../../inverse-problem.md#normal-operator-source-condition) with $v=\lambda u^\dagger$. For a [convex positively one-homogeneous functional](../../../convex-optimization.md#convex-positively-one-homogeneous-functional), the [subgradient inequality](../../../real-analysis.md#subgradient-inequality) applied at zero and at $2u^\dagger$ gives $\langle p,u^\dagger\rangle=J(u^\dagger)$. If $Ku^\dagger\ne0$, then

$$
\lambda=\frac{J(u^\dagger)}{\|Ku^\dagger\|^2}.
$$

Assume the usual positive eigenvalue $\lambda>0$ and $0<\alpha\lambda\leq1$. By [positive homogeneity](../../../real-analysis.md#positively-homogeneous-function-degree-one),

$$
D_J^p((1-\alpha\lambda)u^\dagger,u^\dagger)=0.
$$

The [shifted-comparator Bregman bound](../../../inverse-problem.md#shifted-comparator-bregman-bound) therefore yields

$$
\boxed{D_J^p(u_\alpha,u^\dagger)=0,\qquad Ku_\alpha=(1-\alpha\lambda)Ku^\dagger.}
$$

The vector $(1-\alpha\lambda)u^\dagger$ is itself a minimizer: $p$ remains a [subgradient](../../../real-analysis.md#subgradient) along the nonnegative ray, and substitution satisfies the [subgradient optimality condition](../../../real-analysis.md#subgradient-optimality-condition). If $K$ is injective, this also proves $u_\alpha=(1-\alpha\lambda)u^\dagger$. Otherwise distinct minimizers can differ in the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) while sharing the same predicted data.

For a nonnegative [convex positively one-homogeneous functional](../../../convex-optimization.md#convex-positively-one-homogeneous-functional), the branch continues as $(1-\alpha\lambda)_+u^\dagger$ above the threshold, since $p/(\alpha\lambda)\in\partial J(0)$ there. Nonnegativity is needed for that clipping argument; bare positive homogeneity allows signed linear functionals.

**Zero Bregman distance does not imply exact recovery.** For $K=I$, $J(s)=|s|$, $u^\dagger=a>0$ and $0<\alpha<a$, the minimizer is $u_\alpha=a-\alpha\ne a$, but $D_J^1(a-\alpha,a)=0$. Both points touch the same supporting line, as described by [zero Bregman distance and supporting faces](../../../inverse-problem.md#zero-bregman-distance-and-supporting-faces).

## 3

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For a [proper convex function](../../../real-analysis.md#proper-convex-function) $E$ that is [lower semicontinuous](../../../calculus.md#lower-semicontinuity) on a [Hilbert space](../../../hilbert-space.md), its [proximal operator](../../../convex-optimization.md#proximal-operator) at scale $\gamma>0$ is

$$
\boxed{\operatorname{prox}_{\gamma E}(z)=\arg\min_x\left\{\frac12\|x-z\|^2+\gamma E(x)\right\}=(I+\gamma\partial E)^{-1}z.}
$$

The minimizer is unique because the objective is [strongly convex](../../../real-analysis.md#strongly-convex-function); existence follows from the closed proper convex functional and the coercive quadratic, using an affine lower bound. The [subgradient optimality condition](../../../real-analysis.md#subgradient-optimality-condition) is $0\in x-z+\gamma\partial E(x)$, which is exactly the displayed [resolvent of a monotone operator](../../../convex-optimization.md#resolvent-of-a-monotone-operator) relation. Setting $\gamma=1$ gives the unscaled proximity or resolvent operator requested here. This is a nonlinear resolvent of the [subdifferential](../../../convex-optimization.md#subdifferential), distinct from the spectral resolvent of a linear operator.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $s=Kx$ and assume $s>0$. The scalar [Poisson data fidelity](../../../inverse-problem.md#poisson-data-fidelity) integrand has derivative $1-y/s$. Applying the permitted interchange of differentiation and integration in a direction $z$ gives

$$
\left.\frac d{d\varepsilon}E(x+\varepsilon z)\right|_{\varepsilon=0}=\int_\Sigma\left(1-\frac y{Kx}\right)Kz\,dt=\left\langle z,K^*\left(1-\frac y{Kx}\right)\right\rangle.
$$

Thus the ambient-space [Fréchet derivative](../../../calculus.md#frechet-derivative), or its [Hilbert space](../../../hilbert-space.md) gradient when the pairing is an inner product, is

$$
\boxed{E'(x)=K^*\left(1-\frac y{Kx}\right).}
$$

The quotient is pointwise, and the [adjoint operator](../../../hilbert-space.md#adjoint-operator) transports it back from the data domain to the source domain. The chosen spaces must ensure the integrals and derivative pairing are finite; an output bounded away from zero is a useful sufficient condition.

The printed set of [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) and positive cone are not vector spaces, so the notation for a bounded linear map between them is understood as a positive [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) on ambient function spaces, restricted to admissible inputs. If unit mass is a constraint, admissible directions satisfy $\int_\Omega z=0$. The displayed gradient is then a representative modulo an additive constant; optimization with that constraint additionally includes its [normal cone](../../../mathematical-optimization.md#normal-cone).

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Use the scaled [proximal operator](../../../convex-optimization.md#proximal-operator) $\operatorname{prox}_{\gamma E}$; take $\gamma=1$ for each unscaled resolvent.

For the quadratic case, write $D^TD=\operatorname{diag}(d_1,\ldots,d_n)$ and $\xi=Qx$. Since $Q$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix), the quadratic proximal term becomes $\|\xi-Qz\|^2/2$. The [subgradient optimality condition](../../../real-analysis.md#subgradient-optimality-condition) gives

$$
(I+\gamma D^TD)\xi=Qz+\gamma D^Ty.
$$

All $d_j\geq0$, so each diagonal entry is positive, including when $d_j=0$. Multiplying by the inverse [diagonal matrix](../../../linear-algebra.md#diagonal-matrix) gives

$$
\boxed{\operatorname{prox}_{\gamma E}(z)=Q^T\operatorname{diag}\left(\frac1{1+\gamma d_j}\right)(Qz+\gamma D^Ty).}
$$

The [proximal operator of Poisson data fidelity](../../../inverse-problem.md#proximal-operator-of-poisson-data-fidelity) separates pointwise. At each $t$, the scalar optimality equation on $x>0$ is

$$
x-z+\gamma\left(1-\frac yx\right)=0,\qquad x^2+(\gamma-z)x-\gamma y=0.
$$

Since $y>0$, the two roots have opposite signs. **Only the positive root is admissible** in the logarithm:

$$
\boxed{\operatorname{prox}_{\gamma E}(z)(t)=\frac{z(t)-\gamma+\sqrt{(z(t)-\gamma)^2+4\gamma y(t)}}2.}
$$

The negative root is outside the effective domain. The second derivative $1+\gamma y/x^2$ of the proximal objective is positive, establishing the unique pointwise minimizer. The integral formula is understood on the function spaces where these quantities are admissible.

Finally, for $E(x)=|x|$, positive and negative minimizers obey $x-z+\gamma=0$ and $x-z-\gamma=0$, respectively. At zero the [subdifferential](../../../convex-optimization.md#subdifferential) condition is $z\in[-\gamma,\gamma]$. Combining these cases yields [soft thresholding](../../../probability-and-statistics.md#soft-thresholding):

$$
\boxed{\operatorname{prox}_{\gamma|\cdot|}(z)=\operatorname{sgn}(z)\max\{|z|-\gamma,0\}.}
$$

Thus $\gamma=1$ supplies all three requested closed forms.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For the [convex conjugate](../../../convex-optimization.md#convex-conjugate), use a dual scalar $q$ to avoid confusing it with the fixed centre $z$. Differentiating $qx-\lambda(x-z)^2/2$ gives $q-\lambda(x-z)=0$, so the unique maximizing point is $x=z+q/\lambda$. Substitution yields

$$
\boxed{E^*(q)=qz+\frac{q^2}{2\lambda}.}
$$

The positivity of $\lambda$ makes the maximized quadratic strictly concave and the [convex conjugate](../../../convex-optimization.md#convex-conjugate) finite for every real $q$.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Take $F=(F^*)^*$ with the usual proper closed convex assumptions, so the [Fenchel-Moreau theorem](../../../convex-optimization.md#fenchel-moreau-theorem) identifies its conjugate with the supplied $F^*$. Put $z^k=u^k-\tau D^Tv^k$. The first update is $w^{k+1}=\operatorname{prox}_{F^*/\tau}(z^k/\tau)$. By [Moreau decomposition](../../../convex-optimization.md#moreau-decomposition), the second update is

$$
u^{k+1}=z^k-\tau\operatorname{prox}_{F^*/\tau}(z^k/\tau)=\operatorname{prox}_{\tau F}(z^k).
$$

Also $\tau(D^Tv^k+w^{k+1})=u^k-u^{k+1}$, so the argument in the final update contains $u^{k+1}-\tau(D^Tv^k+w^{k+1})=2u^{k+1}-u^k$. Eliminating the auxiliary variable gives

$$
\boxed{\begin{aligned}
u^{k+1}&=\operatorname{prox}_{\tau F}(u^k-\tau D^Tv^k),\\
v^{k+1}&=\operatorname{prox}_{\sigma G}\left(v^k+\sigma D(2u^{k+1}-u^k)\right).
\end{aligned}}
$$

This is the [primal-dual hybrid gradient method](../../../convex-optimization.md#chambolle-pock-algorithm) with extrapolation parameter one and the primal update performed first. Its [saddle point](../../../analysis.md#saddle-point) function is $F(u)+\langle Du,v\rangle-G(v)$, corresponding to the primal objective $F(u)+G^*(Du)$.

For proper [lower semicontinuous](../../../calculus.md#lower-semicontinuity) [convex functions](../../../real-analysis.md#convex-function) and a nonempty saddle-point set in these finite-dimensional spaces, the standard [convergence of primal-dual hybrid gradient](../../../convex-optimization.md#convergence-of-primal-dual-hybrid-gradient) theorem gives the sufficient parameter condition

$$
\boxed{\tau>0,\qquad\sigma>0,\qquad\tau\sigma\|D\|_2^2<1.}
$$

Here $\|D\|_2$ is the [operator norm](../../../continuous-dual-space.md#operator-norm), or largest [singular value](../../../linear-algebra.md#singular-value). For $D\ne0$, one possible choice is $\tau=\sigma=\eta/\|D\|_2$ with $0<\eta<1$; for $D=0$ any positive steps satisfy the condition. The existence assumption is necessary: step sizes alone cannot guarantee convergence to a saddle point that does not exist.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
