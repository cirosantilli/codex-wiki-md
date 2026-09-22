<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $\mathbb T^n=(\mathbb R/2\pi\mathbb Z)^n$ and the uniform metric $d(f,g)=\|f-g\|_\infty$. Let $N(\varepsilon,E)$ be the least number of radius-$\varepsilon$ balls in this metric covering $E$. The [Kolmogorov entropy](../../../../../metric-entropy.md), equivalently [metric entropy](../../../../../metric-entropy.md), is

$$
\boxed{H(\varepsilon,E)=\log N(\varepsilon,E)}.
$$

It is infinite if no finite cover exists; set the entropy of the empty set to zero. Changing the logarithm base or requiring centres in $E$ changes only the constants and resolution factors in the estimates below.

For an explicit appropriate norm, take

$$
\|f\|_{C^p}=\max_{|\alpha|\le p}\|\partial^\alpha f\|_\infty.
$$

An equivalent standard norm gives the same exponents, with different constants. We prove the two bounds for the [entropy of a smooth periodic function ball](../../../../../entropy-of-a-smooth-periodic-function-ball.md) separately.

For the lower bound, choose a nonnegative [bump function](../../../../../bump-function.md) $\varphi\in C_c^\infty((-1,1)^n)$ with $0\le\varphi\le1$ and $\varphi(0)=1$. Let $K$ bound all its derivatives of orders at most $p$, and choose $c>0$ with $cK\le1$. For sufficiently small $h\le1$, place $L\ge c_nh^{-n}$ translates of its scaled support disjointly on the [torus](../../../../../torus.md), for instance by taking grid centres separated by $3h$ in a fundamental cube. Define the real functions

$$
f_\sigma(x)=c h^p\sum_{j=1}^{L}\sigma_j\varphi\left(\frac{x-x_j}{h}\right),
\qquad \sigma\in\{0,1\}^{L},
$$

using periodic extension. Disjointness means that at any point only one summand contributes. For every $|\alpha|\le p$, its derivative is bounded by $c h^{p-|\alpha|}K\le1$. Thus every $f_\sigma$ lies in $B_{n,p}$. If $\sigma\ne\tau$, evaluate at a centre where the binary coefficients differ to obtain

$$
\|f_\sigma-f_\tau\|_\infty=ch^p.
$$

Choose $h=(4\varepsilon/c)^{1/p}$ for sufficiently small $\varepsilon$. The $2^L$ functions are more than $2\varepsilon$ apart, so no radius-$\varepsilon$ ball covers two of them. The [metric covering number](../../../../../metric-covering-number.md) consequently satisfies

$$
H(\varepsilon,B_{n,p})\ge L\log2\ge c'_{n,p}\varepsilon^{-n/p}.
$$

To include the remaining $\varepsilon<1/2$, observe that the two constant functions $1,-1$ belong to the ball and require distinct covering balls. Reducing the positive lower-bound constant extends the estimate over that fixed remaining interval.

For the upper bound, use this precise version of [multivariable Jackson approximation](../../../../../multivariable-jackson-approximation.md): for every $f\in C^p(\mathbb T^n)$ and integer $N\ge1$, there exists a real [trigonometric polynomial](../../../../../trigonometric-polynomial.md) $P_N$ with $|k_j|\le N$ in every coordinate and

$$
\|f-P_N\|_\infty\le J_{n,p}N^{-p}\|f\|_{C^p}.
$$

Choose $N=\lceil(4J_{n,p}/\varepsilon)^{1/p}\rceil$. Then the approximation error is at most $\varepsilon/4$, and $\|P_N\|_\infty\le2$. Write $P_N(x)=\sum_{k\in\{-N,\ldots,N\}^n}c_ke^{ik\cdot x}$. There are $D=(2N+1)^n$ coefficients, and normalized integration gives $|c_k|\le\|P_N\|_\infty\le2$.

Round their real and imaginary parts with mesh $\delta=\varepsilon/(8D)$, respecting $c_{-k}=\overline{c_k}$ so the rounded polynomial remains real. Each coefficient changes by at most $2\delta$, and hence the uniform change in the polynomial is at most $2D\delta=\varepsilon/4$. At most $(C/\delta)^{2D}$ choices are needed; allowing redundant choices only enlarges this bound. These rounded polynomials form an $\varepsilon$-net for the ball, and

$$
H(\varepsilon,B_{n,p})\le2D\log\left(\frac{CD}{\varepsilon}\right)
\le C_2\varepsilon^{-n/p}\log(1/\varepsilon).
$$

Here $D\le C_{n,p}\varepsilon^{-n/p}$, and the last logarithm absorbs the constant and $\log D$ for $\varepsilon<1/2$. Together the bounds give

$$
\boxed{C_1\varepsilon^{-n/p}\le H(\varepsilon,B_{n,p})
\le C_2\varepsilon^{-n/p}\log(1/\varepsilon)}.
$$

For the unit ball of $C(\mathbb T^n)$ alone, take infinitely many disjoint small neighbourhoods and a height-one continuous bump supported in each. Distinct such functions have uniform distance one. Thus no finite $\varepsilon$-net exists when $\varepsilon<1/2$, and

$$
\boxed{H(\varepsilon,B_{C})=\infty\quad(0<\varepsilon<1/2)}.
$$

The derivative bound was essential for [total boundedness](../../../../../totally-bounded-space.md); mere continuity gives no common small-scale oscillation bound.

For the final composition estimate, interpret outer [periodic functions](../../../../../periodic-function.md) on $\mathbb T^m$ by their $2\pi$-periodic extensions to $\mathbb R^m$. Since $p\ge1$, each $f\in B_{m,p}$ satisfies

$$
|f(x)-f(y)|\le\sum_{j=1}^m|x_j-y_j|
\le m\max_j|x_j-y_j|,
$$

by integrating its first partial derivatives along coordinate segments. This uniform [Lipschitz continuity](../../../../../lipschitz-continuity.md) controls errors in the inner functions.

Choose an outer net of radius $\eta=\varepsilon/2$ for $B_{m,p}$ and an inner net of radius $\delta=\varepsilon/(2m)$ for $E$. For each $g=f(u_1,\ldots,u_m)$ choose corresponding approximants $f_0,v_1,\ldots,v_m$. No derivative bound for $f_0$ is needed: use the derivative bound of $f$ before replacing the outer function. Pointwise,

$$
\begin{aligned}
|f(u_1,\ldots,u_m)-f_0(v_1,\ldots,v_m)|
&\le|f(u_1,\ldots,u_m)-f(v_1,\ldots,v_m)|+\|f-f_0\|_\infty\\
&\le m\delta+\eta=\varepsilon.
\end{aligned}
$$

All composed centres are continuous. Multiplying the numbers of outer and inner choices gives the [entropy of Lipschitz compositions](../../../../../entropy-of-lipschitz-compositions.md) inequality

$$
H(\varepsilon,F)\le H(\varepsilon/2,B_{m,p})
+mH(\varepsilon/(2m),E).
$$

Apply the proved upper bound with dimension $m$, and the assumed estimate for $E$. Fixed rescalings of $\varepsilon$ preserve its exponent and change $\log(1/\varepsilon)$ by only an additive constant. Therefore

$$
\boxed{H(\varepsilon,F)\le C_4\varepsilon^{-m/p}\log(1/\varepsilon)
\quad(0<\varepsilon<1/2)}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
