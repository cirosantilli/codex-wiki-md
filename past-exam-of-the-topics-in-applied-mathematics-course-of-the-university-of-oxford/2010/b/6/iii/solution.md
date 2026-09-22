<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A useful operational definition of [chaos](../../../../../chaos.md) for a deterministic flow is bounded, nonperiodic long-time dynamics on an [invariant set](../../../../../invariant-set-of-a-measure-preserving-transformation.md) with [sensitive dependence on initial conditions](../../../../../butterfly-effect.md): arbitrarily close starting states can separate by a fixed macroscopic amount. Boundedness distinguishes recurrent irregular dynamics from simple exponential escape; aperiodicity excludes a [limit cycle](../../../../../limit-cycle.md); sensitivity distinguishes chaotic unpredictability from a regular quasiperiodic signal. These are properties of the asymptotic dynamics, not a short irregular transient. One precise topological convention, [Devaney chaos](../../../../../devaney-chaos.md) on a [compact](../../../../../compact-space.md) [invariant set](../../../../../invariant-set-of-a-measure-preserving-transformation.md), instead specifies [topological transitivity](../../../../../topological-transitivity.md), dense [periodic orbits](../../../../../periodic-orbit.md), and sensitive dependence. Transitivity expresses indecomposability of the recurrent motion, while dense [periodic orbits](../../../../../periodic-orbit.md) mean every region contains unstable recurrent structure. The convention should be stated because these formulations are not identical in complete generality.

An [attractor](../../../../../attractor.md) is an [invariant set](../../../../../invariant-set-of-a-measure-preserving-transformation.md) approached by trajectories from a neighbourhood or positive-measure basin, according to the adopted [attractor](../../../../../attractor.md) convention. Calling it strange refers to irregular, typically [fractal geometry](../../../../../fractal-geometry.md) rather than a smooth point, cycle or [torus](../../../../../torus.md). **Strangeness alone does not force [chaos](../../../../../chaos.md).** [Strange nonchaotic attractors](../../../../../strange-nonchaotic-attractor.md) provide counterexamples: geometrically irregular attracting sets can lack positive exponential separation. Primary examples appear in [Strange attractors that are not chaotic, Physica D 13 (1984), pages 261–268](https://doi.org/10.1016/0167-2789(84)90282-3). This geometric convention does not assert that every such example occurs in the autonomous three-variable Lorenz family.

Two complementary numerical diagnostics are to estimate the largest [Lyapunov exponent](../../../../../lyapunov-exponent.md) and to construct a return map. For the first, integrate the [variational equation](../../../../../variational-equation.md) $\dot\eta=DF(x(t))\eta$ alongside the Lorenz trajectory, repeatedly normalize $\eta$, and average the logarithms of the accumulated stretch factors after discarding a transient. A positive converged exponent suggests sensitive exponential separation; the full spectrum should include a zero flow exponent and have sum $-(\sigma+1+b)$, providing checks. For the second, record transverse crossings of a Poincaré section or successive maxima of a state variable, then look for the stretching and folding of an aperiodic return set rather than one point or a finite cycle. Nearby-orbit separation or a broadband [power spectrum](../../../../../power-spectrum.md) can add evidence, but plots alone do not prove [chaos](../../../../../chaos.md). Repeat with smaller integration step, longer runs and several [initial conditions](../../../../../initial-condition.md) to distinguish numerical error, long transients and coexistence of [attractors](../../../../../attractor.md) from persistent dynamics.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
