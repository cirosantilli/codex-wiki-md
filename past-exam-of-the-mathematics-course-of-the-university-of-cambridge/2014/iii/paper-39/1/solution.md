<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $S=R+\delta$ and let $C_i=\delta+\sum_{j\ne i}b_j$. Player $i$'s payoff in the [proportional contest with outside effort](../../../../../proportional-contest-with-outside-effort.md) is $u_i(b)=v_i b/(b+C_i)-b$. When $C_i>0$, this is strictly [concave](../../../../../concave-function.md) and

$$
u_i'(b)=\frac{v_iC_i}{(b+C_i)^2}-1.
$$

The [best response](../../../../../best-response.md) is zero when $v_i\leq C_i$, and otherwise is $\sqrt{v_iC_i}-C_i$. Thus the nonnegative-effort [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) at a [pure strategy](../../../../../pure-strategy.md) [Nash equilibrium](../../../../../nash-equilibrium.md) give

$$
\boxed{b_i=S\left(1-\frac S{v_i}\right)>0\quad\text{if }v_i>S,\qquad b_i=0\quad\text{if }v_i\leq S.}
$$

For an active player the first-order equation is $v_i(S-b_i)=S^2$. For an inactive player the derivative at zero is $v_i/S-1$. Strict [concavity](../../../../../concave-function.md) makes these conditions sufficient as well as necessary.

If $\delta=0$, an equilibrium cannot have just one active player: that player would win with certainty and could lower its positive effort. An all-zero profile also cannot be an equilibrium under the usual completion of proportional allocation at zero: at least one player can gain by investing an arbitrarily small amount. Consequently there are at least two active players, so every $C_i$ is positive. If $\delta>0$ this positivity is automatic. The allocation rule's otherwise undefined all-zero value at $\delta=0$ is therefore immaterial to the equilibrium calculation.

Let $k=\hat n>0$, $H_k=\sum_{i=1}^k1/v_i$, and use the [harmonic mean](../../../../../harmonic-mean.md) $\bar v_k=k/H_k$. Summing the active efforts gives

$$
R=kS-H_kS^2=S-\delta,
\qquad H_kS^2-(k-1)S-\delta=0.
$$

The positive root supplies the [total-effort formula for a proportional contest with outside effort](../../../../../total-effort-formula-for-a-proportional-contest-with-outside-effort.md):

$$
\boxed{R=\frac{\bar v_k}{2k}\left[(k-1)+\sqrt{(k-1)^2+\frac{4k\delta}{\bar v_k}}\right]-\delta.}
$$

At $\delta=0$ this reduces to $R=(k-1)\bar v_k/k$. There is also a genuine zero-active case: **if $\delta\geq v_1$, then $k=0$ and $R=0$**; no [harmonic mean](../../../../../harmonic-mean.md) of an empty family is needed.

For a fully explicit active-set rule, set

$$
G(s)=\sum_{i=1}^n\left(1-\frac{s}{v_i}\right)_+-1+\frac\delta s,
\qquad s>0.
$$

The equilibrium equation is $G(S)=0$. For $\delta>0$, $G$ is strictly decreasing from $+\infty$ to $-1$. For $\delta=0$ its limit at zero is $n-1>0$, and it is strictly decreasing wherever a zero could occur. Hence the positive root is unique. Moreover $S\geq\delta$, since its equation gives $1-\delta/S\geq0$, and $b_i=S(1-S/v_i)_+$ supplies an equilibrium with total effort $S-\delta$.

Player $j$ is active exactly when $v_j>S$, equivalently $G(v_j)<0$. Ordering the valuations, including ties, gives

$$
G(v_j)=j-2-\sum_{i<j}\frac{v_j}{v_i}+\frac\delta{v_j}.
$$

Therefore the [active-set threshold for a proportional contest with outside effort](../../../../../active-set-threshold-for-a-proportional-contest-with-outside-effort.md) is

$$
\boxed{\hat n=\max\left(\{0\}\cup\left\{j\in\{1,\ldots,n\}:\
\delta<v_j\left(2-j+\sum_{i<j}\frac{v_j}{v_i}\right)\right\}\right).}
$$

The qualifying indices form a prefix because $G$ is decreasing. Equality excludes the marginal player, as required by strict positivity of effort. Equivalently, the positive root $S_k$ of the displayed quadratic must satisfy $v_k>S_k\geq v_{k+1}$, with $v_{n+1}=0$. These formulas include one active player when $\delta>0$ and exclude that case when $\delta=0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
