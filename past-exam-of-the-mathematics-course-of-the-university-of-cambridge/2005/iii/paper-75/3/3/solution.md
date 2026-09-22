<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In [Gaussian units](../../../../../../gaussian-units.md), the ensemble-averaged [magnetic energy](../../../../../../magnetic-energy.md) density is

$$
\boxed{\mathcal E_B(t)=\frac1{8\pi}\int_0^\infty B^2F(B,t)\,dB.}
$$

Let $M_q=\int_0^\infty B^qF\,dB$, and assume the relevant moment exists and endpoint terms vanish. Twice applying [integration by parts](../../../../../../integration-by-parts.md) to the conservative magnitude equation gives

$$
\frac{dM_q}{dt}=-Dq\int_0^\infty B^{q-1}(B^2F_B-2BF)\,dB
=Dq(q+3)M_q.
$$

In particular, the [magnetic stretching moment growth](../../../../../../magnetic-stretching-moment-growth.md) for $q=2$ is

$$
\boxed{\frac{d\langle B^2\rangle}{dt}=10D\langle B^2\rangle=2\gamma\langle B^2\rangle,\qquad
\mathcal E_B(t)=\mathcal E_B(0)e^{2\gamma t}.}
$$

This is a [kinematic magnetic dynamo](../../../../../../kinematic-magnetic-dynamo.md) result with prescribed velocity statistics and no Ohmic loss. Once the [Lorentz force](../../../../../../lorentz-force.md) appreciably changes the flow, this indefinitely exponential kinematic approximation is no longer self-consistent.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
