# Double integrator

↑ **Parent:** [Reachability in control theory](reachability-in-control-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double_integrator)

The [double integrator](double-integrator.md) is the [linear time-invariant system](linear-time-invariant-system.md) in which one [control input](control-input.md) is integrated into [velocity](velocity.md), and [velocity](velocity.md) into [position](position.md). It is a mathematical idealization of one-dimensional motion under commanded [acceleration](acceleration.md); for a constant [mass](mass.md) $m$ and net [force](force-split.md) $F$, [Newton's second law](newton-s-second-law.md) gives $u=F/m$. The worked examples here use normalized [dimensionless quantities](dimensionless-quantity.md) and assume no [control disturbances](control-disturbance.md), rather than describing a laboratory record. [Venkatesh G. Rao and Dennis S. Bernstein, Naive Control of the Double Integrator, pages 87–88](https://www-personal.umich.edu/~dsbaero/others/25-DoubleIntegrator.pdf)

Writing $x=(p,v)^T$ gives

$$
A=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad
B=\begin{pmatrix}0\\1\end{pmatrix},\qquad
\mathcal C=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
\det\mathcal C=-1.
$$

The [Kalman rank criterion](kalman-rank-criterion.md) therefore gives [controllability](controllability.md) in every $T>0$ for unrestricted real [control inputs](control-input.md). More concretely, choose constants $a,b$ on the first and second halves. Starting at $x_0=(p_0,v_0)^T$, direct [integration](integral-split.md) gives

$$
\begin{pmatrix}p(T)-p_0-Tv_0\\v(T)-v_0\end{pmatrix}
=\begin{pmatrix}3T^2/8&T^2/8\\T/2&T/2\end{pmatrix}
\begin{pmatrix}a\\b\end{pmatrix}.
$$

The endpoint map has [determinant](determinant.md) $T^3/8\ne0$, so these two amplitudes can supply any desired endpoint displacement. For a rest-to-rest move of distance $d$, take $a=4d/T^2$, $b=-4d/T^2$. At $T=2$ and $d=1$ these are the two commands in the first figure. No impulse is needed; shorter deadlines require larger finite commands.

## ↑ Ancestors (5)

1. [Reachability in control theory](reachability-in-control-theory.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Controllability](controllability.md)
- [Controllability Gramian](controllability-gramian.md)
- [Double integrator](double-integrator.md)
- [Kalman rank criterion](kalman-rank-criterion.md)
- [Reachability in control theory](reachability-in-control-theory.md)
- [Reachable set](reachable-set.md)
