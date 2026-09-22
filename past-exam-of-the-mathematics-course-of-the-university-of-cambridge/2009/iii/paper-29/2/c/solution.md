<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x\leq0$, $f_n(x)=|x|$; for $x>0$, only the interval $(0,1/n)$ contributes an error to the integral of the derivative. Hence

$$
0\leq|x|-f_n(x)\leq\frac2n\qquad(x\in\mathbb R).
$$

By the [Itô formula](../../../../../../ito-s-lemma.md), the continuous processes

$$
C_t^{(n)}=\frac12\int_0^t f_n''(X_s)d[M]_s=f_n(X_t)-\int_0^t f_n'(X_s)dM_s-\int_0^t f_n'(X_s)dA_s
$$

are nondecreasing, since $f_n''\geq0$. Parts (a) and (b), together with the uniform approximation of absolute value, show that $C^{(n)}$ converges [uniformly on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md) to

$$
Z_t=|X_t|-\int_0^t\operatorname{sgn}_-(X_s)dM_s-\int_0^t\operatorname{sgn}_-(X_s)dA_s.
$$

The limit is continuous: the [martingale](../../../../../../martingale-split.md) integral is continuous, and the bounded-integrand finite-variation integral is continuous because $A$ is continuous. For any rational $s<t$, [convergence in probability](../../../../../../convergence-in-probability.md) and $C_t^{(n)}-C_s^{(n)}\geq0$ imply $Z_t-Z_s\geq0$ almost surely. Intersect these countably many events and use continuity to extend to all real $s<t$. Thus

$$
\boxed{Z_0=0,\qquad Z\text{ is continuous and nondecreasing almost surely}.}
$$

Since $|X|=\operatorname{sgn}_-(X)\cdot M+(\operatorname{sgn}_-(X)\cdot A+Z)$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md) plus continuous [finite variation](../../../../../../total-variation-of-a-function.md), $|X|$ is a [continuous semimartingale](../../../../../../continuous-semimartingale.md). This is the [smooth convex approximation proof of the Tanaka formula](../../../../../../smooth-convex-approximation-proof-of-the-tanaka-formula.md). With the specified sign value $-1$ at zero, $Z$ is the [right local time](../../../../../../right-local-time-of-a-continuous-semimartingale.md) at zero, rather than an unspecified symmetric normalization.

For an arbitrary [continuous semimartingale](../../../../../../continuous-semimartingale.md) starting at zero, use its continuous decomposition $X=M+A$, with both parts starting at zero, and let

$$
\rho_k=\inf\{t\geq0:|M_t|+V_t\geq k\}\wedge k.
$$

The continuity and local finiteness of variation imply $\rho_k\uparrow\infty$ almost surely. Up to $\rho_k$ the required deterministic bound holds, and the stopped [local martingale](../../../../../../local-martingale.md) is bounded, hence a true $L^2$-bounded [martingale](../../../../../../martingale-split.md). Apply the previous argument to $X^{\rho_k}$ for each integer $k$. Stopping the defining integrals gives precisely $Z_{t\wedge\rho_k}$. On the intersection of their full-probability events, each stopped $Z$ is nondecreasing; every finite interval is eventually contained before $\rho_k$, so $Z$ is nondecreasing globally. Therefore

$$
\boxed{|X|\text{ is a continuous semimartingale for every continuous semimartingale }X.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
