<h1 id="n/n2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an irreducible [positive recurrent](../../../../../../positive-recurrent-markov-chain.md) [Markov chain](../../../../../../markov-chain-split.md), the [Markov chain ergodic theorem](../../../../../../markov-chain-ergodic-theorem.md) gives a unique [stationary distribution](../../../../../../stationary-distribution.md) $\pi$, with almost-sure long-run occupation fraction $\pi_j$ in state $j$. More generally, time averages of an integrable state reward converge to its stationary mean. If the chain is also aperiodic, then $\mathbb P_i(X_n=j)\to\pi_j$ for every initial state $i$; the aperiodicity assumption is needed for this last distributional conclusion.

For either transition rule in part (i), $0<p<1$ permits progression through the phase-A states and a return from phase B to zero. Both chains are finite and irreducible, hence [positive recurrent](../../../../../../positive-recurrent-markov-chain.md). State $K$ has a positive self-loop, so both are aperiodic. Therefore

$$
\boxed{\lim_{n\to\infty}\mathbb P(X_n=j)=\pi_j},
$$

using respectively the cumulative or consecutive [stationary distribution](../../../../../../stationary-distribution.md) given in part (i), for every starting distribution.

The excluded endpoint cases are simple: at $p=0$, phase B is eventually reached and then absorbing, so the limiting law is the point mass at $K$. At $p=1$, the cumulative rule traps the chain at its current phase-A count (or eventually at zero if started in phase B), so the limit can depend on the initial count; under the consecutive rule zero is eventually absorbing. Irreducibility and the preceding stationary formulas must not be asserted unchanged at these endpoints.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [N2](../../../n2.md)
4. [N](../../../../n.md)
5. [2004](../../../../../2004-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
