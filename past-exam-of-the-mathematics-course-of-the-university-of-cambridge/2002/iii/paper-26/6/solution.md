<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use $\Xi(u)=\pi^{-u/2}\Gamma(u/2)\zeta(u)$ for the [completed Riemann zeta function](../../../../../completed-riemann-zeta-function.md), without the polynomial factor used to define the entire [Riemann xi function](../../../../../riemann-xi-function.md). For complex $\nu$ put

$$
K_\nu(Y)=\frac12\int_0^\infty e^{-Y(t+t^{-1})/2}t^{\nu-1}\,dt,\qquad Y>0.
$$

This is the [Modified Bessel function of the second kind](../../../../../modified-bessel-function-of-the-second-kind.md). The substitution $t=e^v$ writes it as $\tfrac12\int_{\mathbb R}e^{-Y\cosh v+\nu v}\,dv$, proving that it is entire in $\nu$, that $K_\nu=K_{-\nu}$, and that it decays exponentially as $Y\to\infty$, uniformly for $\nu$ in a compact set.

For $\Re s>1$ all the lattice sums and the integrals below converge absolutely. The $m=0$ terms in the [completed nonholomorphic Eisenstein series](../../../../../completed-nonholomorphic-eisenstein-series.md) contribute $\Xi(2s)y^s$. For $m\ne0$, use the [Gamma integral](../../../../../gamma-integral.md) and then [Poisson summation](../../../../../poisson-summation-formula.md) in $n$:

$$
\begin{aligned}
\mathcal E(z,s)-\Xi(2s)y^s
&=\frac{y^s}{2}\sum_{m\ne0}\int_0^\infty u^{s-1}e^{-\pi m^2y^2u}\sum_n e^{-\pi u(n+mx)^2}\,du\\
&=\frac{y^s}{2}\sum_{m\ne0}\sum_{h\in\mathbb Z}e^{2\pi ihmx}
\int_0^\infty u^{s-3/2}e^{-\pi m^2y^2u-\pi h^2/u}\,du.
\end{aligned}
$$

Here the Poisson identity is $\sum_n e^{-\pi u(n+mx)^2}=u^{-1/2}\sum_h e^{-\pi h^2/u}e^{2\pi ihmx}$. At $h=0$, evaluating the [Gamma integral](../../../../../gamma-integral.md) and summing over $m$ gives $\Xi(2s-1)y^{1-s}$. At $h\ne0$, the substitution $u=|h|t/(|m|y)$ and the [integral representation of the modified Bessel function of the second kind](../../../../../integral-representation-of-the-modified-bessel-function-of-the-second-kind.md) give

$$
\int_0^\infty u^{s-3/2}e^{-\pi m^2y^2u-\pi h^2/u}\,du
=2\left(\frac{|h|}{|m|y}\right)^{s-1/2}K_{s-1/2}(2\pi|mh|y).
$$

Collect the frequency $r=mh\ne0$. There are two signed choices of $m$ for each positive divisor of $|r|$. Thus, with $\sigma_a(n)=\sum_{d\mid n}d^a$, the full [Fourier expansion](../../../../../fourier-series-split.md) is

$$
\boxed{\mathcal E(z,s)=\Xi(2s)y^s+\Xi(2s-1)y^{1-s}
+2\sqrt y\sum_{r\ne0}|r|^{s-1/2}\sigma_{1-2s}(|r|)K_{s-1/2}(2\pi|r|y)e^{2\pi irx}.}
$$

The factor $2$ is important: the lattice sum includes both signs, while the defining factor $1/2$ was already used in its Mellin integral. This expansion uses exactly the completion in the question.

We can deduce both of the offered conclusions. First recall, with a short proof, the needed [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md). Put $\Theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}$. [Poisson summation](../../../../../poisson-summation-formula.md) gives $\Theta(t)=t^{-1/2}\Theta(1/t)$. Splitting the Mellin integral of $\Theta-1$ at one yields

$$
\Xi(u)=-\frac1u-\frac1{1-u}
+\frac12\int_1^\infty(\Theta(t)-1)\left(t^{u/2-1}+t^{(1-u)/2-1}\right)\,dt.
$$

The integral is entire and invariant under $u\mapsto1-u$. Hence $\Xi(u)=\Xi(1-u)$, with only simple [poles](../../../../../pole.md) at $u=0,1$, of residues $-1,1$. This is the pole-bearing completion, not the entire xi function.

For fixed $y>0$, the nonconstant part of the Eisenstein expansion is entire in $s$ and locally normally convergent: the [divisor sums](../../../../../divisor-sum.md) grow at most polynomially on a compact set of $s$, whereas $K_{s-1/2}(2\pi|r|y)$ decays exponentially in $|r|$. The same argument gives local uniformity for $z$ in compact subsets of the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Thus only the constant terms can have poles. Their apparent poles at $s=1/2$ cancel: $\Xi(2s)$ has principal part $1/(2(s-1/2))$, while $\Xi(2s-1)$ has its negative, and both multiply $y^{1/2}$ there. The remaining poles are simple, at $s=0,1$, with residues $-1/2,1/2$.

Under $s\mapsto1-s$, the two constant terms interchange by the zeta functional equation. The nonconstant terms are unchanged because $K_\nu=K_{-\nu}$ and

$$
|r|^{s-1/2}\sigma_{1-2s}(|r|)=|r|^{1/2-s}\sigma_{2s-1}(|r|),
$$

which follows by replacing a divisor $d$ by $|r|/d$. Therefore

$$
\boxed{\mathcal E(z,s)\text{ is meromorphic on }\mathbb C,\quad
\mathcal E(z,s)=\mathcal E(z,1-s),\quad
\operatorname{Res}_{s=0}\mathcal E=-\tfrac12,\quad
\operatorname{Res}_{s=1}\mathcal E=\tfrac12.}
$$

For the [Kronecker limit formula](../../../../../kronecker-limit-formula.md), evaluate the finite Laurent coefficient at $s=1$. Write $\gamma_E$ for the [Euler--Mascheroni constant](../../../../../euler-s-constant.md). From $\zeta(u)=1/(u-1)+\gamma_E+O(u-1)$ and $\Gamma'(1/2)/\Gamma(1/2)=-\gamma_E-2\log2$ we obtain

$$
\Xi(2s-1)=\frac1{2(s-1)}+\frac{\gamma_E-\log(4\pi)}2+O(s-1).
$$

The gamma derivative follows by differentiating the [Gamma duplication formula](../../../../../gamma-duplication-formula.md) and using $\Gamma'(1)=-\gamma_E$. Multiplication by $y^{1-s}$ adds $-\tfrac12\log y$ to the constant term; the other constant term contributes $\Xi(2)y=\pi y/6$.

The half-order [Modified Bessel function of the second kind](../../../../../modified-bessel-function-of-the-second-kind.md) is $K_{1/2}(Y)=\sqrt{\pi/(2Y)}e^{-Y}$. For example, in its even integral representation set $v/2$ as variable and then $u=\sinh(v/2)$: $\cosh v=1+2u^2$ and the $\cosh(v/2)$ factor converts the integral to a Gaussian. At $s=1$ the nonconstant Eisenstein coefficients are consequently $\sigma_{-1}(|r|)e^{-2\pi|r|y}$. On the other hand, the absolutely convergent logarithmic series gives

$$
\log\prod_{n\geq1}(1-q^n)=-\sum_{r\geq1}\sigma_{-1}(r)q^r.
$$

Adding this identity to its conjugate identifies the nonconstant sum as $-2\log|\prod_{n\geq1}(1-q^n)|$. With the analytic [Dedekind eta function](../../../../../dedekind-eta-function.md) product $\eta(z)=q^{1/24}\prod_{n\geq1}(1-q^n)$, the resulting answer is

$$
\boxed{\mathcal E(z,s)=\frac1{2(s-1)}+\frac{\gamma_E-\log(4\pi)}2
-\log\left(\sqrt y\,|\eta(z)|^2\right)+O(s-1).}
$$

This derivation of the [Kronecker limit formula](../../../../../kronecker-limit-formula.md) uses the analytic eta product only; it does not assume its modular transformation. The lattice series is invariant for $\Re s>1$ by an integral change of the pair $(m,n)$ and $\Im(\gamma z)=y/|cz+d|^2$. Analytic continuation preserves this invariance, so its finite Laurent coefficient is invariant too. This supplies the independent weight-two transformation argument used in Question 2.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
