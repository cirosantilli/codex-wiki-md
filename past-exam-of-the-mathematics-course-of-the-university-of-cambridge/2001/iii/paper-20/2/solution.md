<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We prove the Mahler alternative in full. Let $f(z)=\sum_{n\ge0}z^{l^n}$. Its series converges locally uniformly in the [unit disc](../../../../../unit-disc.md) and satisfies

$$
f(z^l)=f(z)-z.
$$

It is transcendental as a function. At a [root of unity](../../../../../root-of-unity.md) $\zeta$ with $\zeta^{l^r}=1$, the radial tail $\sum_{n\ge r}t^{l^n}$ in $f(t\zeta)$ is real and tends to infinity as $t\uparrow1$, while the initial terms remain bounded. These roots are dense on the [unit](../../../../../unit-in-a-ring.md) circle. An algebraic function can have singularities only at the finitely many zeros of its leading coefficient and [polynomial discriminant](../../../../../polynomial-discriminant.md): elsewhere its defining [polynomial](../../../../../polynomial-split.md) and the implicit-function theorem give local analytic branches. Hence $f$ cannot be algebraic over $\mathbb C(z)$.

Assume now that $\alpha$ and $f(\alpha)$ are algebraic, with $0<|\alpha|<1$, and put both in a [number field](../../../../../number-field.md) $K$ of degree $d$. For each $N$, the $(N+1)^2$ coefficients of a [polynomial](../../../../../polynomial-split.md) $P_N(X,Y)$ of bidegree at most $N$ can cancel the first $(N+1)^2-1$ Taylor coefficients of $P_N(z,f(z))$. The equations have [integer](../../../../../integer.md) coefficients, so a nonzero [integer](../../../../../integer.md) solution exists after clearing denominators. Functional transcendence makes $R_N(z)=P_N(z,f(z))$ nonzero. Its order $T_N$ at zero satisfies $T_N\ge(N+1)^2-1$.

At $\alpha_r=\alpha^{l^r}$ the [functional equation](../../../../../functional-equation.md) gives $f(\alpha_r)=f(\alpha)-\sum_{j<r}\alpha^{l^j}\in K$. Thus $\eta_r=R_N(\alpha_r)\in K$ is nonzero for all sufficiently large $r$ and

$$
\log|\eta_r|\le-T_Nl^r\log(1/|\alpha|)+O_N(1).
$$

Use the absolute [logarithmic height](../../../../../absolute-logarithmic-weil-height.md) $h$. The elementary inequalities for sums and [polynomial](../../../../../polynomial-split.md) evaluation give

$$
h(\eta_r)\le N\left(1+\frac1{l-1}\right)l^rh(\alpha)+O_N(r+1).
$$

Here $h(f(\alpha_r))\le h(f(\alpha))+(l^r-1)h(\alpha)/(l-1)+r\log2$. The [Liouville height inequality](../../../../../liouville-height-inequality.md) gives $\log|\eta_r|\ge-dh(\eta_r)$. Divide by $l^r$ and let $r\to\infty$ to obtain

$$
T_N\log(1/|\alpha|)\le dN\frac l{l-1}h(\alpha).
$$

The left grows quadratically in $N$, the right only linearly. Choose $N$ large to contradict this. Hence **every such algebraic $\alpha$ has transcendental $f(\alpha)$**. This is the [auxiliary-value height argument for the Fredholm series](../../../../../auxiliary-value-height-argument-for-the-fredholm-series.md).

For the rational continuation, let $a_n=\sum_{j=0}^n(p/q)^{l^j}$ and $Q_n=q^{l^n}$. This is a [rational number](../../../../../rational-number.md) with reduced denominator $B_n\le Q_n$, and its positive tail satisfies, for large $n$,

$$
0<f(p/q)-a_n\le2(p/q)^{l^{n+1}}=2Q_n^{-\kappa},\qquad\kappa=l\left(1-\frac{\log p}{\log q}\right)>l(1-\delta)>2.
$$

A rational value $a/b$ would instead have distance at least $1/(bQ_n)$ from each distinct $a_n$, already impossible. If the value were algebraic irrational, choose $\epsilon>0$ with $2+\epsilon<\kappa$. The distinct truncations have unbounded reduced denominators, and the displayed errors are eventually smaller than $B_n^{-2-\epsilon}$. This contradicts [Roth theorem](../../../../../roth-s-theorem.md). Thus the requested rational values are transcendental by the [Roth criterion for rational Fredholm values](../../../../../roth-criterion-for-rational-fredholm-values.md).

For completeness, the elliptic alternative's conclusion also has a short auxiliary-divisor certificate. If $\Phi$ is Frobenius on $E/\mathbb F_q$, then $\deg\Phi=q$ and $\deg(1-\Phi)=N=\#E(\mathbb F_q)$: the latter map is separable and its kernel is exactly the rational points. The [divisor](../../../../../divisor.md) identity for $x(P)-x(Q)$ on $E\times E$ gives the parallelogram rule $\deg(u+v)+\deg(u-v)=2\deg u+2\deg v$. Polarizing it yields

$$
\deg(m+n\Phi)=m^2+tmn+qn^2,\qquad t=q+1-N.
$$

All these degrees are nonnegative. In particular $\deg(-t+2\Phi)=4q-t^2\ge0$, so $|t|\le2\sqrt q$. The Frobenius characteristic [polynomial](../../../../../polynomial-split.md) is $X^2-tX+q$; its complex roots have modulus $\sqrt q$, including the double-root case. The zeta function has numerator $1-tT+qT^2$, whose zeros consequently have modulus $q^{-1/2}$, the elliptic Riemann hypothesis. This supplements the fully proved Mahler branch with the [degree-form proof of the Hasse bound](../../../../../degree-form-proof-of-the-hasse-bound.md); it is an auxiliary-divisor proof, not a claim that an unspecified transcendence theorem proves the bound.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
