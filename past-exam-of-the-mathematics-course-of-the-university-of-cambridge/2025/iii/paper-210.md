# Paper 210

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_210.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_210.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Writing $P_ng=n^{-1}\sum_{i=1}^ng(X_i)$ and $Pg=\mathbb Eg(X)$, the class $\mathcal G$ satisfies a [uniform law of large numbers](../../../convergence-of-random-variables.md#uniform-law-of-large-numbers) when

$$
\sup_{g\in\mathcal G}|P_ng-Pg|\longrightarrow0
$$

in probability; a strong ULLN uses almost-sure convergence.

Fix $\varepsilon>0$ and choose finitely many brackets $[g_j^L,g_j^U]$ of $L^1(P)$ width at most $\varepsilon$. The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers), simultaneously for their finitely many endpoints, gives

$$
\max_j\{|P_ng_j^L-Pg_j^L|,|P_ng_j^U-Pg_j^U|\}\to0.
$$

If $g_j^L\leq g\leq g_j^U$, bracketing both $P_ng$ and $Pg$ shows

$$
|P_ng-Pg|\leq\max\{|P_ng_j^L-Pg_j^L|,
|P_ng_j^U-Pg_j^U|\}+P(g_j^U-g_j^L).
$$

Taking the supremum gives a limit superior at most $\varepsilon$. Since $\varepsilon$ is arbitrary, the ULLN follows.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Glivenko-Cantelli theorem](../../../convergence-of-random-variables.md#glivenko-cantelli-theorem) states that for the empirical distribution function $F_n$ of iid real observations with distribution function $F$,

$$
\sup_{t\in\mathbb R}|F_n(t)-F(t)|\longrightarrow0
$$

almost surely.

Apply part (a) to $\mathcal G=\{\mathbf1_{(-\infty,t]}:t\in\mathbb R\}$. For each $\varepsilon>0$, choose finitely many quantile cutpoints so that the $P$-mass between consecutive cutpoints is at most $\varepsilon$, treating atoms as cutpoints themselves. Indicators at adjacent cutpoints give finite $L^1(P)$ brackets of width at most $\varepsilon$. Using the strong law for the finite bracket endpoints and then intersecting the probability-one events for $\varepsilon=1/m$ gives the almost-sure conclusion.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**No.** For each realized sample let $A_n=\{X_1,\ldots,X_n\}$. This is a finite Borel set, and continuity of $F$ makes $P(A_n)=0$ almost surely, while $P_n(A_n)=1$. Therefore

$$
\sup_{A\in\mathcal B(\mathbb R)}|P_n(A)-P(A)|=1
$$

almost surely for every $n$, so the class of all Borel-set indicators cannot satisfy a ULLN.

## 2

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) is an integrable function $K$ with $\int K=1$, usually also bounded and nonnegative, and its scaled version is $K_h(u)=h^{-1}K(u/h)$. For suitable $g_1,g_2$, their [convolution](../../../fourier-analysis.md#convolution) is

$$
(g_1*g_2)(x)=\int_{\mathbb R}g_1(x-u)g_2(u)du.
$$

Because the observations have length-biased density $g(u)=uf(u)/\mu$,

$$
\mathbb E\widehat f_n(x)
=\frac\mu h\int_0^\infty\frac1uK\left(\frac{x-u}{h}\right)
\frac{uf(u)}\mu du
=(K_h*f)(x).
$$

Thus the exact bias is $(K_h*f)(x)-f(x)$, exactly the same as for the ordinary [kernel density estimator](../../../nonparametric-statistics.md#kernel-density-estimation) based directly on observations from $f$.

Write $R(K)=\int K(u)^2du$. The estimator is the average of $Y_i(x)=\mu X_i^{-1}K_h(x-X_i)$, so

$$
\int\mathbb EY_i(x)^2dx
=\mu^2\mathbb E_g(X_i^{-2})\int K_h^2
=\frac{\mu\bar\mu R(K)}h.
$$

Its mean is $K_h*f$. Integrating the pointwise variance therefore gives

$$
\int\operatorname{Var}\widehat f_n(x)dx
=\frac{\mu\bar\mu R(K)}{nh}
-\frac1n\int(K_h*f)(x)^2dx.
$$

Finally, [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) under density $f$ gives

$$
\mu\bar\mu=\mathbb E_fX\,\mathbb E_f(X^{-1})
\geq(\mathbb E_f1)^2=1.
$$

Equality would require $X$ to be constant almost surely, impossible for a density, so $\mu\bar\mu>1$. The ordinary KDE has the same negative term but leading integrated variance $R(K)/(nh)$; length-biased sampling strictly inflates it.

## 3

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $r=\lceil\beta\rceil-1$. The [Hölder class](../../../sobolev-space.md#holder-class) $\mathcal H(\beta,L)$ consists of functions with $r$ continuous derivatives whose $r$th derivative satisfies

$$
|m^{(r)}(x)-m^{(r)}(y)|\leq L|x-y|^{\beta-r},
$$

with the equivalent Lipschitz convention when $\beta$ is an integer.

The degree-$p$ [local polynomial regression](../../../nonparametric-statistics.md#local-polynomial-regression) estimator minimizes

$$
\sum_{i=1}^nK_h(x_i-x)
\left[Y_i-\sum_{j=0}^pb_j\frac{(x_i-x)^j}{j!}\right]^2
$$

and takes $\widehat m_n(x;p,h)=\widehat b_0$. Put $X_i^T=Q((x_i-x)/h)^T$, $W_{ii}=K_h(x_i-x)$, and rescale $b_j$ by $h^j$. If $X^TWX$ is positive definite, weighted least squares gives

$$
\widehat b=(X^TWX)^{-1}X^TWY,
\qquad
\widehat m_n=e_0^T\widehat b.
$$

Define

$$
w_i(x)=e_0^T\left(\frac1nX^TWX\right)^{-1}X_iW_{ii}.
$$

Then $\widehat m_n=n^{-1}\sum_iw_iY_i$. If $R$ has degree at most $p$, fitting the noiseless response $R(x_i)$ reproduces that polynomial exactly, and hence

$$
\frac1n\sum_iw_i(x)R(x_i)=R(x).
$$

For nonzero $a$, the polynomial $a^TQ(u)$ cannot vanish throughout $[0,1]$. Therefore

$$
a^T\left(\int_0^1Q(u)Q(u)^Tdu\right)a>0,
$$

and compactness of the unit sphere makes its minimum eigenvalue $\Lambda_p$ positive. Choose $a(p)$ and $n_0(p)$ so that $nh\geq a(p)$ makes the supplied lower bound on $\lambda_0$ at least $\Lambda_p/4$. On the kernel support, $Q$ is bounded by a constant depending only on $p$, and $K_h\leq1/(2h)$. It follows that only $O(nh)$ weights are nonzero and

$$
|w_i(x)|\leq C_p/h,
\quad
\frac1{n^2}\sum_iw_i(x)^2\leq\frac{C_p}{nh},
\quad
\frac1n\sum_i|w_i(x)|\leq C_p.
$$

Polynomial reproduction cancels the Taylor polynomial of degree $r\leq p$. The Hölder remainder on $|x_i-x|\leq h$ is at most $C_pLh^\beta$, so the squared bias is at most $C_pL^2h^{2\beta}$. Independence and $\operatorname{Var}\varepsilon_i\leq\sigma^2$ bound the variance by $C_p\sigma^2/(nh)$. Combining them uniformly in $x$ and $m$ proves

$$
\boxed{\sup_{x\in[0,1]}\sup_{m\in\mathcal H(\beta,L)}
\mathbb E(\widehat m_n(x;p,h)-m(x))^2
\leq C(p)\left(\frac{\sigma^2}{nh}+L^2h^{2\beta}\right).}
$$

## 4

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

With densities $p,q$,

$$
\operatorname{TV}(P,Q)=\frac12\int|p-q|d\mu,
\qquad
H(P,Q)^2=\int(\sqrt p-\sqrt q)^2d\mu.
$$

By [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality),

$$
\operatorname{TV}(P,Q)
\leq\frac12H(P,Q)
\left(\int(\sqrt p+\sqrt q)^2d\mu\right)^{1/2}
\leq H(P,Q).
$$

Also $(\sqrt p-\sqrt q)^2\leq|p-q|$, so $H^2\leq2\operatorname{TV}$.

The Hellinger affinity is $\rho(P,Q)=\int\sqrt{pq}\,d\mu=1-H^2/2$. Product densities and [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) give $\rho(P^n,Q^n)=\rho(P,Q)^n$, hence

$$
H^2(P^n,Q^n)=2-2\left(1-\frac12H^2(P,Q)\right)^n.
$$

[Le Cam two-point lemma](../../../statistical-inference.md#le-cam-two-point-lemma) states, for squared-error estimation at parameter points $\theta_0,\theta_1$, that

$$
\inf_{\widehat\theta}\max_{j=0,1}
\mathbb E_j(\widehat\theta-\theta_j)^2
\geq\frac{(\theta_1-\theta_0)^2}{8}
\left(1-\operatorname{TV}(P_0,P_1)\right).
$$

Take $\theta_0=0$, $\theta_1=\delta=1/(4n)$. The one-observation uniform densities overlap on length $1-\delta$, so $H^2(P_0,P_1)=2\delta$. Therefore

$$
H^2(P_0^n,P_1^n)
=2-2(1-\delta)^n\leq2n\delta=\frac12.
$$

The first distance inequality gives $\operatorname{TV}(P_0^n,P_1^n)\leq1/\sqrt2$. Le Cam's lemma now yields

$$
\inf_{\widehat\theta}\sup_{\theta\in\mathbb R}
\mathbb E_\theta(\widehat\theta-\theta)^2
\geq\frac{1-1/\sqrt2}{128n^2}.
$$

This proves the claim with the displayed universal positive constant.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
