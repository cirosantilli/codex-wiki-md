<h1 id="25k/solution">Solution</h1>

↑ **Parent:** [25K](../25k.md)

Assume nonnegative wealth and rewards, and initially $0<p_i\leq1$. Set $F_0(x)=x$, and let $R_i$ take the values $0,2a_i$ with equal probability conditional on not being caught. For the [retirement threshold with multiplicative capture risk](../../../../../retirement-threshold-with-multiplicative-capture-risk.md), the [dynamic programming](../../../../../dynamic-programming.md) equation is the displayed maximum; capture contributes zero. Write $t=\max_i a_iq_i/p_i$.

Inductively, if $x\geq t$, all future successful wealth levels also lie above $t$, so $F_{s-1}(x+R_i)=x+R_i$. Continuing in town $i$ is then worth $q_i(x+a_i)\leq x$, and retirement is optimal. If $x<t$, choose $i$ with $a_iq_i/p_i>x$. Continuing for just one night and then retiring is worth $q_i(x+a_i)>x$, so immediate retirement cannot be optimal for any $s\geq1$. This proves **an optimal policy continues exactly when** $\boxed{x<t}$, with retirement chosen at the threshold.

Now suppose $q_1>q_2$ and $q_1a_1>q_2a_2$. Since also $p_1<p_2$, town $1$ has the larger threshold, so $t=a_1q_1/p_1$. The functions $F_s$ are nondecreasing in wealth and in $s$, and $F_s(x)\geq x$; these properties follow by induction from the dynamic programming equation.

Prove by induction on the remaining horizon that town $2$ is never optimal when continuation is worthwhile. For $s=1$, the difference between the town values is $(q_1-q_2)x+q_1a_1-q_2a_2>0$. If $a_2\leq a_1$, monotonicity gives

$$
\frac{q_1}2[F_{s-1}(x)+F_{s-1}(x+2a_1)]>\frac{q_2}2[F_{s-1}(x)+F_{s-1}(x+2a_2)],
$$

with strictness because the first bracket is positive under the hypotheses.

For $a_2>a_1$, first suppose $x+2a_2\geq t$. The second town's successful large-reward branch retires, so its value is $q_2[F_{s-1}(x)+x+2a_2]/2$. Town $1$ is worth at least $q_1[F_{s-1}(x)+x+2a_1]/2$. Their difference is at least

$$
\frac{q_1-q_2}{2}[F_{s-1}(x)+x]+q_1a_1-q_2a_2>0.
$$

If instead $x+2a_2<t$, all states after either first-night reward remain below the threshold. By induction a policy starting in town $2$ then chooses town $1$ on its second night. Its value is

$$
q_2q_1\mathbb E F_{s-2}(x+R_2+R_1).
$$

Interchanging the first two towns gives exactly the same value, because capture probabilities multiply and independent rewards add. After starting in town $1$, however, the induction hypothesis says town $2$ is strictly inferior on the second night at every possible surviving wealth level. Replacing that second choice by the optimal one strictly improves the value. This proves **town $1$ dominates throughout every finite horizon**.

If a town has $p_i=0$ and $a_i>0$, its threshold is interpreted as infinity and retirement is not optimal before the horizon ends. A town with $q_i a_i=0$ offers no gain; the natural threshold is zero. These conventions handle the degenerate capture probabilities rather than dividing by zero.

## ↑ Ancestors (10)

1. [25K](../25k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
