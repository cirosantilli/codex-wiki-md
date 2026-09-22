<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Because $s>1$, the [function](../../../../../../function-split.md) $t\mapsto s^t$ is increasing and nonnegative. Thus $\{X\geq x\}=\{s^X\geq s^x\}$. Applying [Markov's inequality](../../../../../../markov-s-inequality.md) to the nonnegative [random variable](../../../../../../random-variable-split.md) $s^X$, whose [expected value](../../../../../../expected-value-split.md) is finite by assumption, yields

$$
\boxed{\mathbb P(X\geq x)\leq\frac{\mathbb E[s^X]}{s^x}=s^{-x}G_X(s).}
$$

Under the usual [probability generating function](../../../../../../probability-generating-function.md) convention $X$ takes nonnegative [integer](../../../../../../integer-split.md) values. The argument itself works for any real [random variable](../../../../../../random-variable-split.md) if $G_X(s)$ is understood as the finite [expected value](../../../../../../expected-value-split.md) $\mathbb E[s^X]$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
