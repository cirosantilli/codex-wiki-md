# Monodromy matrix of a periodic linear system

↑ **Parent:** [Floquet theory](floquet-theory.md)

For the homogeneous [linear differential equation](linear-differential-equation.md) $\dot Y=K(t)Y$ with continuous coefficient matrix of period $P>0$, the [monodromy matrix of a periodic linear system](monodromy-matrix-of-a-periodic-linear-system.md) is the one-period map from $Y(0)$ to $Y(P)$. If $X$ is any [fundamental matrix](fundamental-matrix-of-a-linear-differential-equation.md),

$$
N=X(P)X(0)^{-1},\qquad Y(P)=NY(0).
$$

Its [eigenvalues](eigenvalue.md) are the [Floquet multipliers](floquet-multiplier.md). Multipliers are nonzero, since a [fundamental matrix](fundamental-matrix-of-a-linear-differential-equation.md) is invertible. Changing the starting phase conjugates $N$, so the [Floquet multipliers](floquet-multiplier.md) and [Jordan blocks](jordan-block.md) are independent of that choice.[§3.6, printed pp. 91–93, equations (3.119), (3.122) and (3.127)](ordinary-differential-equations-and-dynamical-systems-by-gerald-teschl.md)

This turns a continuous-time problem into repeated [matrix multiplication](matrix-multiplication.md):

$$
Y(nP)=N^nY(0).
$$

If $Nv=mv$, the associated [solution of a differential equation](solution-of-a-differential-equation.md) obeys $Y(t+P)=mY(t)$ at every time, not merely at the sampled times. In particular, $Nv=v$ gives a nonzero $P$-[periodic solution](periodic-solution.md), and every nonzero $P$-[periodic solution](periodic-solution.md) arises this way. If $Nv=-v$, the state changes sign after one period and repeats after two. A unit-modulus [Floquet multiplier](floquet-multiplier.md) different from $1$ need not give repetition after one period, and a [generalized eigenvector](generalized-eigenvector.md) in a nontrivial [Jordan block](jordan-block.md) need not even give bounded motion.

For the scalar example under [periodic solution](periodic-solution.md), $N$ is the one-by-one matrix $(e^{2\pi a})$. Numerically solving a matrix problem uses the same idea: integrate one [initial value problem](initial-value-problem.md) for each column of $X(0)=I$ through one period, then compute the [eigenvalues](eigenvalue.md) of $X(P)$. This is useful when an explicit [solution of a differential equation](solution-of-a-differential-equation.md) is unavailable: one period determines the [Floquet growth rate](floquet-growth-rate.md) over arbitrarily many periods.

For piecewise constant coefficients, which are also covered by the one-period construction, $N$ is the time-ordered product of the segment [matrix exponentials](matrix-exponential.md), with the earliest segment on the right. For example, take period $P=2$ and alternate

$$
K_1=\begin{pmatrix}0&1\\0&0\end{pmatrix}\quad(0\leq t<1),\qquad K_2=\begin{pmatrix}0&0\\1&0\end{pmatrix}\quad(1\leq t<2).
$$

Since $K_1^2=K_2^2=0$,

$$
N=e^{K_2}e^{K_1}=\begin{pmatrix}1&1\\1&2\end{pmatrix},\qquad m_\pm=\frac{3\pm\sqrt5}{2},\qquad \gamma=\frac12\log\frac{3+\sqrt5}{2}\approx0.4812.
$$

Replacing the coefficient by its mean would instead give $e^{K_1+K_2}=\left(\begin{smallmatrix}\cosh1&\sinh1\\\sinh1&\cosh1\end{smallmatrix}\right)$ and the incorrect rate $0.5$. The [matrices](matrix.md) do not commute. The scalar mean-coefficient formula therefore cannot simply be transferred to matrix systems. Nevertheless the [Liouville formula for a fundamental matrix](liouville-formula-for-a-fundamental-matrix.md) gives the correct [determinant](determinant.md) even in the noncommuting case:

$$
\det N=\exp\left(\int_0^P\operatorname{tr}K(t)\,dt\right).
$$

In the example, this is $1=m_+m_-$; it fixes the product of the [Floquet multipliers](floquet-multiplier.md), rather than either multiplier separately.

In Sur les équations différentielles linéaires à coefficients périodiques (1883), [Gaston Floquet](gaston-floquet.md) calls a function satisfying $f(t+P)=mf(t)$ periodic of the second kind, and distinguishes the genuinely [periodic function](periodic-function.md) obtained when $m=1$. This historical terminology captures precisely the difference between repetition of the coefficient and repetition of the state.[Printed p. 48, definition of a function periodic of the second kind and its multiplier; p. 49, transformation of a fundamental solution system after one period](sur-les-equations-differentielles-lineaires-a-coefficients-periodiques-by-gaston-floquet-1883.md)

## ↑ Ancestors (8)

1. [Floquet theory](floquet-theory.md)
2. [Linear differential equation](linear-differential-equation.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Floquet multiplier](floquet-multiplier.md)
- [Monodromy matrix of a periodic linear system](monodromy-matrix-of-a-periodic-linear-system.md)
- [Parker dynamo wave](parker-dynamo-wave.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-318/2/solution.md)
- [Periodically reversing Parker dynamo coupling](periodically-reversing-parker-dynamo-coupling.md)
