<h1 id="2/2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write

$$
A=\|\nabla u\|_2^2,\qquad B=\|u\|_2^2,\qquad C=\|u\|_p^p.
$$

Differentiating $\log J(u+th)$ at $t=0$ for a real [test function](../../../../../../../space-of-test-functions.md) $h$ gives

$$
\frac2A\int\nabla u\mathbin{\cdot}\nabla h
+\frac4{dB}\int uh-\frac pC\int u^{p-1}h=0.
$$

After [integration by parts](../../../../../../../integration-by-parts.md),

$$
\Delta u-\lambda u+\mu u^{1+4/d}=0,
\qquad
\lambda=\frac{2A}{dB}>0,\qquad
\mu=\frac{pA}{2C}>0.
$$

Rescaling the dependent and independent variables reduces this [Euler-Lagrange equation](../../../../../../../euler-lagrange-equation.md) to the ground-state equation for $Q$. The uniqueness of its positive radial solution and the equality cases in rearrangement show that all minimizers are

$$
u(x)=aQ(b(x-x_0)),
\qquad
a\in\mathbb C\setminus\{0\},\quad b>0,\quad x_0\in\mathbb R^d.
$$

This is the [classification of Weinstein-functional minimizers](../../../../../../../classification-of-weinstein-functional-minimizers.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
