<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Enlarge the space if needed to choose $Y_0$ with density $p$, independent of the driving [Brownian motion](../../../../../../brownian-motion-split.md), and solve the same equation with the same driver as $X_0=x$. The second moment of $p$ makes the initial difference square integrable. By parts (a) and (b),

$$
\mathbb E f(Y_t)=\int f(y)p(y)\,dy,
$$

while part (c) gives

$$
\mathbb E|X_t-Y_t|^2\leq D_xe^{-kt},\qquad D_x=\int(x-y)^2p(y)\,dy<\infty.
$$

We must not assume that the smooth bounded $f$ is globally Lipschitz. The hypotheses give $C_Y=\sup_t\mathbb EY_t^2<\infty$, hence [uniform tightness](../../../../../../uniform-tightness.md) of $(Y_t)$. For any $R$ and $0<\delta\leq1$, define the modulus of continuity of $f$ on $[-R-1,R+1]$ by $\omega_R(\delta)$. Splitting according to $|Y_t|\leq R$ and $|X_t-Y_t|\leq\delta$, and applying [Markov inequality](../../../../../../markov-inequality.md), gives

$$
\mathbb E|f(X_t)-f(Y_t)|
\leq\omega_R(\delta)+2\|f\|_\infty\left(\frac{C_Y}{R^2}+\frac{D_xe^{-kt}}{\delta^2}\right).
$$

First choose $R$ large, then $\delta$ small using uniform continuity on that compact interval, and finally let $t\to\infty$. The right side can be made arbitrarily small. Together with part (a), this proves

$$
\boxed{u(t,x)\longrightarrow\int_{\mathbb R}f(y)p(y)\,dy\quad\text{for every }x.}
$$

This is [convergence by synchronous coupling for bounded continuous test functions](../../../../../../convergence-by-synchronous-coupling-for-bounded-continuous-test-functions.md). It only needs the constant expectation from part (b) and uniform second moments; it does not add an unstated global bound on $f'$ or require a separate stationarity theorem. As explained in part (c), the literal bounded-drift plus strict-contraction assumptions have no global example; the calculation records the intended consequence under compatible dissipative-drift hypotheses as well.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
