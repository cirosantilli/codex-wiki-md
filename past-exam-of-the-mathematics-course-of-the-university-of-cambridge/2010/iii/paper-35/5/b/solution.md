<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $L$ be the set of left-shoe owners and $R$ the right-shoe owners. This is the [glove game](../../../../../../glove-game.md) with pair price ten, so its [characteristic function of a coalitional game](../../../../../../characteristic-function-of-a-coalitional-game.md) is

$$
v(S)=10\min\{|S\cap L|,|S\cap R|\}.
$$

All singleton values are zero. Write $\ell_i\geq0$ for left-owner payoffs and $r_j\geq0$ for right-owner payoffs. Efficiency gives total $10\min(a,b)$, and each mixed pair imposes $\ell_i+r_j\geq10$.

Suppose $a<b$. Removing any right owner leaves at least $a$ right shoes, so the complement coalition still has value $10a$. Its core inequality and efficiency imply $r_j\leq0$. Thus every right owner receives zero. The pair constraints then force $\ell_i\geq10$, and their total is $10a$, so every left owner receives ten. Conversely this allocation gives each coalition $10|S\cap L|$, at least its value, so it is in the core. The argument is symmetric when $a>b$.

When $a=b=k$, sum all $k^2$ mixed-pair inequalities. Their total left side is $k$ times the grand-coalition payoff, namely $10k^2$. Hence every inequality is equality: $\ell_i+r_j=10$ for every pair. Fixing one right owner shows all left payoffs are the same $\theta$, and fixing one left owner shows all right payoffs are $10-\theta$. Individual rationality gives $0\leq\theta\leq10$. Such allocations are sufficient: for a coalition with $u$ left owners and $v$ right owners,

$$
\theta u+(10-\theta)v\geq10\min(u,v),
$$

as is seen by subtracting the right side and factoring either $\theta(u-v)$ or $(10-\theta)(v-u)$.

The [core of a glove game](../../../../../../core-of-a-glove-game.md) is therefore

$$
\boxed{\begin{array}{c|cc}
&\text{each left owner}&\text{each right owner}\\\hline
a<b&10&0\\
a>b&0&10\\
a=b&\theta&10-\theta,\quad 0\leq\theta\leq10
\end{array}.}
$$

Payoffs are in pounds. The parameter in the balanced case is common to all owners of a given shoe type.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
