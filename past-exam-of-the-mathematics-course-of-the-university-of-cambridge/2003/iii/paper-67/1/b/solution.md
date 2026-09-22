<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Q(y)=y^TSy$. In the usual pointwise meaning of an [ODE invariant](../../../../../../first-integral-of-an-ordinary-differential-equation.md), differentiation along an exact solution through an arbitrary state gives

$$
\frac d{dt}Q(y(t))=2y^TSf(t,y)=0.
$$

For a nonautonomous equation this identity must hold at the stage time as well as at the initial time. It follows directly from invariance for solutions started at any time and state, or from the stated initial-time invariance when the exact flow onto the stage-time domain is invertible. This is the first-integral condition used below.

Put $Y=(y_n+y_{n+1})/2$ and $t_*=t_n+h/2$. Since $S$ is symmetric,

$$
Q(y_{n+1})-Q(y_n)
=(y_{n+1}+y_n)^TS(y_{n+1}-y_n)
=2hY^TSf(t_*,Y)=0.
$$

Induction over all well-defined implicit steps gives

$$
\boxed{y_n^TSy_n=y_0^TSy_0.}
$$

No positive-definiteness assumption on $S$ was used. Nor is uniqueness of the stage essential to this algebraic identity: any stage solution satisfying the method and the pointwise invariant condition preserves $Q$. This is the one-stage case of [Runge-Kutta conservation of quadratic invariants](../../../../../../runge-kutta-conservation-of-quadratic-invariants.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
