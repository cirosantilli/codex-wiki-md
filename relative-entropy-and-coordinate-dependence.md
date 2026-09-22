# Relative entropy and coordinate dependence

↑ **Parent:** [Differential entropy](differential-entropy.md)

Apply the same invertible differentiable transformation to two [probability distributions](probability-distribution.md) with densities $f$ and $r$. Both transformed densities acquire the same [Jacobian determinant](jacobian-determinant.md) factor. Write their transformed densities as $f_g$ and $r_g$. Their ratio is unchanged, and the integration measure transforms with the numerator density. Consequently their [relative entropy](kullback-leibler-divergence.md) is unchanged:

$$
D(f_g\Vert r_g)=D(f\Vert r).
$$

The densities describe two alternative laws in the same coordinate, with a nonzero [Jacobian determinant](jacobian-determinant.md) on their common domain, and the expression is assumed well defined. This explains why comparing two laws can survive a change of measurement units even though either law's [differential entropy](differential-entropy.md) changes. [Mutual information](mutual-information.md), formulated as [relative entropy](kullback-leibler-divergence.md) from a product of marginals, has the same invariance under invertible changes to either observed coordinate.

[Differential entropy](differential-entropy.md) is also the entropy term in the [evidence lower bound](evidence-lower-bound.md) for continuous [variational inference](variational-inference.md). Its coordinate dependence must be combined consistently with that of the model density; changing units does not justify changing only one term of the objective.

## ↑ Ancestors (7)

1. [Differential entropy](differential-entropy.md)
2. [Information entropy](information-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
