<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $X_j$ be the [indicator random variable](../../../../../../indicator-random-variable.md) that coin $j$ shows a head. Each [expectation](../../../../../../expected-value-split.md) is $\mathbb E X_j=1/2$, so [linearity of expectation](../../../../../../linearity-of-expectation.md) gives the expected number of heads:

$$
\boxed{\mathbb E\left[\sum_{j=1}^nX_j\right]=\frac n2.}
$$

For the game, write $p_i$ for the [probability](../../../../../../probability.md) that $H$ eventually holds all $n$ coins when starting with $i$. The states $0,n$ are absorbing, so $p_0=0$ and $p_n=1$. Conditioning on the first toss and using the [law of total probability](../../../../../../law-of-total-probability.md) gives

$$
p_i=\frac12p_{i-1}+\frac12p_{i+1},\qquad 1\le i\le n-1.
$$

Thus $p_{i+1}-p_i=p_i-p_{i-1}$: successive differences are constant, and $p_i=A+Bi$. The boundary values give $A=0$, $B=1/n$, hence the [gambler's ruin](../../../../../../gambler-s-ruin.md) answer is

$$
\boxed{p_i=\frac in.}
$$

For completeness, the game terminates with [probability](../../../../../../probability.md) one. From any nonabsorbing state, a run of $n$ consecutive heads would reach $n$ within the next $n$ tosses, and that run has [probability](../../../../../../probability.md) $2^{-n}$. Conditional on survival, the same bound applies to the next block. Therefore the [probability](../../../../../../probability.md) of surviving $kn$ tosses is at most $(1-2^{-n})^k$, which tends to zero.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
