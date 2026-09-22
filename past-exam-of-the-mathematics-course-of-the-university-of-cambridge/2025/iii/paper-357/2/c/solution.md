<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Lie derivative](../../../../../../lie-derivative-of-a-differential-form.md) of the spatial covector $j_\alpha$ along $n^\mu$ is

$$
\mathcal L_nj_\alpha
=n^\mu\nabla_\mu j_\alpha+j_\mu\nabla_\alpha n^\mu.
$$

To show that it is spatial, contract with $n^\alpha$. Differentiating $n^\alpha j_\alpha=0$ along $n^\mu$ gives

$$
n^\alpha n^\mu\nabla_\mu j_\alpha=-a^\alpha j_\alpha,
$$

whereas

$$
n^\alpha j_\mu\nabla_\alpha n^\mu=j_\mu a^\mu.
$$

The terms cancel, so

$$
n^\alpha\mathcal L_nj_\alpha=0.
$$

A spatial projector therefore acts trivially:

$$
\boxed{\perp^\alpha{}_\beta\mathcal L_nj_\alpha
=\mathcal L_nj_\beta}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 357](../../../paper-357-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
