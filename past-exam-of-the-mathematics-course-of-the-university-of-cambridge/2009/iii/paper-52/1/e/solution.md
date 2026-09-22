<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Replace evaluation in a possibly inaccurate dynamical model by an experimental objective. Parametrize an admissible pulse as $f(t;a)$, with $a$ collecting time-slice amplitudes or basis-function coefficients. Prepare the same initial state, apply the pulse, measure performance, and update $a$ before the next run. This is [adaptive experimental quantum control](../../../../../../adaptive-experimental-quantum-control.md): the loop closes through experimental results, even though each individual pulse is applied open loop.

For example, minimize

$$
\boxed{J_{\mathrm{exp}}(a)=1-\operatorname{Tr}[\rho_d\rho_a(T)]
+\eta\int_0^T\|f(t;a)\|^2\,dt,\qquad a\in\mathcal A,}
$$

for a pure target $\rho_d$, with a nonempty closed [convex set](../../../../../../convex-set.md) $\mathcal A$ enforcing amplitude and bandwidth bounds. The overlap is an experimentally estimable [probability](../../../../../../probability.md). An [observable](../../../../../../observable.md) objective can use its measured expectation instead; a gate objective generally needs more input states and measurement settings. The true dynamics constrain the physically produced $\rho_a(T)$, but no accurate formula for those dynamics is required to evaluate this objective.

A direct search compares measured scores for candidate pulses, accepts improvements and refines the search region. Alternatively estimate a [gradient](../../../../../../gradient.md) experimentally by finite differences,

$$
\widehat{\partial_{a_k}J}=
\frac{\widehat J(a+\varepsilon e_k)-\widehat J(a-\varepsilon e_k)}{2\varepsilon},
\qquad a_{n+1}=\Pi_{\mathcal A}(a_n-\gamma_n\widehat{\nabla J}),
$$

where $\Pi_{\mathcal A}$ is the [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md). Population-based searches can also explore several candidates in parallel. These methods use experimental data rather than simulated propagation or a model-derived adjoint [gradient](../../../../../../gradient.md).

Each score needs enough repeated preparations to manage measurement noise; uncertainty in score differences should determine replication and stopping decisions. Excessively small finite-difference steps amplify that noise. A model-based pulse can provide a useful starting point, but adaptation corrects its systematic mismatch using the device itself. This mitigates model uncertainty, not arbitrary fluctuations: reproducible preparation, calibrated measurements and sufficiently slow drift remain necessary. Nor does a local numerical search guarantee a global optimum.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
