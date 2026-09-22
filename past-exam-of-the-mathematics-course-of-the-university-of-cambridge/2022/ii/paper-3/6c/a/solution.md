<h1 id="6c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Probability enters state $n$ through a birth from $n-1$ or a pair-death event from $n+2$, and leaves through either event at state $n$. Thus the [Kramers-Moyal master equation](../../../../../../kramers-moyal-master-equation.md) is

$$
\boxed{
\frac{\partial P(n,t)}{\partial t}
=\lambda P(n-1,t)+\beta(n+2)^2P(n+2,t)
-(\lambda+\beta n^2)P(n,t)
},
$$

with probabilities and impossible transition rates taken as zero outside the nonnegative states.

A birth changes $n$ by $+1$, while a death event changes it by $-2$. Applying these increments to the first moment gives

$$
\boxed{
\frac d{dt}\langle n\rangle
=\lambda-2\beta\langle n^2\rangle
}.
$$

Consequently every steady state must satisfy

$$
\boxed{\langle n^2\rangle=\frac{\lambda}{2\beta}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6C](../../6c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
