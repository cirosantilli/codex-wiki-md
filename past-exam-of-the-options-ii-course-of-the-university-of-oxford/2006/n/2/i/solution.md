<h1 id="n/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [state space](../../../../../state-space.md) is $\{0,1,2,\ldots\}$. Write $q=1-p$. The nonzero transition probabilities are

$$
P(0,1)=1,\qquad P(j,0)=p,\quad P(j,j+1)=q\quad(j\geq1).
$$

The stationary equations give $\pi_1=\pi_0$ and $\pi_j=q^{j-1}\pi_0$ for $j\geq1$. Normalization gives $\pi_0[1+\sum_{j\geq1}q^{j-1}]=\pi_0(1+1/p)=1$, so

$$
\boxed{\pi_0=\frac p{1+p},\qquad
\pi_j=\frac{p(1-p)^{j-1}}{1+p}\quad(j\geq1).}
$$

The remaining equation $\pi_0=p\sum_{j\geq1}\pi_j$ is satisfied, confirming stationarity.

The chain is [irreducible](../../../../../irreducible-representation.md): every positive state can jump to zero, and zero can reach every state through consecutive immigration steps. A stationary probability distribution makes it [positive recurrent](../../../../../positive-recurrent-markov-chain.md). Returns to zero can have lengths two and three with positive probability, so it is also [aperiodic](../../../../../aperiodic-markov-chain.md). The Markov-chain ergodic theorem now gives the almost-sure long-run time proportion for $X_n>K$ as the stationary tail:

$$
\boxed{\sum_{j=K+1}^\infty\pi_j=\frac{(1-p)^K}{1+p}.}
$$

This time-average conclusion applies to the specified start at zero.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [N](../../../n.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
