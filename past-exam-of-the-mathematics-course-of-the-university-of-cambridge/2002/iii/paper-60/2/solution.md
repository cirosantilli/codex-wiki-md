<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work in the standard class of real constant-coefficient [linear multistep methods](../../../../../linear-multistep-method.md) using only first-derivative evaluations. Write

$$
\sum_{j=0}^s\alpha_jY_{n+j}=h\sum_{j=0}^s\beta_jf(t_{n+j},Y_{n+j}),\qquad
\rho(z)=\sum_{j=0}^s\alpha_jz^j,\quad \sigma(z)=\sum_{j=0}^s\beta_jz^j,
$$

with $\alpha_s\ne0$. The [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) states that such a method converges on each fixed finite time interval, for sufficiently regular Lipschitz [initial value problems](../../../../../initial-value-problem.md) and every set of consistent starting values, if and only if it is consistent and [zero-stable](../../../../../zero-stability.md). Consistency means $\rho(1)=0$ and $\rho'(1)=\sigma(1)$. [Zero-stability](../../../../../zero-stability.md) means all roots of $\rho$ lie in $|z|\leq1$ and every root on $|z|=1$ is simple. In particular the consistency root at $1$ is simple.

[Taylor expansion](../../../../../taylor-expansion.md) of the exact-solution residual gives the [exponential-symbol order criterion for a multistep method](../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md)

$$
\rho(e^w)-w\sigma(e^w)=O(w^{p+1}).
$$

This criterion packages the identities $\sum\alpha_jj^q=q\sum\beta_jj^{q-1}$ through $q=p$. We now derive the upper bound on $p$ from the root condition, rather than assuming the [first Dahlquist barrier](../../../../../first-dahlquist-barrier.md).

Use the [Cayley transform](../../../../../cayley-transform-complex-analysis.md) $z=(1+x)/(1-x)$ and define

$$
R(x)=(1-x)^s\rho\left(\frac{1+x}{1-x}\right)=xP(x),\qquad
S(x)=(1-x)^s\sigma\left(\frac{1+x}{1-x}\right).
$$

The simple root at $z=1$ gives $P(0)\ne0$, while $\deg P\leq s-1$ and $\deg S\leq s$. Each finite transformed root is $x=(z-1)/(z+1)$, with nonpositive real part when $|z|\leq1$. A possible root at $z=-1$ simply lowers the degree of $R$. Factor $P$ over the reals: a real root contributes $x+a$ with $a>0$, and a conjugate pair contributes $x^2+2ax+a^2+b^2$ with $a\geq0$. Therefore, after reversing the overall sign if needed,

$$
P(x)=\sum_{j=0}^{s-1}P_jx^j,\qquad P_j\geq0,\quad P_0>0.
$$

Since $w=2\operatorname{arctanh}x$, the order criterion is equivalent to

$$
S(x)-\frac12P(x)F(x)=O(x^p),\qquad F(x)=\frac{x}{\operatorname{arctanh}x}.
$$

The key [coefficient sign lemma for the first Dahlquist barrier](../../../../../coefficient-sign-lemma-for-the-first-dahlquist-barrier.md) is

$$
F(x)=1-\sum_{j\geq1}\gamma_jx^{2j},\qquad \gamma_j>0.
$$

Here is a proof of that sign assertion. Direct integration gives

$$
F(x)=\int_0^1(1+x)^t(1-x)^{1-t}\,dt.
$$

Differentiate twice and pair the terms at $t$ and $1-t$ to obtain

$$
F''(x)=-4\int_0^1t(1-t)(1-x^2)^{-3/2}
\cosh[(2t-1)\operatorname{arctanh}x]\,dt.
$$

The [power series](../../../../../power-series.md) of $\operatorname{arctanh}x$ has positive odd coefficients. The even powers in the [hyperbolic cosine](../../../../../hyperbolic-cosine.md) therefore have nonnegative coefficients, and $(1-x^2)^{-3/2}$ has strictly positive even coefficients. Every even coefficient of $F''$ is consequently negative. Also $F$ is even and $F(0)=1$, proving the assertion.

If $s$ is odd and $p\geq s+2$, the coefficient of $x^{s+1}$ in $PF$ must vanish because $\deg S\leq s$. But it is

$$
-\sum_{j\geq1}\gamma_jP_{s+1-2j}<0,
$$

where out-of-range indices are zero and the sum includes the strictly positive $\gamma_{(s+1)/2}P_0$. This is impossible, so $p\leq s+1$. If $s$ is even and $p\geq s+3$, exactly the same argument with the coefficient of $x^{s+2}$ gives a contradiction. Thus $p\leq s+2$ in that case. This proves the [Cayley coefficient proof of the first Dahlquist barrier](../../../../../cayley-coefficient-proof-of-the-first-dahlquist-barrier.md):

$$
\boxed{p\leq 2\left\lfloor\frac{s+2}{2}\right\rfloor.}
$$

To prove that the bound is attainable for every $s$, let $L_j$ be the [Lagrange polynomials](../../../../../lagrange-polynomial.md) for the nodes $0,1,\ldots,s$, and take $w_j=\int_0^sL_j(t)\,dt$. The [Newton-Cotes multistep methods attaining the first Dahlquist barrier](../../../../../newton-cotes-multistep-methods-attaining-the-first-dahlquist-barrier.md) are

$$
Y_{n+s}-Y_n=h\sum_{j=0}^sw_jf_{n+j}.
$$

The underlying [Newton-Cotes closed quadrature](../../../../../newton-cotes-closed-quadrature.md) is exact on all [polynomials](../../../../../polynomial-split.md) of degree at most $s$. For even $s$, the node [polynomial](../../../../../polynomial-split.md) $q(t)=\prod_{j=0}^s(t-j)$ is odd about $s/2$, so $\int_0^sq(t)\,dt=0$. Dividing any degree-$s+1$ [polynomial](../../../../../polynomial-split.md) by $q$ shows that quadrature exactness extends one degree further. Integrating the exact derivative therefore gives method order at least $s+1$ for odd $s$ and at least $s+2$ for even $s$.

Finally $\rho(z)=z^s-1$ has only simple unit-circle roots, so these methods satisfy the root condition. The weights sum to $s=\rho'(1)$, proving consistency. The [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) gives convergence with consistent starts; the proved upper bound makes the attained formal orders exact; starting values accurate to those orders also give the corresponding global accuracy. Hence **the highest convergent order is $2\lfloor(s+2)/2\rfloor$**. This result concerns the stated linear first-derivative class, not unrestricted multiderivative or nonlinear formulas.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
