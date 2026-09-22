<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [lower shadow](../../../../../lower-shadow.md) consists of the sets obtained by removing one element from a member:

$$
\partial\mathcal A=\{S:|S|=r-1,\ S\subset A\text{ for some }A\in\mathcal A\}.
$$

For a nonempty [uniform set family](../../../../../uniform-set-family.md), write its size in its unique decreasing [binomial coefficient](../../../../../binomial-coefficient.md) expansion

$$
|\mathcal A|=\binom{a_r}{r}+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_t}{t},
\qquad a_r>a_{r-1}>\cdots>a_t\geq t.
$$

The [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) states that

$$
\boxed{|\partial\mathcal A|\geq\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_t}{t-1}.}
$$

A [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) attains equality; thus this is an exact minimum, not just an asymptotic estimate.

Here is a direct proof of the requested [Lovász shadow bound](../../../../../lovasz-shadow-bound.md), avoiding any unproved numerical interpolation of the [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md). The real [binomial coefficient](../../../../../binomial-coefficient.md) means $\binom{x}{r}=x(x-1)\cdots(x-r+1)/r!$. It is strictly increasing for $x>r-1$. Since the [set family](../../../../../set-family.md) is nonempty and its size is an integer, necessarily $x\geq r$.

Apply the usual left [coordinate shifts of a set family](../../../../../coordinate-shifts-of-a-set-family.md) until the [set family](../../../../../set-family.md) is fixed by every shift. A shift preserves its size and does not increase its [lower shadow](../../../../../lower-shadow.md); the witness argument is supplied in Solution 3. Termination follows because every nontrivial shift reduces $\sum_{A\in\mathcal A}\sum_{i\in A}i$. It suffices to prove the inequality for this shifted [set family](../../../../../set-family.md).

Induct on $r$, and, for each fixed $r$, on $|\mathcal A|$. The cases $r=1$ and $|\mathcal A|=1$ give, respectively, the single empty shadow member and the $r$ faces of an $r$-set. Split the [set family](../../../../../set-family.md) at coordinate one, writing $\mathcal A_0$ for the members avoiding it and $\mathcal A_1$ for the sets obtained by deleting it from members containing it. Every $(r-1)$-subset of a member of $\mathcal A_0$ belongs to $\mathcal A_1$: replace the one omitted coordinate by coordinate one. Therefore

$$
\partial\mathcal A_0\subseteq\mathcal A_1,
\qquad |\partial\mathcal A|=|\mathcal A_1|+|\partial\mathcal A_1|.
$$

The two terms count shadow members avoiding and containing coordinate one.

Put $b=|\mathcal A_1|$. This is positive. If $b<\binom{x-1}{r-1}$, the [Pascal's identity](../../../../../pascal-s-rule.md) gives $|\mathcal A_0|>\binom{x-1}{r}$. In this case $x>r$ and $\mathcal A_0$ is a smaller nonempty [set family](../../../../../set-family.md). The [mathematical induction](../../../../../mathematical-induction.md) hypothesis on family size gives $|\partial\mathcal A_0|>\binom{x-1}{r-1}$, contradicting its containment in $\mathcal A_1$. Consequently $b\geq\binom{x-1}{r-1}$. Write $b=\binom{z}{r-1}$, so $z\geq x-1$. The [mathematical induction](../../../../../mathematical-induction.md) hypothesis on uniformity and the [Pascal's identity](../../../../../pascal-s-rule.md) now give

$$
|\partial\mathcal A|\geq\binom{z}{r-1}+\binom{z}{r-2}
\geq\binom{x-1}{r-1}+\binom{x-1}{r-2}
=\boxed{\binom{x}{r-1}}.
$$

For $r=2$ the degree-zero term is the constant one, which causes no difficulty.

For the graph application, identify a [triangle-free graph](../../../../../triangle-free-graph.md) with a subset of the $N$ possible edges. Removing an edge preserves being [triangle-free](../../../../../triangle-free-graph.md), so $\partial\mathcal G_{m+1}\subseteq\mathcal G_m$. If $\mathcal G_{m+1}$ is nonempty, the [Lovász shadow bound](../../../../../lovasz-shadow-bound.md) gives

$$
\binom{x_{m+1}}m\leq|\partial\mathcal G_{m+1}|\leq|\mathcal G_m|=\binom{x_m}m,
\qquad x_{m+1}\leq x_m.
$$

Thus, for $1\leq m<N$ with $p_m>0$,

$$
|\mathcal G_{m+1}|\leq\binom{x_m}{m+1},
\qquad
\boxed{\frac{p_{m+1}}{p_m}\leq\frac{x_m-m}{N-m}}.
$$

If the next [set family](../../../../../set-family.md) is empty its probability is zero, so the same inequality holds without introducing $x_{m+1}$. If $p_m=0$, every later [set family](../../../../../set-family.md) is empty; the divided expression is undefined and the correct assertion is this zero-probability conclusion.

Iterate the monotonicity of the [effective ground-set parameter of a hereditary uniform layer](../../../../../effective-ground-set-parameter-of-a-hereditary-uniform-layer.md). Whenever $p_{m+k}>0$, all the intermediate parameters are at least their layer sizes, and all factors below are nonnegative. We obtain the stronger estimate

$$
p_{m+k}\leq p_m\prod_{j=0}^{k-1}\frac{x_m-m-j}{N-m-j}
\leq\boxed{p_m\prod_{j=0}^{k-1}\frac{x_m-j}{N-j}}.
$$

The second inequality follows from $x_m\leq N$ and the fact that $(x_m-t)/(N-t)$ decreases with $t$. If the target [set family](../../../../../set-family.md) is empty, the requested bound follows directly when its right side is nonnegative. When $k>x_m+1$, the printed product can have signed factors and should instead be stopped at the first empty layer: its unrestricted signed form is not a meaningful probability bound. In the nonzero target range there is no such ambiguity. A uniformly safe extension, for $0\leq k\leq N-m$, is

$$
\boxed{p_{m+k}\leq p_m\prod_{j=0}^{k-1}\frac{(x_m-j)_+}{N-j}},\qquad t_+=\max\{t,0\}.
$$

It agrees with the printed expression whenever all its factors are nonnegative. In particular $0\leq k\leq m$ is always safe when $p_m>0$, and this includes the requested doubling case.

Taking $k=m$ in the nonzero range,

$$
\prod_{j=0}^{m-1}\frac{x_m-j}{N-j}=\frac{\binom{x_m}m}{\binom Nm}=p_m,
\qquad \boxed{p_{2m}\leq p_m^2\leq\tfrac14}.
$$

If the $2m$-edge [set family](../../../../../set-family.md) is empty the conclusion is immediate; if $2m>N$, interpreting the event as impossible gives the same conclusion. These qualifications distinguish the probability assertion from products or ratios outside their domains.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
