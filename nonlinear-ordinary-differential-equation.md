# Nonlinear ordinary differential equation

↑ **Parent:** [Ordinary differential equation](ordinary-differential-equation.md)

A [nonlinear ordinary differential equation](nonlinear-ordinary-differential-equation.md) depends nonlinearly on the unknown [function](function-split.md) or its [derivatives](derivative.md): it cannot be written in the form defining a [linear differential equation](linear-differential-equation.md). For example, $y'=y^2$ contains a square of the unknown [function](function-split.md), and $y'=y(1-y)$ is a [logistic differential equation](logistic-differential-equation.md). A [coefficient](coefficient.md) such as $t^2$ depending only on the independent variable does not make an [ordinary differential equation](ordinary-differential-equation.md) nonlinear. This distinction concerns dependence on the unknown, rather than the shape of its [function graph](graph-of-a-function.md).

For a concrete [initial value problem](initial-value-problem.md), consider $y'=y^2$, $y(0)=y_0>0$. Its [solution of a differential equation](solution-of-a-differential-equation.md) is

$$
y(t)=\frac{y_0}{1-y_0t},\qquad -\infty<t<\frac1{y_0}.
$$

Taking its [derivative](derivative.md) gives $y'=y_0^2/(1-y_0t)^2=y^2$, and evaluating at zero checks the [initial condition](initial-condition.md). The stated [interval](interval-mathematics.md) contains zero and ends at [finite-time blowup](finite-time-blowup.md): $y$ tends to positive infinity as $t$ approaches $1/y_0$ from below. Increasing the positive [initial condition](initial-condition.md) brings [finite-time blowup](finite-time-blowup.md) closer. This is a simple mathematical example with [dimensionless](dimensionless-quantity.md) $t$ and $y$, rather than a calibrated physical model.

Choose $y_0=1$ and $y_0=2$, giving $y_1=1/(1-t)$ and $y_2=2/(1-2t)$. At $t=1/4$ they have values $4/3$ and $4$, so their sum $s=y_1+y_2$ has value $16/3$. On the common [interval](interval-mathematics.md) $0\leq t\leq0.4$, both are valid [solutions of a differential equation](solution-of-a-differential-equation.md), but their sum fails the same [ordinary differential equation](ordinary-differential-equation.md):

$$
s'-s^2=y_1^2+y_2^2-(y_1+y_2)^2=-2y_1y_2\ne0.
$$

Already at $t=0$, $s=3$ and its [derivative](derivative.md) is $1+4=5$, whereas $y'=y^2$ would require $9$. At $t=1/4$, the defect $s'-s^2$ is $-32/3$. The cross term explains the failure of the [superposition principle](superposition-principle.md), even though each individual [solution of a differential equation](solution-of-a-differential-equation.md) is a [smooth function](smooth-function.md).

<a id="image-two-solutions-of-a-differential-equation-for-y-y-2-have-a-sum-with-a-nonzero-defect"></a>
![](linear-versus-nonlinear-ode.png)

**[Figure 5](#image-two-solutions-of-a-differential-equation-for-y-y-2-have-a-sum-with-a-nonzero-defect). Two solutions of a differential equation for $y'=y^2$ have a sum with a nonzero defect**.

The first panel shows $y_1$, $y_2$ and their invalid sum only up to $t=0.4$, before either [finite-time blowup](finite-time-blowup.md). The second measures the defect in the [ordinary differential equation](ordinary-differential-equation.md), including the computed value at $t=1/4$. For a [homogeneous linear differential equation](homogeneous-linear-differential-equation.md), the corresponding defect of a sum is zero. [Nonlinear ordinary differential equations](nonlinear-ordinary-differential-equation.md) can describe state-dependent growth such as the [logistic differential equation](logistic-differential-equation.md), whose negative quadratic term limits growth instead of accelerating it without bound. Recognizing the distinction tells us when we may assemble [solutions of a differential equation](solution-of-a-differential-equation.md) from simpler pieces and when we must account for their interaction. See [MIT's worked counterexample to nonlinear superposition](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/be944aa565ebdaa2f9e369e5128d4641_IrRgAWI6bmw.pdf).

**Table of contents**

- [Ermakov-Pinney equation](ermakov-pinney-equation.md)
  - [Exact amplitude-phase equation](exact-amplitude-phase-equation.md)
- [Position-dependent damping](position-dependent-damping.md)
- [Logistic differential equation](logistic-differential-equation.md)
  - [Euler discretization of logistic growth](euler-discretization-of-logistic-growth.md)

## ↑ Ancestors (6)

1. [Ordinary differential equation](ordinary-differential-equation.md)
2. [Differential equation](differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Linear differential equation](linear-differential-equation.md)
- [Logistic differential equation](logistic-differential-equation.md)
- [Nonlinear ordinary differential equation](nonlinear-ordinary-differential-equation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-317/3/ii/solution.md)
