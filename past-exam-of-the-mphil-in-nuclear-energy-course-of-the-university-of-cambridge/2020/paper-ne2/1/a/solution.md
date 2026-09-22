<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take one-dimensional [steady state](../../../../../steady-state.md) [thermal conduction](../../../../../thermal-conduction.md), constant [thermal conductivity](../../../../../thermal-conductivity.md) $k>0$, and positive [volumetric heat generation rate](../../../../../volumetric-heat-generation-rate.md). Write $q_0=q'''_0$ for brevity, and let $x$ increase away from the illuminated face. [Conservation of energy](../../../../../conservation-of-energy.md) and [Fourier's law](../../../../../fourier-s-law.md) give

$$
\frac{d}{dx}\left(-k\frac{dT}{dx}\right)=q_0e^{-\mu x},
\qquad T(0)=T(a)=T_0.
$$

Thus $T''=-(q_0/k)e^{-\mu x}<0$: the profile is strictly concave and any stationary point is its unique maximum. Two [integrations](../../../../../integral-split.md) and the equal-surface [boundary conditions](../../../../../boundary-condition.md) yield the [exponential slab heating](../../../../../slab-conduction-with-exponentially-decaying-heat-generation.md) solution

$$
\boxed{T(x)-T_0=\frac{q_0}{k\mu^2}
\left[1-e^{-\mu x}-(1-e^{-\mu a})\frac{x}{a}\right].}
$$

Its derivative is

$$
T'(x)=\frac{q_0}{k\mu}
\left[e^{-\mu x}-\frac{1-e^{-\mu a}}{\mu a}\right].
$$

Define $\beta=\mu a$ and $C=(1-e^{-\beta})/\beta$. Setting $T'(x_m)=0$ gives **the distance from the illuminated surface**:

$$
\boxed{x_m=\frac1\mu\ln\frac{\mu a}{1-e^{-\mu a}}=-\frac{\ln C}{\mu}.}
$$

For $\beta>0$, $e^{-\beta}<C<1$, so $0<x_m<a$. More specifically $C=e^{-\beta/2}\sinh(\beta/2)/(\beta/2)>e^{-\beta/2}$, hence $x_m<a/2$: the peak is nearer the more strongly heated face.

The apparent singularity at $\mu=0$ is removable. Expansion gives

$$
\frac{x_m}{a}=\frac12-\frac{\beta}{24}+O(\beta^3),
\qquad
T(x)-T_0\longrightarrow\frac{q_0}{2k}x(a-x).
$$

The uniform-heating limit therefore has its maximum at $a/2$, as symmetry requires.

## ↑ Ancestors (10)

1. [A](../a.md)
2. [1](../../1.md)
3. [Module NE2](../../../paper-ne2-split.md)
4. [2020](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
