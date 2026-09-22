<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The linear predictor is unchanged by $\alpha_j\mapsto\alpha_j+c$, $\beta_t\mapsto\beta_t+d$, $\mu\mapsto\mu-c-d$. Without constraints, different parameter triples therefore give the same rates and [likelihood](../../../../../../likelihood-function.md). [Identifiability](../../../../../../identifiability.md) requires choosing one representative of this redundancy.

Taking the first levels as reference yields $\alpha_1=\beta_1=0$. Then

$$
\mu=\log\lambda_{11},\qquad
\alpha_2=\log\lambda_{21}-\log\lambda_{11},\qquad
\beta_2=\log\lambda_{12}-\log\lambda_{11}.
$$

These identify all three free parameters, while $\lambda_{22}=\lambda_{21}\lambda_{12}/\lambda_{11}$ is the model's no-interaction constraint. **The zero reference effects fix a parametrization; they do not remove the baseline rate or impose equal rates across groups.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
