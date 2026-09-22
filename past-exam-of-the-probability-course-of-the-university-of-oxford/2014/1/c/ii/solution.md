<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Now $M_{n+1}=\max(M_n,X_{n+1})$. Again $X_{n+1}$ is [independent](../../../../../independent-random-variables.md) of the whole previous history, so the recursion is a [Markov chain obtained from independent innovations](../../../../../markov-chain-obtained-from-independent-innovations.md). To remain at $s$, the new observation must be at most $s$; to jump to $t>s$, it must equal $t$. Thus the [transition probabilities](../../../../../transition-probability.md) are

$$
\boxed{P_{st}=\begin{cases}0,&t<s,\\\dfrac{s}{s+1},&t=s,\\\dfrac1{t(t+1)},&t>s.\end{cases}}
$$

The upper tail sums to $1/(s+1)$, complementing the holding [probability](../../../../../probability.md) $s/(s+1)$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
