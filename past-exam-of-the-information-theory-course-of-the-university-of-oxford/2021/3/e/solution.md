<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

There are two possible messages and three channel uses, giving

$$
\boxed{R=\frac{\log_2 2}{3}=\frac13\ \text{bit per use}.}
$$

Conditional on either transmitted message, a decoding error occurs exactly when at least two of the three [bits](../../../../bit.md) are flipped. The [discrete memoryless channel](../../../../discrete-memoryless-channel.md) makes these flips [independent](../../../../independent-random-variables.md), each with [probability](../../../../probability.md) $\varepsilon=1/10$. Their count therefore has a [binomial distribution](../../../../binomial-distribution.md) with parameters $3,\varepsilon$. [Majority-vote decoding of a repetition code](../../../../majority-vote-decoding-of-a-repetition-code.md) gives

$$
\begin{aligned}
\mathbb P(\text{error}\mid W=a)
&=\binom32\varepsilon^2(1-\varepsilon)+\varepsilon^3\\
&=3\left(\frac1{10}\right)^2\frac9{10}+\left(\frac1{10}\right)^3
=\frac7{250}=0.028.
\end{aligned}
$$

Interchanging the two [bit](../../../../bit.md) values leaves the [binary symmetric channel](../../../../binary-symmetric-channel.md) and majority decision unchanged, so **$\mathbb P(\text{error}\mid W=b)=7/250$ as well**. Both the maximum conditional error and the average error, for any message prior, are therefore $0.028$. The [probability](../../../../probability.md) of correct decoding for each message is $243/250=0.972$. These are finite-block error [probabilities](../../../../probability.md); a channel-capacity statement alone would not determine them.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
