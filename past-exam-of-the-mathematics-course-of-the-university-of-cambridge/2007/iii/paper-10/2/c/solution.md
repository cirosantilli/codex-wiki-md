<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $C=[A,B]$ be [trace](../../../../../../matrix-trace.md) class and set $F(t)=e^{tA}e^Be^{-tA}e^{-B}$. The integral identity $e^BAe^{-B}-A=\int_0^1e^{sB}[B,A]e^{-sB}ds$ is trace-norm convergent. It shows that this difference is [trace](../../../../../../matrix-trace.md) class. The analogous Duhamel identity then makes $F(t)-I$ [trace](../../../../../../matrix-trace.md) class and differentiable in that [norm](../../../../../../norm.md). Hence $F(t)\in G(H)$.

Compute the right logarithmic [derivative](../../../../../../derivative.md) without taking separate traces of $A$:

$$
\dot F F^{-1}=e^{tA}(A-e^BAe^{-B})e^{-tA}.
$$

[Trace](../../../../../../matrix-trace.md) invariance under bounded invertible similarity and the integral identity give $\operatorname{Tr}(\dot F F^{-1})=-\int_0^1\operatorname{Tr}[B,A]ds=\operatorname{Tr}[A,B]$. Cyclicity with a [trace-class](../../../../../../trace-class-operator.md) factor makes this equal to the [trace](../../../../../../matrix-trace.md) in part (b). As $F(0)=I$, integrating the scalar differential equation gives

$$
\boxed{\det(e^Ae^Be^{-A}e^{-B})=\exp\operatorname{Tr}[A,B].}
$$

This [Fredholm determinant of an exponential commutator](../../../../../../fredholm-determinant-of-an-exponential-commutator.md) can be nontrivial in infinite [dimension](../../../../../../dimension-vector-space.md): it is not legitimate to set the [trace](../../../../../../matrix-trace.md) of a [trace-class](../../../../../../trace-class-operator.md) [commutator](../../../../../../commutator.md) to zero when $A,B$ themselves need not be [trace](../../../../../../matrix-trace.md) class.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
