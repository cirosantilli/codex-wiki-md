<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Itô's formula](../../../../ito-s-lemma.md) to $f(u,s)=e^{-\alpha u}s$. Its second stock derivative is zero, and the two drift terms cancel, giving

$$
d(e^{-\alpha u}S_u)=\sigma e^{-\alpha u}\,dW_u.
$$

Integrating and multiplying by $e^{\alpha T}$ solves the [linear stochastic differential equation](../../../../linear-stochastic-differential-equation.md):

$$
\boxed{S_T=e^{\alpha(T-t)}S_t+\sigma\int_t^T e^{\alpha(T-u)}\,dW_u.}
$$

The [Itô integral](../../../../ito-integral.md) has a deterministic integrand, so it is a centered [Gaussian random variable](../../../../gaussian-random-variable.md) independent of the current [filtration](../../../../filtration-probability-theory.md) $\mathcal F_t$. Its [variance](../../../../variance-split.md) follows from the [Itô isometry](../../../../ito-isometry.md). With $\tau=T-t$,

$$
\boxed{\mathbb E[S_T\mid\mathcal F_t]=e^{\alpha\tau}S_t,\qquad
\operatorname{var}(S_T\mid\mathcal F_t)=\begin{cases}
\dfrac{\sigma^2}{2\alpha}(e^{2\alpha\tau}-1),&\alpha\ne0,\\
\sigma^2\tau,&\alpha=0.
\end{cases}}
$$

The second line is also the [limit](../../../../limit-of-a-function.md) as $\alpha\to0$. The normal law asserted here is conditional on $\mathcal F_t$; an arbitrary random initial value need not give an unconditional [normal distribution](../../../../normal-distribution.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
