<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The claim law is an [Erlang distribution](../../../../../erlang-distribution.md) of shape two and rate $2/\beta$. Direct integration, using $\int_0^\infty xe^{-ax}\,dx=a^{-2}$ for $a>0$, gives its [moment-generating function](../../../../../moment-generating-function.md)

$$
M_X(r)=\frac4{\beta^2}\int_0^\infty xe^{-(2/\beta-r)x}\,dx
=\left(1-\frac{\beta r}{2}\right)^{-2},\qquad r<2/\beta.
$$

Differentiating at zero gives $\mathbb EX=\beta$. The positive [relative safety loading](../../../../../relative-safety-loading.md) condition for the [classical risk model](../../../../../classical-risk-model.md) is therefore

$$
\boxed{c>\lambda\beta.}
$$

The [adjustment coefficient](../../../../../adjustment-coefficient.md) is the positive root in the finite-transform domain of

$$
\lambda[M_X(R)-1]=cR.
$$

Set $z=\beta R/2$ and $k=2c/(\lambda\beta)>2$. For $R>0$, division by $z$ reduces the equation to

$$
\frac{2-z}{(1-z)^2}=k,
\qquad kz^2+(1-2k)z+k-2=0.
$$

The two roots are $z=(2k-1\pm\sqrt{1+4k})/(2k)$. The minus root lies strictly between zero and one: positivity follows from $(2k-1)^2-(1+4k)=4k(k-2)>0$, and the numerator is smaller than $2k$. The plus root exceeds one and is outside the moment-generating function's domain. Consequently the [adjustment coefficient for shape-two Erlang claims](../../../../../adjustment-coefficient-for-shape-two-erlang-claims.md) is

$$
\boxed{R=\frac{2k-1-\sqrt{1+4k}}{k\beta},\qquad k=\frac{2c}{\lambda\beta}.}
$$

The zero root of the original equation is not an adjustment coefficient. The increasing secant slope $(M_X(r)-1)/r$ on $(0,2/\beta)$ also establishes uniqueness of the positive root.

Now set $\beta=1$. Under [quota share reinsurance](../../../../../quota-share-reinsurance.md), the retained payment is $Y_\alpha=\alpha X$. For $0<\alpha\leq1$, the [change of variables](../../../../../change-of-variables-formula.md) $x=y/\alpha$ yields

$$
\boxed{f_{Y_\alpha}(y)=\frac4{\alpha^2}ye^{-2y/\alpha},\quad y>0,\qquad
Y_\alpha\sim\operatorname{Gamma}(2,2/\alpha).}
$$

Here the second gamma parameter is the rate. In particular, $\mathbb EY_\alpha=\alpha$ and $M_{Y_\alpha}(r)=(1-\alpha r/2)^{-2}$. At full cession $\alpha=0$ the retained payment instead has a point mass at zero.

The reinsurer's expected annual payments are $\lambda(1-\alpha)$, so its loaded premium is $(1+\theta_R)\lambda(1-\alpha)$. Subtract it from the original premium income to obtain the direct insurer's net premium rate

$$
\begin{aligned}
c_\alpha
&=(1+\theta)\lambda-(1+\theta_R)\lambda(1-\alpha)\\
&=\lambda[(1+\theta_R)\alpha+\theta-\theta_R].
\end{aligned}
$$

Its expected retained claim outflow is $\lambda\alpha$. Thus

$$
\boxed{c_\alpha-\lambda\mathbb EY_\alpha
=\lambda[\theta-\theta_R(1-\alpha)]>0}
$$

by the stipulated lower bound on $\alpha$. In particular $c_\alpha>0$, so the retained portfolio satisfies the net profitability condition. Its [relative safety loading](../../../../../relative-safety-loading.md) is $\theta_R-(\theta_R-\theta)/\alpha$.

Apply the same [adjustment coefficient for shape-two Erlang claims](../../../../../adjustment-coefficient-for-shape-two-erlang-claims.md) formula with scale $\alpha$ and net premium $c_\alpha$. Writing

$$
k_\alpha=\frac{2c_\alpha}{\lambda\alpha}
=2\left[1+\theta_R-\frac{\theta_R-\theta}{\alpha}\right]>2,
$$

gives

$$
\boxed{R_\alpha=\frac{2k_\alpha-1-\sqrt{1+4k_\alpha}}{k_\alpha\alpha}.}
$$

Equivalently it is the positive solution, with $R_\alpha<2/\alpha$, of

$$
\lambda\left[\left(1-\frac{\alpha R_\alpha}{2}\right)^{-2}-1\right]=c_\alpha R_\alpha.
$$

For fixed positive initial capital, a larger [adjustment coefficient](../../../../../adjustment-coefficient.md) reduces the exponential upper bound $\psi_\alpha(u)\leq e^{-R_\alpha u}$ from the [Lundberg inequality](../../../../../lundberg-inequality.md). It also makes the large-capital decay exponent in the [Cramér–Lundberg ruin asymptotic](../../../../../cramer-lundberg-ruin-asymptotic.md) larger. These are the reasons for maximizing $R_\alpha$ as a ruin-risk criterion; the coefficient alone need not order exact finite-capital ruin probabilities for arbitrary different models.

If $\theta_R=\theta$, then $c_\alpha=(1+\theta)\lambda\alpha$ and $k_\alpha=2(1+\theta)$ is constant. The [equal-loading quota share and vanishing retention](../../../../../equal-loading-quota-share-and-vanishing-retention.md) relation becomes

$$
\boxed{R_\alpha=\frac{3+4\theta-\sqrt{9+8\theta}}{2(1+\theta)\alpha}
=\frac{R_1}{\alpha}.}
$$

The numerator is positive for $\theta>0$, so $R_\alpha$ decreases strictly with $\alpha$ and tends to infinity as $\alpha\downarrow0$. **There is no maximizing retention in the stipulated interval $0<\alpha\leq1$; the best limit is full cession.** If the endpoint $\alpha=0$ is admitted as an idealized contract, all claims are transferred and the net premium income is zero, leaving the direct insurer's capital constant and its [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) zero. At that endpoint the coefficient equation is identically zero, so it no longer defines a unique finite adjustment coefficient. Calling $\alpha=0$ optimal requires this explicit extension of the original admissible set.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
