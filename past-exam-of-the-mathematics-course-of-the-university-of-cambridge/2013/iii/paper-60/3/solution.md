<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [oscillatory integral](../../../../../oscillatory-integral.md) defines a [distribution](../../../../../distribution-mathematical-analysis.md) by cancellation, even when its [oscillatory integral amplitude](../../../../../amplitude-of-an-oscillatory-integral.md) is not integrable in frequency. We use [symbol class](../../../../../symbol-class.md) $\operatorname{Sym}(X,\mathbb R^k;N)=S^N_{1,0}(X\times\mathbb R^k)$, where $X\subset\mathbb R^d$ is open and $N\in\mathbb R$. An [oscillatory integral amplitude](../../../../../amplitude-of-an-oscillatory-integral.md) $a$ belongs to this class if it is smooth and, for every [compact set](../../../../../compact-space.md) $K\subset X$ and all [multi-indices](../../../../../multi-index-notation.md) $\alpha,\beta$,

$$
|\partial_x^\alpha\partial_\theta^\beta a(x,\theta)|\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|},
\qquad x\in K,\quad\langle\theta\rangle=(1+|\theta|^2)^{1/2}.
$$

In [symbol calculus](../../../../../symbol-calculus.md), spatial derivatives preserve the order and frequency derivatives lower it. The fixed number $N$ is independent of $K$; this will produce a finite global [order of a distribution](../../../../../order-of-a-distribution.md), although continuity constants may depend on $K$.

A [phase function](../../../../../phase-function.md) $\Phi$ is real and smooth on $X\times(\mathbb R^k\setminus\{0\})$, is positively homogeneous of degree one in $\theta$, and has nonzero total differential there:

$$
\Phi(x,r\theta)=r\Phi(x,\theta)\ (r>0),\qquad
(\nabla_x\Phi,\nabla_\theta\Phi)\ne0\quad(\theta\ne0).
$$

This [positive homogeneity](../../../../../positively-homogeneous-function-degree-one.md) is required at nonzero frequency; arbitrary smooth low-frequency modifications give the equivalent version homogeneous only for large $|\theta|$. In particular, smoothness at zero is not an additional requirement on a general homogeneous [phase function](../../../../../phase-function.md). The integral over bounded frequencies is a [smooth function](../../../../../smooth-function.md) of $x$: spatial derivatives of the phase have size $O(|\theta|)$ near zero, uniformly on compact spatial sets and frequency directions.

Choose a [cutoff function](../../../../../cutoff-function.md) $\chi\in C_c^\infty(\mathbb R^k)$ equal to one near zero. The proposed meaning of the [oscillatory integral distribution](../../../../../oscillatory-integral.md) is

$$
\langle I_\Phi(a),\varphi\rangle
=\lim_{R\to\infty}\int_X\int_{\mathbb R^k}e^{i\Phi(x,\theta)}a(x,\theta)\varphi(x)\chi(\theta/R)\,d\theta\,dx,
\qquad\varphi\in\mathcal D(X).
$$

Existence and [cutoff independence of an oscillatory integral](../../../../../cutoff-independence-of-an-oscillatory-integral.md) require a proof. Split $a=a_0+a_\infty$ using a fixed frequency [cutoff function](../../../../../cutoff-function.md), with $a_0$ supported in a bounded ball and $a_\infty$ zero for $|\theta|\leq1$. The low-frequency part is already absolutely integrable. On nonzero frequency set

$$
q=|\nabla_x\Phi|^2+|\theta|^2|\nabla_\theta\Phi|^2,\qquad
L=\frac1{iq}\left(\nabla_x\Phi\cdot\nabla_x+|\theta|^2\nabla_\theta\Phi\cdot\nabla_\theta\right).
$$

The [positive homogeneity](../../../../../positively-homogeneous-function-degree-one.md) and nonvanishing total differential of the [phase function](../../../../../phase-function.md) imply $q\geq c_K|\theta|^2$ for $x\in K$: normalize to the compact [unit sphere](../../../../../unit-sphere.md) in frequency. Direct differentiation gives $Le^{i\Phi}=e^{i\Phi}$.

The $x$ coefficients of $L$ have [symbol class](../../../../../symbol-class.md) order $-1$, and its frequency coefficients have order zero. If these coefficients are $A_j$ and $B_\ell$, the [formal transpose of a differential operator](../../../../../formal-transpose-of-a-differential-operator.md) is

$$
L^tb=-\sum_j\partial_{x_j}(A_jb)-\sum_\ell\partial_{\theta_\ell}(B_\ell b).
$$

Thus the [symbol order reduction by a phase integration operator](../../../../../symbol-order-reduction-by-a-phase-integration-operator.md) is $L^t:S^s_{1,0}\to S^{s-1}_{1,0}$: the first sum has an order-$-1$ coefficient, and the second contains a frequency derivative. In applying this to $a_\infty\varphi$, every application also differentiates $\varphi$ at most once. Repeated [integration by parts](../../../../../integration-by-parts.md), in both $x$ and $\theta$, consequently gives for an integer $m>N+k$

$$
\int\!\int e^{i\Phi}a_\infty\varphi\chi(\theta/R)\,d\theta\,dx
=\int\!\int e^{i\Phi}(L^t)^m\big(a_\infty\varphi\chi(\theta/R)\big)\,d\theta\,dx.
$$

There are no spatial boundary terms because $\varphi$ has [compact support](../../../../../compact-support.md), and the frequency cutoff removes frequency boundary terms. Derivatives of $\chi(\theta/R)$ are bounded uniformly by constants times $\langle\theta\rangle^{-|\beta|}$ on their annular support. The transformed integrand is therefore bounded in absolute value by

$$
C_K\langle\theta\rangle^{N-m}\max_{|\alpha|\leq m}\|\partial^\alpha\varphi\|_\infty.
$$

This is integrable in $k$ frequency dimensions. Pointwise the transformed integrand tends to $(L^t)^m(a_\infty\varphi)$, so the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) establishes

$$
\langle I_\Phi(a),\varphi\rangle
=\int\!\int e^{i\Phi}a_0\varphi\,d\theta\,dx
+\int\!\int e^{i\Phi}(L^t)^m(a_\infty\varphi)\,d\theta\,dx.
$$

The limit is independent of the expanding cutoff, the fixed splitting cutoff, and the admissible $m$, since each formula is the limit of the same truncated integral. Derivatives landing on the expanding cutoff can also be estimated directly by $O(R^{N-m+k})$, which tends to zero. In particular,

$$
\boxed{|\langle I_\Phi(a),\varphi\rangle|\leq C_K\max_{|\alpha|\leq m}\|\partial^\alpha\varphi\|_\infty,
\quad m\in\mathbb Z_{\geq0},\quad m>N+k.}
$$

This proves continuity on the [space of test functions](../../../../../space-of-test-functions.md) and the [finite order of an oscillatory integral distribution](../../../../../finite-order-of-an-oscillatory-integral-distribution.md). The same $m$ works for all [compact sets](../../../../../compact-space.md). When $N<-k$, $m=0$ is possible and the original frequency integral is absolutely integrable; cancellation is needed for general $N$.

The [singular support](../../../../../singular-support.md) theorem states that

$$
\boxed{\operatorname{sing\,supp}I_\Phi(a)\subset
\{x\in X:\text{some }\theta\ne0\text{ satisfies }\nabla_\theta\Phi(x,\theta)=0\}.}
$$

By [positive homogeneity](../../../../../positively-homogeneous-function-degree-one.md), frequencies can be restricted to the [unit sphere](../../../../../unit-sphere.md), so this projected set is closed locally in $X$. More precisely, the [stationary-direction bound for singular support](../../../../../stationary-direction-bound-for-singular-support.md) restricts the frequency directions to the closed [conic support of an oscillatory amplitude](../../../../../conic-support-of-an-oscillatory-amplitude.md); using a closed directional support avoids losing limits occurring at arbitrarily high frequency. The simpler displayed bound is sufficient here.

To prove the bound, take $x_0$ outside the displayed stationary set. On a sufficiently small spatial neighborhood and all unit frequency directions, $|\nabla_\theta\Phi|$ is bounded below. The frequency-only operator

$$
L_\theta=\frac{\nabla_\theta\Phi\cdot\nabla_\theta}{i|\nabla_\theta\Phi|^2}
$$

satisfies $L_\theta e^{i\Phi}=e^{i\Phi}$, and its [formal transpose](../../../../../formal-transpose-of-a-differential-operator.md) lowers [symbol class](../../../../../symbol-class.md) order by one. A spatial derivative of order $|\alpha|$ of $e^{i\Phi}a$ has amplitude order at most $N+|\alpha|$. Applying the frequency [integration by parts](../../../../../integration-by-parts.md) more than $N+|\alpha|+k$ times makes that derivative absolutely integrable, uniformly on smaller [compact sets](../../../../../compact-space.md). Every spatial derivative therefore exists and is continuous there. The [oscillatory integral distribution](../../../../../oscillatory-integral.md) is a [smooth function](../../../../../smooth-function.md) near $x_0$, proving the [singular support](../../../../../singular-support.md) assertion.

For the [linear transport equation](../../../../../linear-transport-equation.md), use spacetime $X=\mathbb R^n\times(0,\infty)$, frequency $\theta\in\mathbb R^n$, and

$$
\Phi(x,t,\theta)=(x-ct)\cdot\theta,\qquad a=(2\pi)^{-n}.
$$

This is a valid [phase function](../../../../../phase-function.md), because $\nabla_x\Phi=\theta\ne0$ at nonzero frequency; the [oscillatory integral amplitude](../../../../../amplitude-of-an-oscillatory-integral.md) is in [symbol class](../../../../../symbol-class.md) order zero. The [Fourier representation of the Dirac delta function](../../../../../fourier-representation-of-the-dirac-delta-function.md) gives the [transport of a Dirac point mass](../../../../../transport-of-a-dirac-point-mass.md):

$$
\boxed{u(x,t)=\frac1{(2\pi)^n}\int e^{i(x-ct)\cdot\theta}\,d\theta=\delta_0(x-ct).}
$$

Its rigorous spacetime [distribution](../../../../../distribution-mathematical-analysis.md) pairing is $\langle u,\varphi\rangle=\int_0^\infty\varphi(ct,t)\,dt$. Consequently

$$
\langle(\partial_t+c\cdot\nabla_x)u,\varphi\rangle
=-\int_0^\infty\frac d{dt}\varphi(ct,t)\,dt=0,
$$

where the endpoints vanish since a spacetime [test function](../../../../../test-function.md) has [compact support](../../../../../compact-support.md) in $t>0$. At each fixed $t$, $\langle u(t),\psi\rangle=\psi(ct)$, so [weak convergence of distributions](../../../../../weak-convergence-of-distributions.md) gives $u(t)\to\delta_0$ as $t\downarrow0$. This is the required initial trace.

Finally, $\nabla_\theta\Phi=x-ct$, so the [singular support](../../../../../singular-support.md) theorem confines singularities to $x=ct$. In fact equality holds: $u$ is a nonzero order-zero [distribution](../../../../../distribution-mathematical-analysis.md) on that trajectory and vanishes off it. A [smooth function](../../../../../smooth-function.md) supported on this set of empty interior must vanish, so $u$ cannot be smooth in any neighborhood of a point of the trajectory. Thus

$$
\boxed{\operatorname{sing\,supp}u=\{(ct,t):t>0\}.}
$$

The [method of characteristics](../../../../../method-of-characteristics.md) also proves uniqueness among solutions with a distributional initial trace: the [change of variables](../../../../../change-of-variables-formula.md) $y=x-ct$ turns the [linear transport equation](../../../../../linear-transport-equation.md) into $\partial_t w=0$. Such a [distribution](../../../../../distribution-mathematical-analysis.md) is constant in $t$; pairing with spatial [test functions](../../../../../test-function.md) reduces this assertion to [a distribution with zero derivative is constant](../../../../../a-distribution-with-zero-derivative-is-constant.md). Its initial trace fixes $w=\delta_0$, so the moving [Dirac delta distribution](../../../../../dirac-delta-function.md) above is the unique solution. There is transport of the singularity along the characteristic and no smoothing.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
