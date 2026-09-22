<h1 id="m/m5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Given $X_n=k$, the next child takes a fresh uniform choice from $1,\ldots,k$, making $X_{n+1}$ uniform on $0,\ldots,k-1$. At zero the count stays zero. This conditional law depends only on the current count, so $X_n$ is a [Markov chain](../../../../../../markov-chain-split.md).

The amounts taken do not generally retain that state information. For $N\geq3$, compare two positive-[probability](../../../../../../probability.md) histories with the same current value $Y_2=1$: if $Y_1=N-2$, exactly one sticker remains and $Y_3=1$; if $Y_1=N-1$, none remains and $Y_3=0$. Thus the next amount depends on earlier history even after conditioning on the current amount, violating the [Markov property](../../../../../../markov-property.md).

The non-Markov assertion needs this nondegenerate range of $N$. With $N=1$ the amount process is trivial; for $N=2$ it is also Markov if time-inhomogeneous transitions are permitted. The history counterexample establishes the intended failure for every $N\geq3$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
