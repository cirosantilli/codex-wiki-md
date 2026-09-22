<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Under the [Fourier transform](../../../../../../fourier-transform.md), the operator $A(t)=\partial_x^3+\phi(t)\partial_x$ is the [Fourier multiplier operator](../../../../../../fourier-multiplier-operator.md)

$$
\widehat{A(t)u}(\xi)
=i\bigl(\phi(t)\xi-\xi^3\bigr)\widehat u(\xi).
$$

Its symbol is purely imaginary because $\phi$ is real. Consequently $A(t)$ is [skew-adjoint](../../../../../../skew-adjoint-generator.md) on $L^2(\mathbb R)$ with common domain $H^3(\mathbb R)$ and generates the [strongly continuous unitary group](../../../../../../strongly-continuous-unitary-group.md)

$$
\widehat{e^{rA(t)}u}(\xi)
=e^{ir(\phi(t)\xi-\xi^3)}\widehat u(\xi).
$$

The [Plancherel theorem](../../../../../../plancherel-theorem.md) gives $\|e^{rA(t)}u\|_2=\|u\|_2$, so every $A(t)\in\mathcal G(1,0)$. Products of the frozen groups are also unitary; hence this is a [stable family of semigroup generators](../../../../../../stable-family-of-semigroup-generators.md) with constants $1,0$.

For $u\in H^3(\mathbb R)$,

$$
\|(A(t)-A(s))u\|_2
=|\phi(t)-\phi(s)|\,\|\partial_xu\|_2
\leq|\phi(t)-\phi(s)|\,\|u\|_{H^3}.
$$

Since $\phi\in C^1(\mathbb R)$, the map $t\mapsto A(t)$ is continuously differentiable from $H^3$ to $L^2$. All hypotheses from part f are satisfied, so an [evolution family](../../../../../../evolution-family.md) exists on every finite interval $[0,T]$.

In this commuting [Fourier multiplier operator](../../../../../../fourier-multiplier-operator.md) example the solution operator can also be written explicitly:

$$
\boxed{
\widehat{U(t,s)u}(\xi)
=\exp\left(i\left[-(t-s)\xi^3
+\xi\int_s^t\phi(r)\,dr\right]\right)\widehat u(\xi)}.
$$

Its multiplier has absolute value one, directly confirming [strong continuity](../../../../../../strong-continuity.md), the [evolution family](../../../../../../evolution-family.md) law, preservation of $H^3$, and the required derivatives. The equation combines the dispersive [Airy equation](../../../../../../airy-equation.md) with a time-dependent [linear transport equation](../../../../../../linear-transport-equation.md).

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
