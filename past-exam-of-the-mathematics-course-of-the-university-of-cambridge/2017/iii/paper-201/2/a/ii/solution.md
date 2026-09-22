<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the converse in the [characterization of a martingale by stopped expectations](../../../../../../../characterization-of-a-martingale-by-stopped-expectations.md), fix $n\geq0$ and $A\in\mathcal F_n$. Define the [bounded stopping time](../../../../../../../bounded-stopping-time.md)

$$
T_A=\begin{cases}n+1,&\omega\in A,\\ n,&\omega\notin A.\end{cases}
$$

Indeed, its only nontrivial sublevel [event](../../../../../../../event.md) is $\{T_A\leq n\}=A^c\in\mathcal F_n$. Applying the assumed stopped-expectation equality to $T_A$ and to the deterministic stopping time $n$ gives

$$
0=\mathbb E(M_{T_A}-M_n)=\mathbb E\bigl[\mathbf1_A(M_{n+1}-M_n)\bigr].
$$

This holds for every $A\in\mathcal F_n$. Since $M_n$ is [adapted](../../../../../../../adapted-process.md) and both variables are integrable, the defining test-event property of [conditional expectation](../../../../../../../conditional-expectation.md) yields

$$
\boxed{\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n.}
$$

Together with the given adaptation and integrability, this is exactly the [martingale](../../../../../../../martingale-split.md) property.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 201](../../../../paper-201-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
