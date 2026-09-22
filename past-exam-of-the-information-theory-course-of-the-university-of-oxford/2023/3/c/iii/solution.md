<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $0\leq q<1$, the total number of forward [channel](../../../../../communication-channel.md) uses is $T_n=\sum_{j=1}^nM_j$, so the random [code rate](../../../../../code-rate.md) of a message with $n$ [bits](../../../../../bit.md) is

$$
R_n=\frac{n}{T_n}=\left(\frac1n\sum_{j=1}^nM_j\right)^{-1}.
$$

The [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) $M_j$ have finite [expectation](../../../../../expected-value-split.md) $1/(1-q)$. By the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md),

$$
\boxed{R_n\longrightarrow1-q\quad\text{almost surely}.}
$$

Thus the protocol reaches the [binary erasure channel](../../../../../binary-erasure-channel.md) [channel capacity](../../../../../channel-capacity.md) in its asymptotic forward throughput while guaranteeing zero error on every completed message. Its random transmission length and use of [channel feedback](../../../../../channel-feedback.md) distinguish it from the fixed-length [channel codes](../../../../../channel-code.md) in part (b). Independent erasure indicators suffice for this calculation; the message [bits](../../../../../bit.md) themselves need not be [independent](../../../../../independent-random-variables.md) or uniformly distributed. At $q=1$, the algorithm never produces a completed transmission, so $R_n$ as a completed-code rate is undefined; the physical throughput is zero.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
