<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $d=\gcd(a,b)>1$ and put $a'=a/d$, $b'=b/d$. Then $a',b'$ are [coprime integers](../../../../coprime-integers.md), and $p=b'/(a'+b')$. The six requested revisions are as follows.

**(b)(i): [communicating classes](../../../../communicating-class.md).** Every increment is divisible by $d$, so the [residue class](../../../../residue-class.md) modulo $d$ is preserved. Conversely, if $j-i$ is divisible by $d$, [Bézout's identity](../../../../bezout-s-identity.md) applied to $a',b'$ gives a path just as in (b)(i). Thus the original [Markov chain](../../../../markov-chain-split.md) is reducible on $\mathbb Z$, with exactly the $d$ closed [communicating classes](../../../../communicating-class.md)

$$
\boxed{r+d\mathbb Z,\qquad r=0,1,\ldots,d-1.}
$$

The specified walk starting at zero stays in $d\mathbb Z$.

**(b)(ii): [period of a state in a Markov chain](../../../../period-of-a-state-in-a-markov-chain.md).** The return equation $au=bv$ reduces to $a'u=b'v$. Hence $u=b'k$, $v=a'k$. For every state, the [period of a state in a Markov chain](../../../../period-of-a-state-in-a-markov-chain.md) is therefore

$$
\boxed{a'+b'=\frac{a+b}{d}.}
$$

This is still at least two, so no state is [aperiodic](../../../../aperiodic-markov-chain.md).

**(b)(iii): [stationary distribution](../../../../stationary-distribution.md).** The conclusion is unchanged: there is no [stationary distribution](../../../../stationary-distribution.md) on $\mathbb Z$. The maximum-mass proof in (b)(iii) applies verbatim, without using [coprimality](../../../../coprime-integers.md). Equivalently, each closed [communicating class](../../../../communicating-class.md), after translating and dividing its state labels by $d$, is the same centered [random walk](../../../../random-walk-split.md) with step sizes $a',-b'$ and has no [stationary distribution](../../../../stationary-distribution.md).

**(b)(iv): occupation of zero.** On $d\mathbb Z$, the rescaled walk $S_n/d$ has exactly the [transition probabilities](../../../../transition-probability.md) of the coprime walk with parameters $a',b'$. The return-probability argument in (b)(iv) therefore makes this class [null recurrent](../../../../null-recurrent-state.md). The [renewal process](../../../../renewal-process.md) proof of the occupation limit applies unchanged:

$$
\boxed{\frac1n\sum_{r=0}^{n-1}\mathbf1_{\{S_r=0\}}\longrightarrow0\quad\text{almost surely}.}
$$

Starting in another [residue class](../../../../residue-class.md) would make every visit to zero impossible, also giving occupation proportion zero.

**(c)(i): modified [communicating classes](../../../../communicating-class.md).** These are unchanged: $C=\{-c-b,\ldots,c+a\}$ is one finite [closed communicating class](../../../../closed-communicating-class.md), and all other states are transient singleton classes. The original proof used consecutive reset destinations and never used [coprimality](../../../../coprime-integers.md). Resetting to the $b$ consecutive integers $c-b+1,\ldots,c$ connects different [residue classes](../../../../residue-class.md), so it would be incorrect to split $C$ according to [residue classes](../../../../residue-class.md) modulo $d$.

**(c)(ii): [limiting distribution](../../../../limiting-distribution.md).** The column-sum calculation, the [irreducible Markov chain](../../../../irreducible-markov-chain.md) property on a finite class, positive self-transition [probabilities](../../../../probability.md), and geometric entrance argument also required no [coprimality](../../../../coprime-integers.md). Thus for every initial state the same [convergence in distribution](../../../../convergence-in-distribution.md) holds:

$$
\boxed{R_n\xrightarrow{\mathrm d}\operatorname{Unif}\{-c-b,\ldots,c+a\}.}
$$

In particular, the denominator $2c+a+b+1$ is unchanged; it is not divided by $d$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the probability course of the University of Oxford](../../../split.md)
5. [Probability course of the University of Oxford](../../../../probability-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
