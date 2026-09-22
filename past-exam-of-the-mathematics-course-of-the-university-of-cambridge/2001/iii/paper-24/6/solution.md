<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use coordinates $1,2,3$ for paper, scissors and stone. Let $X^N$ take values in the lattice [simplex](../../../../../simplex.md) $S_N=\{(n_1,n_2,n_3)/N:n_i\geq0,\ \sum_i n_i=N\}$. A uniformly selected unordered pair consists of types $i$ and $j$, $i\ne j$, with probability $2n_in_j/(N(N-1))$. Losing copies the winner, so the possible jumps of the [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) are

$$
\frac{e_1-e_3}{N},\qquad\frac{e_2-e_1}{N},\qquad\frac{e_3-e_2}{N}.
$$

Ties make no change. For arbitrary event rate $\lambda$, the respective transition rates are $2\lambda Nx_1x_3/(N-1)$, $2\lambda Nx_2x_1/(N-1)$ and $2\lambda Nx_3x_2/(N-1)$. Choose

$$
\boxed{\lambda_N=\frac{N-1}{2}.}
$$

Then the rates are exactly $Nx_1x_3$, $Nx_2x_1$, $Nx_3x_2$. The [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md) of this [cyclic imitation chain](../../../../../cyclic-imitation-chain.md) is

$$
\mathcal L_Nf(x)=N\sum_{\ell\in\mathcal J}\beta_\ell(x)\bigl(f(x+\ell/N)-f(x)\bigr),
$$

where $\mathcal J=\{e_1-e_3,e_2-e_1,e_3-e_2\}$ and the three $\beta$ functions are, in that order, $x_1x_3,x_2x_1,x_3x_2$. Its drift is precisely

$$
F(x)=\sum_\ell\ell\beta_\ell(x)
=\bigl(x_1(x_3-x_2),\ x_2(x_1-x_3),\ x_3(x_2-x_1)\bigr).
$$

Here is a precise [fluid limit](../../../../../fluid-limit.md) with its error control. Suppose $X^N_0\to x_0$ in probability, and let $x$ solve $\dot x=F(x)$, $x(0)=x_0$. For every finite $T$,

$$
\boxed{\sup_{0\leq t\leq T}\|X^N_t-x_t\|\longrightarrow0\quad\text{in probability}.}
$$

Indeed, the [martingale decomposition of a density-dependent jump process](../../../../../martingale-decomposition-of-a-density-dependent-jump-process.md) gives

$$
X^N_t=X^N_0+\int_0^tF(X^N_s)\,ds+M^N_t,
\qquad
\langle M^N\rangle_t=\frac1N\int_0^t\sum_\ell\ell\ell^{\mathsf T}\beta_\ell(X^N_s)\,ds.
$$

This follows by compensating each transition count by its integrated rate; the compensated counts are square-integrable [martingales](../../../../../martingale-split.md), with variance equal to the expected compensator. Since $\|\ell\|^2=2$ and $x_1x_2+x_2x_3+x_3x_1\leq1/3$ on the [simplex](../../../../../simplex.md), the [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md), applied coordinatewise, gives

$$
\mathbb E\sup_{t\leq T}\|M^N_t\|^2\leq4\mathbb E\|M^N_T\|^2
\leq\frac{8T}{3N}.
$$

The polynomial drift is [Lipschitz](../../../../../lipschitz-continuity.md) on the compact [simplex](../../../../../simplex.md), with some finite constant $L$. It preserves the sum of the coordinates, and each coordinate solves an equation of the form $\dot x_i=x_i h_i(x)$, so nonnegativity is preserved. Thus the [ordinary differential equation](../../../../../ordinary-differential-equation.md) stays in the [simplex](../../../../../simplex.md) and exists for all time. The [Gronwall inequality](../../../../../gronwall-inequality.md) gives

$$
\sup_{t\leq T}\|X^N_t-x_t\|
\leq e^{LT}\left(\|X^N_0-x_0\|+\sup_{t\leq T}\|M^N_t\|\right),
$$

which proves the claim by [Markov's inequality](../../../../../markov-inequality.md). This proves the required version directly, rather than invoking an unspecified approximation theorem.

For an interior trajectory, differentiating the logarithm of the [product of numbers](../../../../../product-of-numbers.md) gives

$$
\frac{d}{dt}\log(x_1x_2x_3)
=(x_3-x_2)+(x_1-x_3)+(x_2-x_1)=0.
$$

The same identity for the product itself holds on the boundary, so **$x_1(t)x_2(t)x_3(t)$ is conserved.** A strictly positive initial product keeps the deterministic trajectory away from the boundary. Except at $(1/3,1/3,1/3)$ these interior trajectories are periodic: the strictly concave function $\sum_i\log x_i$ has smooth compact level curves surrounding its unique maximum, and the vector field is nonzero and tangent to each such curve.

The finite [Markov chain](../../../../../markov-chain.md) behaves differently at long times. For $P(x)=x_1x_2x_3$, the change in $P$ during the first jump is

$$
P\left(x+\frac{e_1-e_3}{N}\right)-P(x)
=x_2\left(\frac{x_3-x_1}{N}-\frac1{N^2}\right).
$$

The other two terms are cyclic permutations. Their first-order contributions cancel, leaving the exact [product decay in a cyclic imitation chain](../../../../../product-decay-in-a-cyclic-imitation-chain.md) identity

$$
\boxed{\mathcal L_NP=-\frac3NP,\qquad
\mathbb E P(X^N_t)=e^{-3t/N}\mathbb E P(X^N_0).}
$$

For $N\geq3$, while all three counts are positive, their product is at least $N-2$, so $P(X^N_t)\geq(N-2)/N^3$. A missing type cannot reappear. If $\tau$ is the first loss of a type, then

$$
\mathbb P(\tau>t)\leq\frac{N^3}{N-2}\,e^{-3t/N}\mathbb E P(X^N_0)\longrightarrow0.
$$

Once only two types remain, one always wins, so its count increases until an absorbing monochromatic vertex is reached, almost surely in finite time. The cases of one or two initially present types follow the same argument without the first stage. **Every finite chain eventually becomes monochromatic, whereas an interior deterministic solution retains its positive product.** The [fluid limit](../../../../../fluid-limit.md) holds on each fixed finite interval; it does not justify exchanging the limits $N\to\infty$ and $t\to\infty$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
