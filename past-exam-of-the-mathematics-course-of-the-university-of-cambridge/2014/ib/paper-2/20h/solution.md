<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Write $h_i=\mathbb P_i(H^A<\infty)$. For $i\in A$, $h_i=1$. For $i\notin A$, conditioning on the first step and using the [Markov property](../../../../../markov-property.md) gives $h_i=\sum_jp_{ij}h_j$. This establishes the required equations for the [hitting probability](../../../../../hitting-probability.md).

To prove the [hitting probability is the minimal nonnegative harmonic extension](../../../../../hitting-probability-is-the-minimal-nonnegative-harmonic-extension.md), let $h_i^{(n)}=\mathbb P_i(H^A\le n)$. Then $h^{(0)}=\mathbf1_A$ and

$$
h_i^{(n+1)}=
\begin{cases}
1,&i\in A,\\
\sum_jp_{ij}h_j^{(n)},&i\notin A.
\end{cases}
$$

If $g$ is any nonnegative solution of the same boundary equations, $g\ge h^{(0)}$. Positivity of the transition probabilities implies by induction $g\ge h^{(n)}$ for every $n$. The events $\{H^A\le n\}$ increase to $\{H^A<\infty\}$, so $h^{(n)}\uparrow h$ and $g\ge h$. Therefore **$h$ is the minimal nonnegative solution**.

For the [tournament won by two consecutive victories](../../../../../tournament-won-by-two-consecutive-victories.md), a transient pair $ij$, with $i\ne j$ and third player $k$, moves with equal probabilities to the [absorbing state](../../../../../absorbing-state.md) $jj$ or the transient pair $jk$. Thus the two transient cycles are

$$
AB\longrightarrow BC\longrightarrow CA\longrightarrow AB,\qquad
AC\longrightarrow CB\longrightarrow BA\longrightarrow AC,
$$

with probability $1/2$ of absorption at each step. A full cycle without absorption has probability $1/8$, so absorption occurs almost surely.

Starting from $AC$, the successive absorption winners are $C,B,A$, with first-cycle probabilities $1/2,1/4,1/8$. Summing the geometric repetitions gives

$$
\mathbb P(\text{winner}=A,B,C\mid AC)=(1/7,2/7,4/7).
$$

Starting from $BC$, the order is $C,A,B$, giving $(2/7,1/7,4/7)$.

Because the first game is between $A$ and $B$, the initial ordered pair of winners is $AA,AC,BB,BC$, each with probability $1/4$. Combining the immediate wins with the transient [hitting probabilities](../../../../../hitting-probability.md),

$$
\boxed{\mathbb P(A\text{ wins})=\frac5{14},\qquad
\mathbb P(B\text{ wins})=\frac5{14},\qquad
\mathbb P(C\text{ wins})=\frac27.}
$$

Their sum is one, consistent with almost-sure absorption.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
