<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Whenever $I>0$, divide the first [SIR model](../../../../../../sir-model.md) equation by the recovery equation:

$$
\frac{dS}{dR}=-\frac\beta\gamma S.
$$

The [SIR susceptible-recovered identity](../../../../../../sir-susceptible-recovered-identity.md) follows by integrating from $R=0,S=N$, giving **susceptibles as a function of recovered individuals**:

$$
\boxed{S(t)=N e^{-\beta R(t)/\gamma}.}
$$

Population conservation then gives **the infectious count**:

$$
\boxed{I(t)=N+1-R(t)-N e^{-\beta R(t)/\gamma}.}
$$

These identities extend continuously to the limiting state where the infectious count vanishes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
