<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\mathbf X$ be a [weak geometric p-rough path](../../../../../../weak-geometric-p-rough-path.md), $N=\lfloor p\rfloor$, with increments $X^I_{s,t}$ indexed by words $I=(i_1,\ldots,i_k)$ of length at most $N$. Choose a [control function for rough paths](../../../../../../control-function-for-rough-paths.md) $\omega$ with $|X^I_{s,t}|\leq\omega(s,t)^{|I|/p}$. We use the standard sufficient vector-field hypothesis $V_i\in\operatorname{Lip}^\gamma$, $\gamma>p$, with globally bounded regularity norms; smooth bounded fields are a special case. Regard $V_i$ as the differential operator $V_i\cdot\nabla$, and put $F_I=V_{i_1}\cdots V_{i_k}\operatorname{id}$.

A [pathlevel solution of a rough differential equation](../../../../../../pathlevel-solution-of-a-rough-differential-equation.md) is a continuous state path $y:[0,T]\to\mathbb R^e$, with prescribed $y_0$, satisfying a local expansion

$$
y_t-y_s=\sum_{1\leq|I|\leq N}F_I(y_s)X^I_{s,t}+R_{s,t},\qquad |R_{s,t}|\leq C\omega(s,t)^\theta
$$

for some $\theta>1$ on sufficiently small control intervals. One can take $\theta=\min(\gamma,N+1)/p>1$ under the stated regularity. This definition specifies the state path, without requiring its full rough-path enhancement as additional data. For $2<p<3$, the displayed expansion reads

$$
y_t-y_s=V_i(y_s)X^i_{s,t}+DV_j(y_s)V_i(y_s)X^{ij}_{s,t}+R_{s,t}.
$$

Repeated indices are summed.

We use the following discrete form of the [Davie lemma](../../../../../../davie-discrete-sewing-lemma.md). For a finite ordered grid and a continuous superadditive control, suppose nonnegative errors $a_{s,t}$ vanish on adjacent grid points and, for every grid triple $s<u<t$, satisfy

$$
a_{s,t}\leq a_{s,u}+a_{u,t}+L\omega(s,t)^{1/p}a_{s,u}+A\omega(s,t)^\theta,\qquad\theta>1.
$$

There are $\delta>0$ and $C$, depending on $L,A,p,\theta$ but not on the grid, such that $a_{s,t}\leq C\omega(s,t)^\theta$ whenever $\omega(s,t)\leq\delta$. This is the discrete higher-order error estimate: splitting close to half the control size makes the two $\theta$-power errors contract; a crossing single grid interval contributes zero adjacent error.

Define the local Euler map

$$
E_{s,t}(z)=z+\sum_{1\leq|I|\leq N}F_I(z)X^I_{s,t}.
$$

For small $\omega(s,t)$ it has Lipschitz constant at most $1+L\omega(s,t)^{1/p}$. Taylor expansion, the [Chen identity](../../../../../../chen-identity.md) and the [shuffle identity for iterated integrals](../../../../../../shuffle-identity-for-iterated-integrals.md) give the composition estimate

$$
|E_{u,t}(E_{s,u}(z))-E_{s,t}(z)|\leq A\omega(s,t)^\theta.
$$

Here is the cancellation underlying the estimate. Assign degree $k$ to a level-$k$ increment. Expanding each $F_I(E_{s,u}(z))$ and grouping terms through degree $N$ gives the differential-operator coefficients $F_{IJ}(z)$ multiplying $X^I_{s,u}X^J_{u,t}$. Products of coefficients from the first increment are combined by the shuffle identity, which is the iterated Leibniz rule. Chen's identity says that the sum of these products is $X^{IJ}_{s,t}$. Thus every term of degree at most $N$ agrees with the corresponding term in $E_{s,t}$. The remaining Taylor terms have control order at least $\theta$; bounded $\operatorname{Lip}^\gamma$ norms make the estimate uniform in $z$. For smooth fields the remainder has order $(N+1)/p$.

On a partition $\pi$, construct the Euler sequence by $y^\pi_{t_{j+1}}=E_{t_j,t_{j+1}}(y^\pi_{t_j})$. For grid endpoints let

$$
I^\pi_{s,t}=y^\pi_t-E_{s,t}(y^\pi_s).
$$

It vanishes on adjacent points. Insert $y^\pi_u=E_{s,u}(y^\pi_s)+I^\pi_{s,u}$ into the next local map. The Lipschitz and composition estimates give

$$
|I^\pi_{s,t}|\leq|I^\pi_{u,t}|+(1+L\omega(s,t)^{1/p})|I^\pi_{s,u}|+A\omega(s,t)^\theta.
$$

The [Davie lemma](../../../../../../davie-discrete-sewing-lemma.md) therefore yields a bound $|I^\pi_{s,t}|\leq C\omega(s,t)^\theta$ independent of $\pi$ on small control intervals. Together with the Euler expansion this gives $|y^\pi_t-y^\pi_s|\leq C'\omega(s,t)^{1/p}$. A finite subdivision into small-control intervals gives a uniform global bound as well.

Interpolate each Euler sequence linearly in time, and take partitions with mesh tending to zero. Continuity of the control makes these paths uniformly equicontinuous: the grid estimates apply to the interval enlarged to its neighboring grid endpoints, and the enlargement tends to zero uniformly with the mesh. The paths are uniformly bounded. The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) supplies a uniformly convergent subsequence with continuous limit $y$.

For arbitrary $s<t$ in a small control interval, choose neighboring grid endpoints converging to $s,t$. Continuity of $\mathbf X$, the coefficient functions and the control lets us pass to the limit in the grid error estimate. We obtain the defining expansion with $|R_{s,t}|\leq C\omega(s,t)^\theta$, and $y(0)=y_0$. **This constructs a pathlevel RDE solution.** No continuity theorem for the RDE solution map was used to obtain existence.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
