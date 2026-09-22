<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The perturbative expansion of $Z[J]$ contains arbitrary [Feynman diagrams](../../../../../../feynman-diagram.md), including disconnected products. The [linked-cluster theorem](../../../../../../linked-cluster-theorem.md) gives

$$
Z[J]=Z[0]\exp\left(\sum_{C\ \text{connected}}C[J]\right),
$$

because the factorials from repeated connected components reproduce the exponential series. Therefore $W[J]=-\hbar\log Z[J]$ is the sum of [connected Feynman diagrams](../../../../../../connected-feynman-diagram.md).

The Legendre transform removes diagrams that disconnect upon cutting one internal line. Equivalently, every connected diagram is a tree whose vertices are exact one-particle-irreducible vertices and whose edges are exact propagators. Thus

$$
\boxed{\Gamma[\Phi]=S[\Phi]+\text{the sum of loop-level one-particle-irreducible diagrams},}
$$

and its functional derivatives are the [one-particle-irreducible correlation functions](../../../../../../one-particle-irreducible-correlation-function.md). Algebraically, differentiating the Legendre relations gives

$$
\int d^dz\,
\frac{\delta^2\Gamma}{\delta\Phi(x)\delta\Phi(z)}
\frac{\delta^2W}{\delta J(z)\delta J(y)}
=-\delta^{(d)}(x-y),
$$

so an exact [quantum field theory propagator](../../../../../../propagator.md) joining two proper vertices is precisely the inverse [Hessian matrix](../../../../../../hessian-matrix.md) needed to reconstruct connected diagrams.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
