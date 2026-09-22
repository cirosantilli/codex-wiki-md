<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce independent fast and slow times

$$
t_0=t,
\qquad
T=\epsilon t,
$$

and seek $u=u_0+\epsilon u_1+\cdots$. Then

$$
\frac d{dt}=\partial_{t_0}+\epsilon\partial_T,
\qquad
\frac{d^2}{dt^2}
=\partial_{t_0}^2
+2\epsilon\partial_{t_0T}+O(\epsilon^2).
$$

At leading order,

$$
u_{0,t_0t_0}+u_0=0,
$$

so write

$$
u_0=R(T)\cos\theta,
\qquad
\theta=t_0+\phi(T).
$$

At order $\epsilon$,

$$
u_{1,t_0t_0}+u_1
=f(u_0,u_{0,t_0},T)
+2R'\sin\theta
+2R\phi'\cos\theta.
$$

The [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md) removes the resonant sine and cosine components. Averaging over one fast period gives the [amplitude-phase equations for a weakly perturbed oscillator](../../../../../../amplitude-phase-equations-for-a-weakly-perturbed-oscillator.md)

$$
\boxed{
\frac{dR}{dT}
=-\langle f\sin\theta\rangle},
\qquad
\boxed{
R\frac{d\phi}{dT}
=-\langle f\cos\theta\rangle}.
$$

**Therefore $u\sim R(T)\cos[t+\phi(T)]$ without the secular growth that a single-time expansion would produce.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
