<h1 id="question-6/c/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

The [trigonometric identity](../../../../../../../trigonometric-identity.md)

$$
\sin^3\theta=\frac34\sin\theta-\frac14\sin(3\theta)
$$

shows that only angular [Fourier modes](../../../../../../../fourier-mode.md) $1$ and $3$ are required. Differentiating the [harmonic expansion on a disk](../../../../../../../harmonic-expansion-on-a-disk.md) at $r=1$ multiplies the coefficient of each nonconstant [Fourier mode](../../../../../../../fourier-mode.md) by $n$. Thus $B_1=3/4$ and $3B_3=-1/4$, giving

$$
\boxed{T(r,\theta)=C+\frac34r\sin\theta-\frac1{12}r^3\sin(3\theta),\qquad C\in\mathbb R}.
$$

Each term is a regular [harmonic function](../../../../../../../harmonic-function.md), and the radial [derivative](../../../../../../../derivative.md) is

$$
T_r(1,\theta)=\frac34\sin\theta-\frac14\sin(3\theta)=\sin^3\theta.
$$

The [Neumann compatibility condition for Laplace's equation](../../../../../../../neumann-compatibility-condition-for-laplace-s-equation.md) holds because

$$
\int_0^{2\pi}\sin^3\theta\,d\theta=0,
$$

as is necessary by the [divergence theorem](../../../../../../../divergence-theorem.md) applied to the [gradient](../../../../../../../gradient.md) of a [harmonic function](../../../../../../../harmonic-function.md).

**The additive constant is undetermined.** This [Neumann boundary condition](../../../../../../../neumann-boundary-condition.md) is unchanged by $T\mapsto T+C$, so the paper's blanket uniqueness assertion requires a normalization in this case. The [uniqueness of the Neumann problem](../../../../../../../uniqueness-of-the-neumann-problem.md) gives uniqueness up to a constant; prescribing $T(0)=0$, or zero mean temperature, selects the displayed answer with $C=0$.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [c](../../c.md)
3. [Question 6](../../../question-6.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
