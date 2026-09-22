<h1 id="m/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Markov property](../../../../markov-property.md) says that, conditional on the present state, the next state is independent of the earlier history:

$$
\mathbb P(X_{n+1}=j\mid X_0,\ldots,X_n)=p_{X_n,j}.
$$

Two states communicate if each is reachable from the other with positive probability in finitely many steps. The equivalence classes are [communicating classes](../../../../communicating-class.md); a class is closed if no positive-probability transition leaves it.

The displayed probabilities require $0\leq p\leq1/2$; negative values allowed by the printed one-sided inequality are not transition probabilities. For $p=0$, every state is an absorbing singleton, so all singleton classes are closed. For $0<p\leq1/2$, neighboring states communicate in both directions, so there is one closed irreducible class $S$ and no open classes.

For $m=3$, the [detailed balance](../../../../detailed-balance.md) relations give $2\pi_0=\pi_1=\pi_2=2\pi_3$. Normalization yields

$$
\boxed{\pi=(1/6,1/3,1/3,1/6).}
$$

For $0<p<1/2$, positive holding probabilities make the finite irreducible chain aperiodic, so its transition probabilities converge to $\pi_j$ from every initial state. At $p=1/2$, every step changes parity and the period is two; convergence from a fixed initial state fails. A stationary initial mixture still has distribution $\pi$ at every time, but this does not give convergence of the transition probabilities asked for.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [M](../../m.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
