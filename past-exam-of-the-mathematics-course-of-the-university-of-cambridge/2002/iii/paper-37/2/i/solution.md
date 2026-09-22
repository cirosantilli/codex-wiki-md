<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret $h_A,h_B$ as [cause-specific hazards](../../../../../../cause-specific-hazard.md): their conditioning population consists of individuals still free of both events. Write

$$
H_A(t)=\int_0^t h_A(u)\,du,\qquad H_B(t)=\int_0^t h_B(u)\,du.
$$

In a short interval, either event removes an individual from that population. Hence the [survivor function](../../../../../../survival-function.md) satisfies $S'(t)=-S(t)[h_A(t)+h_B(t)]$, with $S(0)=1$. Integrating gives

$$
\boxed{\Pr(T>t)=S(t)=\exp\{-H_A(t)-H_B(t)\}.}
$$

No independence assumption on hypothetical latent event times is needed: this follows directly from the specified [cause-specific hazards](../../../../../../cause-specific-hazard.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
