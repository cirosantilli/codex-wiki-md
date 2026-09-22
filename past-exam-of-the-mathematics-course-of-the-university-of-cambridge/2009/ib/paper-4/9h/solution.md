<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

Use coordinates $(i,j)\in\{0,\ldots,7\}^2$, with the starting corner $(0,0)$. The bishop stays on the 32 squares where $i+j$ is an [even number](../../../../../even-number.md). Its moves form a [random walk on a graph](../../../../../random-walk-on-a-graph.md), with an edge between distinct squares whenever $|i-i'|=|j-j'|$. If $d(i,j)$ is the number of reachable squares, the transition probability to each neighbor is $1/d(i,j)$.

The graph is connected: from $(i,j)$ move along its antidiagonal to $((i+j)/2,(i+j)/2)$, then along the main diagonal to the corner. The midpoint coordinates are [integers](../../../../../integer.md) because $i+j$ is an [even number](../../../../../even-number.md), and this square always lies on the board. Thus this is the full communicating state space of the [bishop random walk](../../../../../bishop-random-walk.md).

The [invariant distribution](../../../../../stationary-distribution.md) is proportional to degree. Its normalizing constant can be counted by summing the ordered pairs along each diagonal. The diagonals of one orientation have lengths $8,6,6,4,4,2,2$, contributing $144$; the other have lengths $1,3,5,7,7,5,3,1$, contributing $136$. Therefore

$$
\boxed{\pi(i,j)=\frac{d(i,j)}{280}.}
$$

For any neighboring states $s,t$, $\pi(s)P(s,t)=1/280=\pi(t)P(t,s)$, proving the [detailed balance](../../../../../detailed-balance.md) equations and hence that the chain is a [reversible Markov chain](../../../../../reversible-markov-chain.md).

The corner has seven neighbors. [Kac's lemma](../../../../../kac-s-lemma.md) gives its expected first positive return time:

$$
\boxed{\mathbb E_{(0,0)}T_{(0,0)}^+=\frac1{\pi(0,0)}=\frac{280}{7}=40\text{ moves}.}
$$

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
