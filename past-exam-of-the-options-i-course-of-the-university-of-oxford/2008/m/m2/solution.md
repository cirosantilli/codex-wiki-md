<h1 id="m/m2/solution">Solution</h1>

↑ **Parent:** [M2](../m2.md)

The [Markov property](../../../../markov-property.md) says that conditional on the present state, the next-state law does not depend on the earlier history. For this time-homogeneous chain, $\mathbb P(X_{n+1}=j\mid X_0=i_0,\ldots,X_n=i)=p_{ij}$ whenever the conditioning event has positive probability.

States communicate when each is accessible from the other by a finite positive-probability path; the equivalence classes are the [communicating classes](../../../../communicating-class.md). A class is closed if no one-step transition leaves it, and open otherwise. Probability nonnegativity adds the implicit restriction $p\geq0$ to the printed upper bound.

At $p=0$, every state is absorbing, so the classes are the singletons, all closed. For $0<p\leq1/2$, every neighbouring pair communicates, so the whole state space is one closed class, making the chain [irreducible](../../../../irreducible-markov-chain.md). There are no open classes in either case.

For $m=3$ and $p>0$, [detailed balance](../../../../detailed-balance.md) along the path gives $2p\pi_0=p\pi_1$, $\pi_1=\pi_2$, and $p\pi_2=2p\pi_3$. After normalization,

$$
\boxed{\pi=(1,2,2,1)/6}.
$$

For $0<p<1/2$, the self-loops have positive probability; the finite irreducible chain is [aperiodic](../../../../aperiodic-markov-chain.md), so $\mathbb P_i(X_n=j)\to\pi_j$ for all fixed starting states and targets. For $p=1/2$, every step changes parity. The chain has period two, and for each fixed $i,j$ one parity of times has probability zero while $\pi_j>0$. Thus the stated convergence from a fixed starting state holds **exactly when $0<p<1/2$**. This is the [stationary law of a reflecting nearest-neighbor walk on a finite path](../../../../stationary-law-of-a-reflecting-nearest-neighbor-walk-on-a-finite-path.md).

## ↑ Ancestors (12)

1. [M2](../m2.md)
2. [M](../../m.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
