<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The term $v\mathbf n$ is directed self-propulsion at fixed speed, while the two components of $\mathbf u$ generate translational [Brownian motion](../../../../brownian-motion-split.md) with [diffusion coefficient](../../../../diffusion-coefficient.md) $D$. The angle has systematic angular velocity $\omega$ and rotational [diffusion coefficient](../../../../diffusion-coefficient.md) $D_r$. With independent standard [Brownian motions](../../../../brownian-motion-split.md), the precise [stochastic differential equations](../../../../stochastic-differential-equation.md) are

$$
d\mathbf r=v\mathbf n(\theta)dt+\sqrt{2D}\,d\mathbf W,
\qquad d\theta=\omega dt+\sqrt{2D_r}\,dW_r.
$$

Independent translational and rotational noises are the usual interpretation; the supplied autocorrelations alone would not specify arbitrary cross-correlated noises.

The complete state $(\mathbf r,\theta\bmod2\pi)$ is a [Markov process](../../../../markov-process-split.md): its future increments depend only on its present state and independent future noise. Its generator is $v\mathbf n\cdot\nabla+\omega\partial_\theta+D\nabla^2+D_r\partial_\theta^2$. Position alone generally lacks the [Markov property](../../../../markov-property.md), since an unobserved current orientation carries memory into future displacements. At long scales orientation averaging produces the effective positional [diffusion equation](../../../../diffusion-equation-split.md) in [solution](../d/solution.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
