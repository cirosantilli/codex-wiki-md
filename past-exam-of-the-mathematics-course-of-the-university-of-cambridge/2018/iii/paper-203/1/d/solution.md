<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Loewner local growth property](../../../../../../loewner-local-growth-property.md) gives a continuous [Loewner driving function](../../../../../../loewner-driving-function.md), and we normalize $U_0=0$. Mapping out an initial hull transforms the future driver to $U_{t+s}-U_t$. The [Conformal Markov property of SLE](../../../../../../conformal-markov-property-of-sle.md) therefore gives [stationary increments](../../../../../../stationary-increments.md) and [independent increments](../../../../../../independent-increments.md).

Consequently $U$ is a continuous [Lévy process](../../../../../../levy-process.md). In the [Lévy–Khintchine formula](../../../../../../levy-khintchine-formula.md), continuity excludes its jump measure, so its only possible components are a deterministic linear drift and [Brownian motion](../../../../../../brownian-motion-split.md):

$$
U_t=\mu t+\sigma B_t,\qquad\sigma\geq0.
$$

Conformal invariance under dilations gives $U_{r^2t}/r\overset{d}=U_t$. Comparing the [expectations](../../../../../../expected-value.md) of these [Gaussian random variables](../../../../../../gaussian-random-variable.md) yields $\mu rt=\mu t$ for every $r>0$, hence $\mu=0$. The Brownian term already has the required law by [Brownian scaling](../../../../../../brownian-scaling.md). Therefore the [characterization of the SLE driving function](../../../../../../characterization-of-the-sle-driving-function.md) is

$$
\boxed{U_t=\sqrt\kappa B_t\quad\text{in law},\qquad\kappa=\sigma^2\geq0.}
$$

The case $\kappa=0$ is the constant zero driver. No reflection-symmetry assumption is needed to remove the drift; scaling suffices.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
