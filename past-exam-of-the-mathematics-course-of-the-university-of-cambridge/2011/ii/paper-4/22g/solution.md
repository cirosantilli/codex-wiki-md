<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

[Urysohn's lemma](../../../../../urysohn-s-lemma.md) states that disjoint closed subsets $A,B$ of a normal space admit a continuous $u:X\to[0,1]$ with $u|_A=0$ and $u|_B=1$. Using the usual convention, normal spaces are also $T_1$.

The [Tietze extension theorem](../../../../../tietze-extension-theorem.md) states that a continuous real-valued function on a closed subset of a normal space extends continuously to the whole space. If its range lies in a closed bounded interval, the extension may be chosen in that same interval.

Prove first the interval version for $f:S\to[-1,1]$. If a continuous residual $r$ on $S$ obeys $|r|\le M$, the sets $\{r\le-M/3\}$ and $\{r\ge M/3\}$ are disjoint closed subsets of $X$. [Urysohn's lemma](../../../../../urysohn-s-lemma.md) gives a continuous $h:X\to[-M/3,M/3]$ taking the endpoint values on those two sets. On each of the three ranges of $r$, it follows that $|r-h|\le2M/3$ on $S$. Repeating with $M_j=(2/3)^j$ produces $h_j$ with $\|h_j\|_\infty\le M_j/3$ and a residual bounded by $M_{j+1}$. The series $\widetilde f=\sum_{j\ge0}h_j$ converges uniformly, has absolute value at most $\sum M_j/3=1$, is continuous and restricts to $f$ as the residual tends to zero. Rescaling proves every closed bounded interval version.

For unbounded $f$, first extend $f/(1+|f|)$ to $g:X\to[-1,1]$. The [closed set](../../../../../closed-set.md) $B=g^{-1}(\{-1,1\})$ is disjoint from $S$. [Urysohn's lemma](../../../../../urysohn-s-lemma.md) gives $\psi:X\to[0,1]$ with $\psi|_S=1$ and $\psi|_B=0$. Then $h=\psi g$ takes values strictly between minus one and one everywhere and equals $f/(1+|f|)$ on $S$. Thus $h/(1-|h|)$ is a continuous real-valued extension of $f$, proving the full theorem.

**Statement 1 is true:** [metric spaces](../../../../../metric-space.md) are normal, and the bounded interval form applies. **Statement 2 is true:** [compact Hausdorff spaces](../../../../../compact-hausdorff-space.md) are normal, and the unrestricted real-valued form applies. **Statement 3 is false.** For a counterexample, let $X=\{a,b,c\}$ have open sets $\varnothing,\{a\},\{a,b\},\{a,c\},X$. The subset $S=\{b,c\}$ is closed and discrete, so $f(b)=-1$, $f(c)=1$ is continuous on it. Every open neighborhood of $b$ or $c$ in $X$ contains $a$. A continuous extension would pull back disjoint neighborhoods of minus one and one to disjoint open sets containing $b$ and $c$, yet both would contain $a$. This is impossible.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
