<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $M_t=B_t^3-3tB_t$. It is an [adapted process](../../../../../adapted-process.md) and is integrable at every finite time, because [normal random variables](../../../../../gaussian-random-variable.md) have finite absolute [moments](../../../../../moment.md) of every order. Fix $0\leq s<t$ and let $D=B_t-B_s$. Then $D$ is [independent](../../../../../independent-random-variables.md) of $\mathcal F_s$, has [mean](../../../../../expected-value-split.md) zero, [variance](../../../../../variance-split.md) $t-s$, and third [moment](../../../../../moment.md) zero. Expanding the cube inside the [conditional expectation](../../../../../conditional-expectation.md) gives

$$
\mathbb E[B_t^3\mid\mathcal F_s]
=B_s^3+3B_s\mathbb ED^2
=B_s^3+3(t-s)B_s.
$$

Also $\mathbb E[B_t\mid\mathcal F_s]=B_s$. Therefore

$$
\boxed{\mathbb E[M_t\mid\mathcal F_s]
=B_s^3+3(t-s)B_s-3tB_s
=B_s^3-3sB_s=M_s.}
$$

These are exactly the defining conditions for a [martingale](../../../../../martingale-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
