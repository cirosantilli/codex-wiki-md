<h1 id="m/m5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Given $X_n=k>0$, the number remaining next time is uniform on $\{0,\ldots,k-1\}$ and is independent of earlier choices; given $X_n=0$, the next state is $0$. Thus the conditional law of $X_{n+1}$ depends only on $X_n$, which is the [Markov property](../../../../../../markov-property.md).

By contrast, observing only the last number removed generally loses information about the remaining stock. For $N\geq3$, compare the two positive-[probability](../../../../../../probability.md) histories

$$
(Y_1,Y_2)=(1,1),\qquad (Y_1,Y_2)=(N-1,1).
$$

Both have $Y_2=1$, but the first leaves $N-2>0$ stickers, so $P(Y_3>0\mid Y_1=1,Y_2=1)=1$, whereas the second leaves none, so $P(Y_3>0\mid Y_1=N-1,Y_2=1)=0$. Hence $(Y_n)$ fails the [Markov property](../../../../../../markov-property.md).

The qualification $N\geq3$ is necessary if a [Markov chain](../../../../../../markov-chain-split.md) is allowed to have time-dependent transitions. For $N=1$, the removal sequence is the deterministic, time-homogeneous [Markov chain](../../../../../../markov-chain-split.md) $1,0,0,\ldots$. For $N=2$, it is a time-inhomogeneous [Markov chain](../../../../../../markov-chain-split.md), although it is not time-homogeneous on its observed removal states: a removal of $1$ at the first step forces another removal of $1$, whereas a removal of $1$ at the second step forces $0$ next. The blanket non-Markov claim should therefore be understood in the generic, nondegenerate setting.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
