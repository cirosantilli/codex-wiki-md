# Kalman rank criterion

↑ **Parent:** [Controllability](controllability.md)

For a finite-dimensional continuous-time [linear time-invariant system](linear-time-invariant-system.md) $\dot x=Ax+Bu$ on $\mathbb R^n$, with constant [matrices](matrix.md) $A,B$ over the [real numbers](real-number.md), no state constraints, and every [piecewise continuous function](piecewise-continuous-function.md) $u:[0,T]\to\mathbb R^m$ allowed as a [control input](control-input.md) without an amplitude bound, [controllability](controllability.md) in any fixed $T>0$ is equivalent to the [controllability matrix](controllability-matrix.md) having [rank of a matrix](matrix-rank.md) $n$. The same equivalence holds with all [square-integrable functions](square-integrable-function.md) as inputs. A stronger useful statement is

$$
\mathcal R_T(x_0)=e^{AT}x_0+\operatorname{im}\mathcal C,\qquad T>0,
$$

where $e^{AT}$ is a [matrix exponential](matrix-exponential.md) and $\operatorname{im}\mathcal C$ is the [column space](column-space.md). Thus a [rank of a matrix](matrix-rank.md) $r<n$ leaves only an $r$-dimensional [affine subspace](affine-subspace.md) reachable at that time. [MIT 16.30/31, Feedback Control Systems: Controllability, pages 10–1 to 10–2](https://ocw.mit.edu/courses/16-30-feedback-control-systems-fall-2010/4bebd71d575bdde1384713e9efb400cc_MIT16_30F10_lec10.pdf)

The [Kalman rank criterion](kalman-rank-criterion.md) allows arbitrarily large commands as $T$ shrinks. It does not assert [controllability](controllability.md) with bounded [control inputs](control-input.md), nor test a general nonlinear [dynamical system](dynamical-system.md) just by counting its inputs. For the [double integrator](double-integrator.md), $B=(0,1)^T$ and $AB=(1,0)^T$ give two independent directions, despite there being only one [control input](control-input.md).

## ↑ Ancestors (5)

1. [Controllability](controllability.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Controllability](controllability.md)
- [Controllability Gramian](controllability-gramian.md)
- [Double integrator](double-integrator.md)
- [Kalman rank criterion](kalman-rank-criterion.md)
- [Reachable set](reachable-set.md)
