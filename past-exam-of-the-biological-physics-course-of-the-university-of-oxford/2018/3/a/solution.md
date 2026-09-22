<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Represent one permissive [voltage-gated potassium channel](../../../../voltage-gated-potassium-channel.md) gate by an available closed state and an activated state, with voltage-dependent [transition rates](../../../../transition-intensity.md) $\alpha_n(V)$ and $\beta_n(V)$. Gain minus loss gives

$$
\frac{dn}{dt}=\alpha_n(1-n)-\beta_nn
=(\alpha_n+\beta_n)(n_\infty-n),
\quad n_\infty=\frac{\alpha_n}{\alpha_n+\beta_n},\quad
\tau_n=\frac1{\alpha_n+\beta_n}.
$$

During a [voltage clamp](../../../../voltage-clamp.md) step the imposed voltage and hence these rates are constant. Integration with $n(0)=n_0$ gives

$$
\boxed{n(t)=n_\infty-(n_\infty-n_0)e^{-t/\tau_n}.}
$$

The fourth power in the [electrical conductance](../../../../electrical-conductance.md) describes four permissive activation variables in the [Hodgkin-Huxley model](../../../../hodgkin-huxley-model.md) phenomenology. If all must be permissive and are statistically independent, their joint [probability](../../../../probability.md) is $n^4$. Even a simple exponential rise in $n$ then gives a delayed-looking macroscopic [potassium](../../../../potassium.md) [electric current](../../../../electric-current.md). The second panel of the model figure in [solution](../../2/c/solution.md) illustrates this. A continuously changing voltage makes the rates time dependent and requires solving the differential equation along that voltage trajectory; one fixed exponential is not the general action-potential solution.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
