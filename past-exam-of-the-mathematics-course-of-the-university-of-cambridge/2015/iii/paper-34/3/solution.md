<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $c_{\rm prem}$ for the premium income rate, reserving $c$ later for the smaller exponential decay rate. In the [classical risk model](../../../../../classical-risk-model.md), the surplus is

$$
U_t=u+c_{\rm prem}t-\sum_{j=1}^{N_t}X_j,
\qquad c_{\rm prem}=(1+\rho)\lambda\mu.
$$

Here $\rho$ is the [relative safety loading](../../../../../relative-safety-loading.md). The aggregate claims form a [Compound Poisson process](../../../../../compound-poisson-process.md). Define $L_t=\sum_{j=1}^{N_t}X_j-c_{\rm prem}t$, so ruin occurs when $L_t>u$. By [independent increments](../../../../../independent-increments.md) and the [exponential formula for a marked Poisson sum](../../../../../exponential-formula-for-a-marked-poisson-sum.md),

$$
\mathbb E[e^{R(L_t-L_s)}]
=\exp\{(t-s)[\lambda(M(R)-1)-c_{\rm prem}R]\}=1.
$$

Thus $Z_t=e^{RL_t}$ is a nonnegative [continuous-time martingale](../../../../../continuous-time-martingale.md) with $Z_0=1$, because the [adjustment coefficient](../../../../../adjustment-coefficient.md) makes the exponent vanish.

Let $\tau=\inf\{t:U_t<0\}$. Apply the [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) at the bounded [stopping time](../../../../../stopping-time.md) $\tau\wedge T$. On $\{\tau\leq T\}$, $L_\tau>u$, so

$$
1=\mathbb E[Z_{\tau\wedge T}]
\geq e^{Ru}\mathbb P(\tau\leq T).
$$

Letting $T$ increase proves **the Lundberg inequality and the unscaled limit**:

$$
\boxed{\psi(u)\leq e^{-Ru},\qquad
\lim_{u\to\infty}\psi(u)=0.}
$$

For the precise asymptotic, put

$$
h=\frac{\lambda\mu}{c_{\rm prem}}=\frac1{1+\rho},\quad
z(u)=e^{Ru}\psi(u),\quad
k(x)=h e^{Rx}f_I(x),\quad
g(u)=h e^{Ru}\int_u^\infty f_I(x)\,dx.
$$

The given exponential integral identity makes $k$ a probability density. Multiplying the given [defective renewal equation](../../../../../defective-renewal-equation.md) by $e^{Ru}$ turns it into the ordinary [renewal equation](../../../../../renewal-equation.md)

$$
z(u)=g(u)+\int_0^u z(u-x)k(x)\,dx.
$$

For clarity, the version of the [key renewal theorem](../../../../../key-renewal-theorem.md) used here is: if the interarrival law is nonarithmetic, has mean $m_k\in(0,\infty)$, and $g$ is [directly Riemann integrable](../../../../../direct-riemann-integrability.md), the locally bounded solution of this [renewal equation](../../../../../renewal-equation.md) satisfies $z(u)\to m_k^{-1}\int_0^\infty g(v)\,dv$. The infinite-mean version gives zero for nonnegative [directly Riemann integrable](../../../../../direct-riemann-integrability.md) $g$.

All the hypotheses can be checked here. The density $k$ gives a [nonarithmetic distribution](../../../../../nonarithmetic-distribution.md). The [Tonelli theorem](../../../../../tonelli-theorem.md) gives

$$
\int_0^\infty g(u)\,du
=h\int_0^\infty f_I(x)\frac{e^{Rx}-1}{R}\,dx
=\frac{1-h}{R}.
$$

Furthermore

$$
g(u)=\int_u^\infty e^{-R(x-u)}k(x)\,dx,\qquad
g'(u)=Rg(u)-k(u)\quad\hbox{almost everywhere}.
$$

Thus $g$ is continuous and integrable, and $\int_0^\infty|g'(u)|\,du\leq R\int g+1<\infty$. On a mesh of width $\delta$, the difference between its upper and lower sums is at most $\delta\int|g'|$; its upper sum is at most $\int g+\delta\int|g'|$. This proves [direct Riemann integrability](../../../../../direct-riemann-integrability.md) rather than assuming it. Also $0\leq z(u)\leq1$ by the [Lundberg inequality](../../../../../lundberg-inequality.md), so the solution is locally bounded. Its [renewal representation](../../../../../renewal-representation.md) is $z=g*U_k$, where $U_k=\sum_{j\geq0}K^{*j}$ and $K(dx)=k(x)\,dx$; the residual after iteration tends to zero on compact intervals because sums of positive interarrivals tend to infinity.

Writing $J=\int_0^\infty xe^{Rx}f_I(x)\,dx$, the tilted interarrival [expected value](../../../../../expected-value.md) is $m_k=hJ$. The [key renewal theorem](../../../../../key-renewal-theorem.md) gives **the [Cramér–Lundberg ruin asymptotic](../../../../../cramer-lundberg-ruin-asymptotic.md)**

$$
\boxed{\lim_{u\to\infty}e^{Ru}\psi(u)
=\frac{1-h}{RhJ}
=\frac{\rho}{R\displaystyle\int_0^\infty xe^{Rx}f_I(x)\,dx}=A.}
$$

If $J=\infty$, the same formula is interpreted as $A=0$. A positive finite asymptotic constant requires $J<\infty$; this extra integrability is not explicitly stated in the paper.

For the final two-exponential case, evaluate the [defective renewal equation](../../../../../defective-renewal-equation.md) at zero:

$$
h=\psi(0)=a+b,\qquad
\boxed{\rho=\frac{1-a-b}{a+b}}.
$$

One can identify the [adjustment coefficient](../../../../../adjustment-coefficient.md) without silently assuming $A>0$. For $0<r<c$, set

$$
P(r)=\int_0^\infty e^{ru}\psi(u)\,du
=\frac{a}{c-r}+\frac{b}{d-r}.
$$

It is finite and positive. Integrating the nonnegative terms of the [defective renewal equation](../../../../../defective-renewal-equation.md), using the [Tonelli theorem](../../../../../tonelli-theorem.md), first shows that $F_I(r)=\int_0^\infty e^{rx}f_I(x)\,dx$ is finite and then gives

$$
P(r)=\frac h r[F_I(r)-1]+hP(r)F_I(r),
\qquad
hF_I(r)=\frac{h+rP(r)}{1+rP(r)}.
$$

As $r\uparrow c$, $P(r)\to\infty$ because $a>0$. By [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), $hF_I(c)=1$. The [integrated tail distribution](../../../../../integrated-tail-distribution.md) in the [classical risk model](../../../../../classical-risk-model.md) has density $f_I(x)=\mathbb P(X_1>x)/\mu$, so $F_I(r)=[M(r)-1]/(\mu r)$ by the [tail integral formula for moments](../../../../../tail-integral-formula-for-moments.md). Hence $c$ solves the adjustment equation, and its stipulated uniqueness implies $R=c$. Finally the displayed form of $\psi$ gives **the remaining constants**

$$
\boxed{R=c,\qquad A=a,\qquad \rho=\frac{1-a-b}{a+b}.}
$$

In particular the decay exponent $d$ and the coefficient $b$ do not affect $R$ or $A$. The $c$ in these final answers is the printed decay rate, not $c_{\rm prem}$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
