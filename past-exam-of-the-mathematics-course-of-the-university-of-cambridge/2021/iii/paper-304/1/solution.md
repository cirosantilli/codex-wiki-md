<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

With Euclidean source convention $+\int d^dx\,J_a\phi_a$, the [generating functional](../../../../../generating-functional.md) is

$$
Z[J]=\int\mathcal D\phi\,
\exp\left[-S[\phi]+\int d^dx\,J_a(x)\phi_a(x)\right].
$$

Here $J_a(x)$ is a nondynamical source. Its [functional derivatives](../../../../../functional-derivative.md) insert fields:

$$
\frac{1}{Z[0]}\frac{\delta^nZ[J]}
{\delta J_{a_1}(x_1)\cdots\delta J_{a_n}(x_n)}\bigg|_{J=0}
=\langle\phi_{a_1}(x_1)\cdots\phi_{a_n}(x_n)\rangle.
$$

This is why $Z$ “generates” correlation functions.

With the notation of the question, $W[J]=-\log Z[J]$ is the Euclidean [connected generating functional](../../../../../connected-generating-functional.md); it is distinct from a [Wilsonian effective action](../../../../../wilsonian-effective-action.md). Define the classical field

$$
\Phi_a(x)=\langle\phi_a(x)\rangle_J=-\frac{\delta W}{\delta J_a(x)}.
$$

The [quantum effective action](../../../../../effective-action.md) is the [Legendre transform](../../../../../convex-conjugate.md)

$$
\boxed{\Gamma[\Phi]=W[J]+\int d^dx\,J_a(x)\Phi_a(x)},
$$

where $J$ is eliminated in favor of $\Phi$. Its first derivative is

$$
\frac{\delta\Gamma}{\delta\Phi_a(x)}=J_a(x),
$$

so at zero source the quantum expectation value is a [stationary point](../../../../../stationary-point.md) of $\Gamma$. Moreover,

$$
\int d^dz\,
\Gamma^{(2)}_{ac}(x,z)G_{cb}(z,y)=\delta_{ab}\delta^{(d)}(x-y),
$$

where $G_{ab}=\langle\phi_a\phi_b\rangle_{J,\rm conn}$ is the exact [connected correlation function](../../../../../connected-correlation-function.md). Thus the second derivative of $\Gamma$ is the inverse exact propagator.

Perturbatively, $Z[J]$ sums all [Feynman diagrams](../../../../../feynman-diagram.md), including disconnected ones. The exponential formula for combinatorial structures says that its logarithm selects [connected Feynman diagrams](../../../../../connected-feynman-diagram.md), so $W$ sums connected diagrams with the sign dictated by the convention above. The Legendre transform removes diagrams that disconnect when one internal line is cut; consequently $\Gamma$ sums [one-particle-irreducible Feynman diagrams](../../../../../one-particle-irreducible-feynman-diagram.md). Equivalently, every connected diagram is a tree assembled from one-particle-irreducible vertices and full propagators, and the Legendre transform inverts that tree construction.

Now let $J'_a=J_bU_{ba}$. Then

$$
Z[J']=\int\mathcal D\phi\,e^{-S[\phi]+\int J_bU_{ba}\phi_a}.
$$

Changing variables to $\phi'_b=U_{ba}\phi_a$ and using invariance of both the action and [functional measure](../../../../../functional-measure.md) gives $Z[J']=Z[J]$, hence $W[J']=W[J]$. In the Legendre transform, the pairing obeys

$$
J_a(U_{ab}\Phi_b)=(J_bU_{ba})\Phi_a.
$$

Changing the source variable and using the invariance of $W$ therefore gives

$$
\boxed{\Gamma[U\Phi]=\Gamma[\Phi]}.
$$

The symmetry of the classical action and measure is inherited by the full [quantum effective action](../../../../../effective-action.md) when it has no [quantum anomaly](../../../../../anomaly-physics.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 304](../../paper-304-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
