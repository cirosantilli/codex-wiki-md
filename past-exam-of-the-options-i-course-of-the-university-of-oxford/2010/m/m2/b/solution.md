<h1 id="m/m2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Markov property](../../../../../markov-property.md) and conditioning on the intermediate state give, for the full history through time $2n$,

$$
P(X_{2n+2}=j\mid X_0,\ldots,X_{2n})=(P^2)_{X_{2n},j}.
$$

Condition this identity again on the smaller history $(Y_0,\ldots,Y_n)$. Its right-hand side is already determined by $Y_n=X_{2n}$, so the tower property gives

$$
\boxed{P(Y_{n+1}=j\mid Y_0,\ldots,Y_n)=(P^2)_{Y_n,j}.}
$$

Thus the sampled sequence is a time-homogeneous [Markov chain](../../../../../markov-chain-split.md) with [transition matrix](../../../../../stochastic-matrix.md) $P^2$. Checking only its one-time marginal distributions would not by itself establish the [Markov property](../../../../../markov-property.md).

It is the every-second-step case of a [subsampled Markov chain](../../../../../subsampled-markov-chain.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [M2](../../m2.md)
3. [M](../../../m.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
