# Plant SI model with logistic total population

↑ **Parent:** [SI model](si-model.md)

The plant-disease model

$$
\dot S=(S+I)(1-S)-\beta IS,
\qquad
\dot I=-(S+I)I+\beta IS
$$

has total population $N=S+I$ and [disease prevalence](prevalence.md) $\theta=I/N$ satisfying

$$
\dot N=N(1-N),
\qquad
\dot\theta=\theta\{\beta N(1-\theta)-1\}.
$$

Thus infection does not alter total-population growth. The invasion threshold at the carrying capacity $N=1$ is $\beta=1$.

**Table of contents**

- [Uniform per-capita culling in the plant SI model](uniform-per-capita-culling-in-the-plant-si-model.md)

## ↑ Ancestors (6)

1. [SI model](si-model.md)
2. [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/14c/c/solution.md)
