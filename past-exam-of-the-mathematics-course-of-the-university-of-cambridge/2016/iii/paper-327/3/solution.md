<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

With $\langle\theta\rangle=(1+|\theta|^2)^{1/2}$, the [symbol class](../../../../../symbol-class.md) $\operatorname{Sym}(X,\mathbb R^k;N)=S^N_{1,0}$ consists of complex-valued $a\in C^\infty(X\times\mathbb R^k)$ such that, for every compact $K\Subset X$ and every pair of [multi-indices](../../../../../multi-index-notation.md) $\alpha,\beta$,

$$
\boxed{|\partial_x^\alpha\partial_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|},\qquad x\in K.}
$$

An $x$ derivative preserves symbol order, while a $\theta$ derivative lowers it by one. The definition is local in $x$ and imposes estimates of every derivative order.

In the homogeneous convention, a [phase function](../../../../../phase-function.md) is real, smooth on $X\times(\mathbb R^k\setminus\{0\})$, positively homogeneous of degree one in $\theta$, and satisfies

$$
(\nabla_x\Phi,\nabla_\theta\Phi)\ne0\quad(\theta\ne0).
$$

Only the large-frequency behavior is relevant to the regularization argument; any prescribed smooth modification near $\theta=0$ contributes an ordinary convergent integral. If the phase is presented on all of $X\times\mathbb R^k$, homogeneity can be required outside a bounded frequency region. Equivalently for this construction, its large-frequency symbol bounds and the following uniform estimate are sufficient:

$$
|\nabla_x\Phi|^2+|\theta|^2|\nabla_\theta\Phi|^2\geq c_K|\theta|^2,\qquad x\in K,\ |\theta|\geq1.
$$

For a homogeneous [phase function](../../../../../phase-function.md), this follows from compactness of $K\times S^{k-1}$. **Nonvanishing of the total gradient is the condition; $\nabla_\theta\Phi$ may vanish.** The displayed definition does not impose the stronger rank condition sometimes called a nondegenerate phase in Fourier-integral-operator theory.

We construct the [oscillatory integral](../../../../../oscillatory-integral.md) by [integration by parts](../../../../../integration-by-parts.md) in both $x$ and $\theta$. For $|\theta|\geq1$, set

$$
q=|\nabla_x\Phi|^2+|\theta|^2|\nabla_\theta\Phi|^2,\qquad
L=\frac1{iq}\left(\nabla_x\Phi\cdot\nabla_x+|\theta|^2\nabla_\theta\Phi\cdot\nabla_\theta\right).
$$

Then $L(e^{i\Phi})=e^{i\Phi}$. The coefficients of the $x$ derivatives have symbol order $-1$ and those of the $\theta$ derivatives have order zero. Use the bilinear [formal transpose of a differential operator](../../../../../formal-transpose-of-a-differential-operator.md), not the Hermitian adjoint:

$$
L^tb=-\sum_j\partial_{x_j}\left(\frac{\partial_{x_j}\Phi}{iq}b\right)
-\sum_\ell\partial_{\theta_\ell}\left(\frac{|\theta|^2\partial_{\theta_\ell}\Phi}{iq}b\right).
$$

The [symbol order reduction by a phase integration operator](../../../../../symbol-order-reduction-by-a-phase-integration-operator.md) follows from the product rule and the [symbol class](../../../../../symbol-class.md) estimates: $L^t:S^s_{1,0}\to S^{s-1}_{1,0}$ locally in $x$. Differentiating the coefficients preserves precisely these orders because $q$ is elliptic of degree two on each compact $x$ set.

Let $\zeta\in C_c^\infty(\mathbb R^k)$ equal one on $|\theta|\leq1$ and vanish on $|\theta|\geq2$. The low-frequency part is an ordinary integral. For an integer $r>N+k$, define the high-frequency part by

$$
\begin{aligned}
\langle I_\Phi(a),\varphi\rangle={}&\iint e^{i\Phi}\zeta(\theta)a(x,\theta)\varphi(x)\,dx\,d\theta\\
&+\iint e^{i\Phi}(L^t)^r\big[(1-\zeta(\theta))a(x,\theta)\varphi(x)\big]\,dx\,d\theta.
\end{aligned}
$$

If the homogeneous phase is only defined off zero, its value at the single point zero is immaterial to the low-frequency integral; its modulus remains one. In the high-frequency term all coefficients are used away from zero. For $\operatorname{supp}\varphi\subset K$, repeated product rules give

$$
\left|(L^t)^r[(1-\zeta)a\varphi]\right|
\leq C_{K,a,\Phi,r}\langle\theta\rangle^{N-r}
\max_{|\alpha|\leq r}\sup_K|\partial^\alpha\varphi|.
$$

Since $N-r<-k$, both terms converge absolutely. They are linear in the [test function](../../../../../test-function.md), with the continuity bound

$$
\boxed{|\langle I_\Phi(a),\varphi\rangle|
\leq C_K\max_{|\alpha|\leq r}\sup_K|\partial^\alpha\varphi|.}
$$

Thus **$I_\Phi(a)\in\mathcal D'(X)$**, with [order of a distribution](../../../../../order-of-a-distribution.md) at most $r$ on each compact set.

To check that this construction is the intended [oscillatory integral](../../../../../oscillatory-integral.md) and does not depend on $r$, $\zeta$ or the large-frequency cutoff, let $\chi\in C_c^\infty(\mathbb R^k)$ equal one near zero and form

$$
J_R(\varphi)=\iint e^{i\Phi(x,\theta)}a(x,\theta)\varphi(x)\chi(\theta/R)\,dx\,d\theta.
$$

After $r$ applications of [integration by parts](../../../../../integration-by-parts.md), the term without a derivative on $\chi$ tends to the absolutely convergent high-frequency term by the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md). Each extra term is supported in an annulus $|\theta|\asymp R$. A derivative of $\chi(\theta/R)$ contributes $R^{-1}$, so those terms have total absolute value at most $C_KR^{N-r+k}\max_{|\alpha|\leq r}\|\partial^\alpha\varphi\|_\infty\to0$. The low-frequency part is unchanged for large $R$. Hence $J_R(\varphi)$ tends to the displayed functional, independently of all cutoffs and of the permissible number of integrations. This proves the [cutoff independence of an oscillatory integral](../../../../../cutoff-independence-of-an-oscillatory-integral.md) as well as its continuity.

For the final [distribution](../../../../../distribution-mathematical-analysis.md), the derivative convention $\langle\delta',g\rangle=-g'(0)$ identifies it as $-x_2\delta'(x_1)$. The [delta derivatives from polynomial oscillatory amplitudes](../../../../../delta-derivatives-from-polynomial-oscillatory-amplitudes.md) identity yields

$$
\boxed{\Phi(x,\theta)=x_1\theta,\qquad
a(x,\theta)=-\frac{i}{2\pi}x_2\theta,\qquad
u=I_\Phi(a)=-\frac{i x_2}{2\pi}\int_{\mathbb R}e^{ix_1\theta}\theta\,d\theta.}
$$

Here $k=1$, $a\in\operatorname{Sym}(\mathbb R^2,\mathbb R;1)$, and $\nabla_x\Phi=(\theta,0)$ is nonzero for $\theta\ne0$. Thus the phase is admissible even though $\partial_\theta\Phi=x_1$ vanishes on the [distribution](../../../../../distribution-mathematical-analysis.md)'s support.

For a direct proof of the sign and normalization, put $g(s)=\int_{\mathbb R}x_2\varphi(s,x_2)\,dx_2\in C_c^\infty(\mathbb R)$. The cutoff integral is

$$
J_R(\varphi)=-\frac{i}{2\pi}\int\theta\chi(\theta/R)\widehat g(-\theta)\,d\theta
=\frac{i}{2\pi}\int\xi\chi(-\xi/R)\widehat g(\xi)\,d\xi.
$$

The [Fourier transform](../../../../../fourier-transform.md) $\widehat g$ is rapidly decreasing, so the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) and differentiated [Fourier inversion](../../../../../fourier-inversion-theorem.md) give

$$
\lim_{R\to\infty}J_R(\varphi)=g'(0)
=\int_{\mathbb R}x_2\frac{\partial\varphi}{\partial x_1}(0,x_2)\,dx_2.
$$

This is exactly the required pairing, so the oscillatory representation gives the prescribed [distribution](../../../../../distribution-mathematical-analysis.md), not its negative or a multiple of it.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
