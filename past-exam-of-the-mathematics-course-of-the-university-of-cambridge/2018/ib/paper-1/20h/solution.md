<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Let the [Markov chain](../../../../../markov-chain.md) state after each toss be $(S,I)$, where $S$ is player $A_1$'s net winnings and $I$ is the next player to toss. From $(S,i)$ it moves to $(S+1,1)$ with probability $p_i$ and to $(S-1,2)$ with probability $q_i=1-p_i$. The initial state is $(0,1)$, and a return means hitting any state with $S=0$ at positive time.

From $(1,1)$, the probability of hitting zero is

$$
r_+=\begin{cases}1,&p_1+p_2\leq1,\\q_1/p_2,&p_1+p_2>1.\end{cases}
$$

Indeed, in the positive-drift case the bounded harmonic solution of

$$
h_1(x)=p_1h_1(x+1)+q_1h_2(x-1),\qquad
h_2(x)=p_2h_1(x+1)+q_2h_2(x-1)
$$

uses the decaying root $q_2/p_1$ and boundary value $h_2(0)=1$, yielding $h_1(1)=q_1/p_2$; with nonpositive drift the walk hits zero surely. By the reflected argument, from $(-1,2)$ the probability is

$$
r_-=\begin{cases}p_2/q_1,&p_1+p_2<1,\\1,&p_1+p_2\geq1.\end{cases}
$$

Conditioning on the first toss, the required return probability is

$$
\boxed{
p_1r_++q_1r_-=
\begin{cases}
p_1+p_2,&p_1+p_2\leq1,\\[3pt]
\dfrac{(1-p_1)(p_1+p_2)}{p_2},&p_1+p_2\geq1.
\end{cases}}
$$

Both formulas equal one at the boundary $p_1+p_2=1$.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
