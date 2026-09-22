<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The first departure from the no-symptoms state has an [exponential distribution](../../../../../../../exponential-distribution.md) with rate $\lambda$. Spending the entire interval there means no departure at all, so

$$
\boxed{\mathbb P(\text{no symptoms throughout }[0,t]\mid X(0)=1)=e^{-\lambda t}.}
$$

This is the [holding time](../../../../../../../holding-time.md) survival [probability](../../../../../../../probability.md). The [transition probability](../../../../../../../transition-probability.md) $p_{11}(t)$ only says that the patient is symptom-free at the endpoint, allowing an onset and recovery in between, and is therefore not the answer. The formula also covers $\lambda=0$, when state 1 is absorbing.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
