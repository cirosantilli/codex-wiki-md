# Controllability Gramian

↑ **Parent:** [Controllability](controllability.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Controllability_Gramian)

For $T>0$ and the constant [matrices](matrix.md) over the [real numbers](real-number.md) in the [Kalman rank criterion](kalman-rank-criterion.md), the finite-time [Controllability Gramian](controllability-gramian.md) accumulates the influence of all command times. Its [column space](column-space.md) equals that of the [controllability matrix](controllability-matrix.md), and $W_T$ is a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) exactly when the [controllability matrix](controllability-matrix.md) has [rank of a matrix](matrix-rank.md) $n$. If so, put $\delta=x_1-e^{AT}x_0$. Among [square-integrable functions](square-integrable-function.md) steering $x_0$ to $x_1$ at $T$, the command

$$
u_*(t)=B^Te^{A^T(T-t)}W_T^{-1}\delta
$$

minimizes $\int_0^T\|u(t)\|^2\,dt$, with value $\delta^TW_T^{-1}\delta$. Here $T$ in a matrix superscript denotes [transpose](transpose.md). This cost is a squared input [norm](norm.md), not necessarily physical [energy](energy.md), and the optimizing command need not satisfy an amplitude bound. [Stephen Boyd, EE263: Controllability and state transfer, slides 18–29 to 18–30](https://ee263.stanford.edu/archive/contr.pdf)

For the [double integrator](double-integrator.md), $e^{As}B=(s,1)^T$, so direct [integration](integral.md) gives

$$
W_T=\begin{pmatrix}T^3/3&T^2/2\\T^2/2&T\end{pmatrix},\qquad
\det W_T=\frac{T^4}{12}>0.
$$

For a rest-to-rest distance $d$, $u_*(t)=6d/T^2-12dt/T^3$ and the minimum squared input [norm](norm.md) is $12d^2/T^3$. Compare the two constant commands in the [double integrator](double-integrator.md) example, whose cost is $16d^2/T^3$: both attain the target, but the smooth command costs less. At $T=2$, $d=1$, however, $u_*$ peaks at $3/2$, so it violates $|u|\le1$ while the two constant commands remain admissible. [Controllability](controllability.md), [optimal control](optimal-control.md), and constrained [reachability in control theory](reachability-in-control-theory.md) answer different questions.

## ↑ Ancestors (5)

1. [Controllability](controllability.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Controllability Gramian](controllability-gramian.md)
