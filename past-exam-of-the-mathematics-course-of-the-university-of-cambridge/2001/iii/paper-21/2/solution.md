<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $s_i=p_i+q_i>0$ and $d_i=p_i-q_i$ for $i=0,1$. For the parity correction $h_\theta(k)=k-\theta\mathbf1_{\{k\text{ odd}\}}$, the [conditional expectations](../../../../../conditional-expectation.md) of the increments of $h_\theta(X_n)$ are

$$
\begin{cases}
p_0(1-\theta)+q_0(-1-\theta)=d_0-\theta s_0,&X_n\text{ even},\\
p_1(1+\theta)+q_1(-1+\theta)=d_1+\theta s_1,&X_n\text{ odd}.
\end{cases}
$$

The holding move contributes zero. Thus the [period-two martingale corrector for a birth-death chain](../../../../../period-two-martingale-corrector-for-a-birth-death-chain.md) exists precisely when

$$
\boxed{\theta=\frac{d_0}{s_0}=-\frac{d_1}{s_1},\qquad \frac{d_0}{s_0}+\frac{d_1}{s_1}=0.}
$$

This is the condition that $h_\theta$ be a [harmonic function for a Markov chain](../../../../../harmonic-function-for-a-markov-chain.md). The process has integrable values from a fixed initial state because $|X_n|\leq|X_0|+n$; the [Markov property](../../../../../markov-property.md) therefore turns the zero conditional increments into the required [martingale](../../../../../martingale-split.md) property. Conversely, both parities are reached with positive [probability](../../../../../probability.md) because all right and left probabilities are positive, so the two conditional equations are necessary. Expanding their numerator also gives the equivalent balance condition $p_0p_1=q_0q_1$. Positivity makes $|\theta|<1$.

Put $L=-aN$, $U=bN$. The exit time $T_N$ is almost surely finite. Indeed, set $m=U-L$ and $p_* =\min(p_0,p_1)>0$. From any interior point, consecutive right steps reach $U$ in at most $m$ moves, with [probability](../../../../../probability.md) at least $p_*^m$. The [Markov property](../../../../../markov-property.md) gives $\mathbb P(T_N>km)\leq(1-p_*^m)^k$. This is the [finite-interval exit times have geometric tails](../../../../../finite-interval-exit-times-have-geometric-tails.md) argument. The walk cannot skip a boundary because its jumps have size at most one.

Under the balance condition, the stopped [martingale](../../../../../martingale-split.md) $h_\theta(X_{n\wedge T_N})$ is bounded, because the stopped position stays in $[L,U]$. Apply the [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $n\wedge T_N$, then [dominated convergence](../../../../../dominated-convergence-theorem.md) as $n\to\infty$. Starting from zero gives

$$
0=\pi_Nh_\theta(L)+(1-\pi_N)h_\theta(U).
$$

With $\varepsilon_a=\mathbf1_{\{aN\text{ odd}\}}$ and $\varepsilon_b=\mathbf1_{\{bN\text{ odd}\}}$,

$$
\pi_N=\frac{bN-\theta\varepsilon_b}{(a+b)N+\theta\varepsilon_a-\theta\varepsilon_b},\qquad
\boxed{\lim_{N\to\infty}\pi_N=\frac{b}{a+b}.}
$$

The bounded parity corrections disappear after division by $N$; the [holding probability of a Markov chain](../../../../../holding-probability-of-a-markov-chain.md) may be positive or zero and may differ between parities.

For failure of balance, use [scale increments for a birth-death chain](../../../../../scale-increments-for-a-birth-death-chain.md) rather than the nonexistent bounded correction. Let $u(k)$ be the upper exit [probability](../../../../../probability.md) from $k$ for boundaries $L,U$. The [Markov property](../../../../../markov-property.md) yields

$$
p_k(u(k+1)-u(k))=q_k(u(k)-u(k-1)),\qquad u(L)=0,\quad u(U)=1,
$$

where $p_k,q_k$ depend only on parity. Choose positive numbers $w_j$ with $w_{j+1}=(q_j/p_j)w_j$. Then $u(k)=\sum_{j=L+1}^k w_j/\sum_{j=L+1}^U w_j$ satisfies these equations and boundary values. Stopping this bounded harmonic function proves that it is the exit [probability](../../../../../probability.md). In particular,

$$
\pi_N=\frac{\sum_{j=1}^{bN}w_j}{\sum_{j=-aN+1}^{bN}w_j},\qquad
w_{j+2}=\rho w_j,\quad \rho=\frac{q_0q_1}{p_0p_1}.
$$

If $\rho<1$, the positive-index sum stays bounded as $N\to\infty$, while the negative-index contribution diverges geometrically, so $\pi_N\to0$. If $\rho>1$, the negative-index sum stays bounded while the positive-index sum diverges, so $\pi_N\to1$. Therefore the complete classification is

$$
\boxed{\lim_{N\to\infty}\pi_N=
\begin{cases}
0,&p_0p_1>q_0q_1,\\
b/(a+b),&p_0p_1=q_0q_1,\\
1,&p_0p_1<q_0q_1.
\end{cases}}
$$

Thus a fixed nonzero imbalance drives the macroscopic exit to the corresponding side, for every positive $a,b$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
