# Finite-time blowup

↑ **Parent:** [Ordinary differential equation](ordinary-differential-equation.md)

A [solution of a differential equation](solution-of-a-differential-equation.md) has [finite-time blowup](finite-time-blowup.md) in norm when $\|y(t)\|\to\infty$ as $t$ approaches a finite endpoint $T$ of its maximal [interval](interval-mathematics.md) of existence. This is stronger than merely approaching an excluded [boundary](boundary-of-a-set.md) of an open state domain while staying bounded. The [finite-dimensional continuation criterion](finite-dimensional-continuation-criterion.md) distinguishes these obstructions; for a locally [Lipschitz continuous](lipschitz-continuity.md) [ordinary differential equation](ordinary-differential-equation.md) on $I\times\mathbb R^d$, a finite maximal endpoint inside $I$ necessarily entails [finite-time blowup](finite-time-blowup.md).

A simple example with a smooth right-hand side is

$$
y'=1+y^2,\qquad y(0)=0,\qquad y(t)=\tan t,\qquad -\frac\pi2<t<\frac\pi2.
$$

The [derivative](derivative.md) identity $(\tan t)'=1+\tan^2t$ verifies the equation and the [initial condition](initial-condition.md). Also $|u^2-v^2|=|u-v||u+v|\leq2R|u-v|$ for $|u|,|v|\leq R$, giving local [Lipschitz continuity](lipschitz-continuity.md) and therefore uniqueness. Yet the positive blowup time is $T=\pi/2\approx1.57079633$. Computed values show the accelerating growth:

$$
y(1)\approx1.55740772,\qquad y(1.4)\approx5.79788372,\qquad y(1.5)\approx14.10141995.
$$

The right panel under the [Picard-Lindelöf theorem](picard-lindelof-theorem.md) deliberately clips its vertical axis at $10$: the trajectory has already left the picture at $t=\arctan10\approx1.47112767$, before reaching $T$. A plot ceiling is a display limit, not a finite value at blowup.

The [tangent function](tangent-function.md) also quantifies the last part of the trajectory. With $\delta=T-t>0$,

$$
y(T-\delta)=\frac{\cos\delta}{\sin\delta},\qquad \delta\,y(T-\delta)\longrightarrow1\quad(\delta\downarrow0).
$$

Thus the height is approximately the reciprocal of the remaining time. At remaining times $\delta=0.1,0.01,0.001$, the heights are approximately $9.96664442,99.99666664,999.99966667$. These follow from the [sine](sine.md) and [cosine](cosine.md) limits at zero and explain the steep rise without relying on the appearance of a clipped [function graph](graph-of-a-function.md).

The distinction is useful when interpreting a [solution of a differential equation](solution-of-a-differential-equation.md): uniqueness certifies a trajectory while it exists, while growth estimates decide how far it can be followed. For $y'=1+y^2$, the [Lipschitz constant](lipschitz-constant.md) $2R$ on a bounded state [interval](interval-mathematics.md) grows with $R$, and the right-hand side grows quadratically. There is no global [Lipschitz constant](lipschitz-constant.md) or linear-growth bound of the kind used by the [finite-dimensional continuation criterion](finite-dimensional-continuation-criterion.md). Smoothness at every finite state is entirely compatible with [finite-time blowup](finite-time-blowup.md).

## ↑ Ancestors (6)

1. [Ordinary differential equation](ordinary-differential-equation.md)
2. [Differential equation](differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Bernoulli differential equation](bernoulli-differential-equation.md)
- [Explosive two-to-one amplitude system](explosive-two-to-one-amplitude-system.md)
- [Finite-dimensional continuation criterion](finite-dimensional-continuation-criterion.md)
- [Finite-time blowup](finite-time-blowup.md)
- [Initial value problem](initial-value-problem.md)
- [Nonlinear ordinary differential equation](nonlinear-ordinary-differential-equation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-336/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-105/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/13/b/solution.md)
- [Peano existence theorem](peano-existence-theorem.md)
- [Picard-Lindelöf theorem](picard-lindelof-theorem.md)
- [Reciprocal Bernoulli equation with finite-time blowup](reciprocal-bernoulli-equation-with-finite-time-blowup.md)
- [Retarded delay differential equation](retarded-delay-differential-equation.md)
