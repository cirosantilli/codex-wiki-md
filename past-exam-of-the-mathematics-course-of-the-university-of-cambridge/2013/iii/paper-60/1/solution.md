<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [space of test functions](../../../../../space-of-test-functions.md) is $\mathcal D(\mathbb R)=C_c^\infty(\mathbb R)$: its elements are [smooth functions](../../../../../smooth-function.md) with [compact support](../../../../../compact-support.md). For a fixed [compact set](../../../../../compact-space.md) $K$, put $\mathcal D_K=\{\varphi\in C^\infty(\mathbb R):\operatorname{supp}\varphi\subset K\}$ and use the [seminorms](../../../../../seminorm.md) $p_m(\varphi)=\max_{0\leq j\leq m}\|\varphi^{(j)}\|_\infty$. The [space of test functions](../../../../../space-of-test-functions.md) carries the usual [test-function inductive limit topology](../../../../../test-function-inductive-limit-topology.md) of these spaces. In particular, **a sequence converges precisely when its supports eventually lie in one compact set and every [derivative](../../../../../derivative.md) converges uniformly**. Thus $\varphi_j\to\varphi$ means that a common $K$ contains their supports and $p_m(\varphi_j-\varphi)\to0$ for every $m$.

A [distribution](../../../../../distribution-mathematical-analysis.md) is a [continuous linear functional](../../../../../continuous-linear-functional.md) on this [space of test functions](../../../../../space-of-test-functions.md), and $\mathcal D'(\mathbb R)$ denotes their space. We use complex-linear, bilinear pairings $\langle u,\varphi\rangle$. Equivalently, for every [compact set](../../../../../compact-space.md) $K$ there are $C_K$ and a nonnegative integer $m_K$ such that

$$
|\langle u,\varphi\rangle|\leq C_Kp_{m_K}(\varphi),\qquad \varphi\in\mathcal D_K.
$$

The usual [weak convergence of distributions](../../../../../weak-convergence-of-distributions.md) is $u_j\to u$ if $\langle u_j,\varphi\rangle\to\langle u,\varphi\rangle$ for every [test function](../../../../../test-function.md). This specifies the convergence used below; it does not require convergence in any norm.

The [distributional derivative](../../../../../distributional-derivative.md) is defined by

$$
\boxed{\langle u',\varphi\rangle=-\langle u,\varphi'\rangle.}
$$

The [derivative](../../../../../derivative.md) map sends $\mathcal D_K$ continuously to itself, with $p_m(\varphi')\leq p_{m+1}(\varphi)$. The preceding continuity estimate therefore proves that $u'$ is again a [distribution](../../../../../distribution-mathematical-analysis.md). This definition extends the ordinary [derivative](../../../../../derivative.md) of a [smooth function](../../../../../smooth-function.md), by [integration by parts](../../../../../integration-by-parts.md).

Choose the [translation of a distribution](../../../../../translation-of-a-distribution.md) convention $\tau_hf(x)=f(x-h)$. Its action on a [test function](../../../../../test-function.md) is

$$
\langle\tau_hu,\varphi\rangle=\langle u,\varphi(\mathord\cdot+h)\rangle.
$$

For fixed $h$, the translated [test functions](../../../../../test-function.md) have translated [compact support](../../../../../compact-support.md) and unchanged derivative sup norms, so this defines a [distribution](../../../../../distribution-mathematical-analysis.md). For the [differentiability of distribution translations](../../../../../differentiability-of-distribution-translations.md), apply the [Taylor theorem](../../../../../taylor-theorem.md) in integral form:

$$
\frac{\varphi(x-h)-\varphi(x)}h=-\int_0^1\varphi'(x-sh)\,ds\longrightarrow-\varphi'(x)
\quad\text{in }\mathcal D(\mathbb R).
$$

All supports lie in one slightly enlarged [compact set](../../../../../compact-space.md) for $|h|\leq1$, and the same identity for every [derivative](../../../../../derivative.md) proves [uniform convergence](../../../../../uniform-convergence.md). The continuity of $u$ now gives

$$
\boxed{\lim_{h\to0}\frac{\tau_{-h}u-u}{h}=u'\quad\text{in }\mathcal D'(\mathbb R).}
$$

The minus sign in the translation parameter is necessary for this convention.

For (a), choose a [test function](../../../../../test-function.md) $\eta$ with $\int\eta=1$. If $\int\psi=0$, then $F(x)=\int_{-\infty}^x\psi(s)\,ds$ is a [test function](../../../../../test-function.md), since the zero integral makes it vanish beyond both ends of the [compact support](../../../../../compact-support.md). If $u_1'=0$, then $\langle u_1,\psi\rangle=\langle u_1,F'\rangle=0$. Decompose $\varphi=(\int\varphi)\eta+\psi$ to obtain

$$
\boxed{u_1=C\quad(C\in\mathbb C),\qquad \langle u_1,\varphi\rangle=C\int\varphi.}
$$

Conversely, these constant [regular distributions](../../../../../regular-distribution.md) have zero [distributional derivative](../../../../../distributional-derivative.md). This also proves the general fact that [a distribution with zero derivative is constant](../../../../../a-distribution-with-zero-derivative-is-constant.md).

For (b), choose a [cutoff function](../../../../../cutoff-function.md) $\rho$ equal to one near zero. Every [test function](../../../../../test-function.md) decomposes as

$$
\varphi(x)=\varphi(0)\rho(x)+x\psi(x),\qquad
\psi(x)=\frac{\varphi(x)-\varphi(0)\rho(x)}x\in\mathcal D(\mathbb R).
$$

The quotient extends as a [smooth function](../../../../../smooth-function.md) at zero, and it has [compact support](../../../../../compact-support.md). If $xu_2=0$, the definition of [multiplication of a distribution by a smooth function](../../../../../multiplication-of-a-distribution-by-a-smooth-function.md) gives $\langle u_2,\varphi\rangle=\langle u_2,\rho\rangle\varphi(0)$. Conversely, $x\delta_0=0$. Thus the [kernel of multiplication by a coordinate](../../../../../kernel-of-multiplication-by-a-coordinate.md) is exactly

$$
\boxed{u_2=C\delta_0.}
$$

In particular, derivatives of the [Dirac delta distribution](../../../../../dirac-delta-function.md) are not additional solutions: $x\delta_0'=-\delta_0$.

Now write $D=d/dx$ and $P(z)=-z^n+\sum_{j=0}^{n-1}a_jz^j$, where $n\geq1$. The [characteristic roots of a constant-coefficient differential equation](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) are the distinct [roots of a polynomial](../../../../../root-of-a-polynomial.md) $\lambda_1,\ldots,\lambda_r$ of $P$, with multiplicities $m_1,\ldots,m_r$. The [distributional regularity of a constant-coefficient ordinary differential equation](../../../../../distributional-regularity-of-a-constant-coefficient-ordinary-differential-equation.md) can be proved without assuming regularity in advance. Put $q_j(z)=(z-\lambda_j)^{m_j}$ and $Q=\prod_jq_j=-P$. Since the $q_j$ are [coprime polynomials](../../../../../coprime-polynomials.md), polynomial division and [Bezout identity](../../../../../bezout-identity.md) give polynomials $b_j$ such that

$$
\sum_jb_j(z)\frac{Q(z)}{q_j(z)}=1.
$$

For example, invert $Q/q_j$ modulo $q_j$, sum the resulting expressions, and absorb a remaining multiple of $Q$ into one coefficient. For $P(D)v=0$, the [kernel decomposition for coprime polynomials](../../../../../kernel-decomposition-for-coprime-polynomials.md) therefore gives

$$
v=\sum_jv_j,\qquad
v_j=b_j(D)\frac{Q(D)}{q_j(D)}v,\qquad
(D-\lambda_j)^{m_j}v_j=0.
$$

The [Leibniz rule](../../../../../leibniz-rule.md) for [multiplication of a distribution by a smooth function](../../../../../multiplication-of-a-distribution-by-a-smooth-function.md) implies $D^{m_j}(e^{-\lambda_jx}v_j)=0$. Repeatedly using [a distribution with zero derivative is constant](../../../../../a-distribution-with-zero-derivative-is-constant.md) shows that a [distribution](../../../../../distribution-mathematical-analysis.md) with $m$th derivative zero is a [polynomial](../../../../../polynomial-split.md) of degree at most $m-1$: subtract the polynomial primitive of its constant $(m-1)$st derivative, and induct on $m$. Consequently the most general [exponential polynomial solution of a constant-coefficient differential equation](../../../../../exponential-polynomial-solution-of-a-constant-coefficient-differential-equation.md) is

$$
\boxed{v(x)=\sum_{j=1}^r e^{\lambda_jx}\sum_{\ell=0}^{m_j-1}c_{j\ell}x^\ell.}
$$

Every displayed term is annihilated by $P(D)$, so all coefficients are allowed. For the [linear independence](../../../../../linear-independence.md) of these $n$ functions, on a relation, apply $\prod_{i\ne j}(D-\lambda_i)^{m_i}$; on $e^{\lambda_jx}$ times a polynomial of degree less than $m_j$, each remaining factor acts invertibly on that polynomial space. Hence the $j$th [polynomial](../../../../../polynomial-split.md) must vanish. **Every distributional solution is an [analytic function](../../../../../space-of-holomorphic-functions.md), and in particular a [classical solution](../../../../../classical-solution.md).** For real coefficients and real-valued [distributions](../../../../../distribution-mathematical-analysis.md), take [complex conjugate](../../../../../complex-conjugate.md) coefficients at conjugate [characteristic roots of a constant-coefficient differential equation](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md), or equivalently use the corresponding real sine and cosine forms.

For the last equation, the operator is $xP(D)$: the coordinate multiplies the result of differentiation. The [kernel of multiplication by a coordinate](../../../../../kernel-of-multiplication-by-a-coordinate.md) says precisely that

$$
xP(D)u=0\quad\Longleftrightarrow\quad P(D)u=C\delta_0.
$$

Choose the [retarded fundamental solution of a constant-coefficient ordinary differential operator](../../../../../retarded-fundamental-solution-of-a-constant-coefficient-ordinary-differential-operator.md) $E=Hw$, where $H$ is the [Heaviside function](../../../../../heaviside-step-function.md) and $w$ is the analytic solution of $P(D)w=0$ with

$$
w^{(j)}(0)=0\quad(0\leq j\leq n-2),\qquad w^{(n-1)}(0)=-1.
$$

Such $w$ exists uniquely by the elementary [initial value problem](../../../../../initial-value-problem.md) for a constant-coefficient [ordinary differential equation](../../../../../ordinary-differential-equation.md); alternatively the residue construction in the next solution gives it explicitly. The [distributional jump formula for a Heaviside product](../../../../../distributional-jump-formula-for-a-heaviside-product.md) is

$$
D^k(Hw)=Hw^{(k)}+\sum_{s=0}^{k-1}w^{(k-1-s)}(0)\delta_0^{(s)}.
$$

It follows by induction from $D(Hw)=Hw'+w(0)\delta_0$, using [integration by parts](../../../../../integration-by-parts.md). With the chosen initial derivatives, every lower-order jump term vanishes and the leading coefficient $-1$ gives $P(D)E=\delta_0$. Subtracting $CE$ reduces the last equation to the homogeneous one. Thus the [coordinate-degenerate constant-coefficient differential equation](../../../../../coordinate-degenerate-constant-coefficient-differential-equation.md) has exactly the solutions

$$
\boxed{u(x)=\sum_{j=1}^r e^{\lambda_jx}\sum_{\ell=0}^{m_j-1}c_{j\ell}x^\ell+C\,H(x)w(x).}
$$

There are $n+1$ independent constants. For $n\geq2$, derivatives through order $n-2$ match at zero, while the derivative of order $n-1$ may jump; for $n=1$, the function itself may jump. An arbitrary [distribution](../../../../../distribution-mathematical-analysis.md) concentrated at zero cannot be added, because its image under the nonzero leading derivative would contain a nonvanishing highest derivative of the [Dirac delta distribution](../../../../../dirac-delta-function.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
