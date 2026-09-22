<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

For a state $i$, let $N_i=\{n\geq1:P^n_{ii}>0\}$ and $d_i=\gcd N_i$. If distinct states $i,j$ communicate, choose positive-probability paths $i\to j$ and $j\to i$ of lengths $r,s$. Then $r+s$ is a return time to each. For every $n\in N_i$, concatenate $j\to i$, the $i$-return loop, and $i\to j$ to see that $s+n+r\in N_j$. Since $d_j$ divides this and $s+r$, it divides $n$. Thus $d_j\mid d_i$, and interchanging the states gives $d_i\mid d_j$. This proves **[period is constant on a communicating class](../../../../../period-is-constant-on-a-communicating-class.md)**.

Read the transition matrix from the original PDF; the converted TeX loses the location of the second row's final entry. The [communicating classes](../../../../../communicating-class.md) are

$$
\boxed{\{1,3,4\},\quad\{2,7\},\quad\{6\},\quad\{5\}}.
$$

Within $\{1,3,4\}$ the only internal cycle is $1\to3\to4\to1$. Return lengths are multiples of three, and length three has positive probability, so its period is three. This class is open because it has exits to other classes. The class $\{2,7\}$ is the closed deterministic two-cycle, of period two. The absorbing class $\{6\}$ is closed and has period one.

State 5 has outgoing transitions but no incoming transition at all, so it is an open singleton class and $N_5=\varnothing$. For this [return-free state in a Markov chain](../../../../../return-free-state-in-a-markov-chain.md), the convention $\gcd\varnothing=0$ gives **period zero**; if period is defined only when positive return times exist, it is undefined instead. In particular, this singleton is not aperiodic: aperiodicity would require period one.

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
