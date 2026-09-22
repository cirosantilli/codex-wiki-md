<h1 id="s7/1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Hamilton's principle](../../../../../principle-of-stationary-action.md) states that the physical path makes the [action](../../../../../action.md) $S=\int_{t_i}^{t_f}L(\mathbf q,\dot{\mathbf q},t)\,dt$ stationary under differentiable variations $\delta q_i$ vanishing at the fixed endpoints. Its conventional “least action” name does not guarantee a minimum. Expanding to first order and integrating the velocity term by parts gives

$$
\delta S=\left[\sum_i\frac{\partial L}{\partial\dot q_i}\delta q_i\right]_{t_i}^{t_f}
+\int_{t_i}^{t_f}\sum_i\left(\frac{\partial L}{\partial q_i}-\frac d{dt}\frac{\partial L}{\partial\dot q_i}\right)\delta q_i\,dt.
$$

The endpoint term vanishes. By the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md), the coefficients of the independent interior variations must vanish, yielding

$$
\boxed{\frac d{dt}\frac{\partial L}{\partial\dot q_i}-\frac{\partial L}{\partial q_i}=0.}
$$

For example, the zero path of a harmonic oscillator with endpoints zero can have both positive and negative second variations when the elapsed time exceeds a half-period; stationary action then need not be a least value. The Euler-Lagrange condition is the local statement that the variational principle actually supplies.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [1](../../1.md)
3. [S7](../../../s7.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
